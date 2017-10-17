---
layout: post
title: "数据聚合和分组一"
categories: DataMining
tags:   python primer datamining
author: Edward
---

* content
{:toc}

对数据集分组并对各组应用同一个函数，是数据分析中重要的环节。

--------------------

## 一、GroupBy技术

### 1、分组运算

分组运算的三个步骤(拆分、应用、合并)：

- 首先pandas对象中的数据根据提供的一个或多个键被拆分为多组
- 然后将一个函数应用到各个分组并产生一个新值
- 所有函数的结果被合并到最终的结果对象中

### 2、分组键

分组键的几种形式：

- 列表或数组，长度和带分组的轴一样
- 表示DataFrame某个列名的值
- 字典或Series，给出分组轴的值和分组名之间的对应关系
- 函数，用于处理轴索引或索引中的各个标签

### 3、groupby方法使用

```python
df = DataFrame({'key1':['a', 'b', 'b', 'b', 'a'], 'key2': ['one', 'two', 'one', 'two', 'one'], 'data1':np.random.randn(5), 'data2':np.random.randn(5)})
grouped = df['data1'].groupby(df['key1'])
grouped.mean()
"""
key1
a   -0.472460
b    0.816076
Name: data1, dtype: float64
"""
```

调用groupby函数对DataFrame按照指定的键进行分组，获得GroupBy对象，但是实际上还没有进行任何计算，再对GroupBy对象调用各种聚合函数，即可进行分组计算。

这里的groupby的参数可以指定多个：`df['data1'].groupby([df['key1'], df['key2']])`或`df['data1'].groupby(['key1', 'key2'])`

- 注意，对数据进行聚合时，只会聚合数值数据，其他数据会从结果中排除：

```python
df.groupby(['key1']).mean()
"""
	    data1	  data2
key1		
a	-0.472460	-0.162090
b	0.816076	-0.090764
"""
```

- 使用grouby的size方法，可以返回一个含有分组大小的Series：

```python
df.groupby(['key1', 'key2']).size()
"""
key1  key2
a     one     2
b     one     1
      two     2
dtype: int64
"""
```

### 4、分组迭代

GroupBy对象可以进行迭代，获得一组二元元组，由分组名和数据块组成：

```python
for name, group in df.groupby('key1'):
    print(name)
    print(group)
"""
a
      data1     data2 key1 key2
0  0.242362  0.310389    a  one
4 -1.187282 -0.634568    a  one
b
      data1     data2 key1 key2
1  0.563591  0.759411    b  two
2  0.785510  0.409223    b  one
3  1.099126 -1.440928    b  two
"""
```

如果键由多个组成，则同样由一个元组组成，不过元组的第一个元素也是一个元组，包含各个键。

- 有一个技巧可以把这些数据片段转换成字典：`pieces = dict(list(df.groupby('key1')))`

默认是在axis=0上进行分组的，也可以指定：`df.groupby('key1', axis=1)`

### 5、选取指定列

使用如下两种方式可以对指定列进行聚合：

- `df.groupby('key1')['data1']` `df.groupby('key1')[['data1' ,'data2']]`
- `df['data1'].groupby('key1')` `df[['data1', 'data2']].groupby('key1')`

### 6、通过字典或Series进行分组

字典的键对应实际DataFrame的列名，然后按照字典的值进行分组，相当于重命名列名并分组，Series类似。

### 7、通过函数进行分组

可以传入一个函数作为分组键，则该函数会在各个索引值上都调用一次，调用的返回值作为分组名称。
同时，函数、字典、Series、列表等混合使用也是可以的

### 8、通过索引级别分组

可以通过传入level关键字，来指定级别的编号或名称，按照指定级别分组

```python
columns = pd.MultiIndex.from_arrays([['CH', 'CH', 'CH', 'UA', 'UA'], [1, 2, 4, 1, 2]], names=['cty', 'tenor'])
hier_df = DataFrame(np.random.randn(4, 5), columns=columns)
"""
cty	                            CH	                    UA
tenor	    1	    2	        4	        1	        2
0	-1.303821	-0.537588	-0.072974	-1.175556	-0.092518
1	0.716616	-0.410726	-0.315785	-1.233117	0.724270
2	-0.422716	-0.860589	-1.844820	0.045313	0.794942
3	-0.572299	-0.767250	1.036550	-0.640327	-0.781942
"""
hier_df.groupby(level='cty', axis=1).mean()
"""
cty	    CH	         UA
0	-0.638128	-0.634037
1	-0.003298	-0.254424
2	-1.042709	0.420127
3	-0.101000	-0.711135
"""
hier_df.groupby(level='tenor', axis=1).mean()
"""
tenor	1	        2	        4
0	-1.239688	-0.315053	-0.072974
1	-0.258250	0.156772	-0.315785
2	-0.188702	-0.032824	-1.844820
3	-0.606313	-0.774596	1.036550
"""
```

## 二、数据聚合

对Groupby调用聚合函数，或者自定义的对数组操作的聚合函数，可以实现高效的聚合运算。

### 1、优化的聚合函数

其中，以下聚合方法经过优化，速度会比自定义的聚合函数快很多：

| 函数名 | 说明 |
| :--- | :--- |
| count | 分组中非NA值的数量 |
| sum | 分组中非NA值的和 |
| mean | 分组中非NA值的平均值 |
| median | 分组中非NA值的中位数 |
| std、var | 分组中非NA值的无偏标准差、方差 |
| min、max | 分组中非NA值的最小值、最大值 |
| prod | 分组中非NA值的积 |
| first、last | 分组中第一个、最后一个非NA值 |

### 2、自定义的聚合函数

可以使用自定义的聚合函数，然后将其传入agg或aggregate方法即可

### 3、多函数

有些情况下，需要对不同的列使用不同的聚合函数，或者一次应用多个函数。

- 可以使用agg来传入多个函数组成的列表：`df.groupby('key1').agg(['mean', 'count'])`，同时，可以给这个函数去取一个别名(在lambda中特别适合)，传入元组构成的列表：`df.groupby('key1').agg([('one', 'mean'), ('two', 'count')])`

- 想要对不同的列应用不同的函数，可以向agg中传入一个从列名映射到函数的字典：`df.groupby('key1').agg({'data1':'mean', 'data2':'count'})`
