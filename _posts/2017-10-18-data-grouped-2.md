---
layout: post
title: "数据聚合和分组二"
categories: DataMining
tags:   python primer datamining
author: Edward
---

* content
{:toc}

之前介绍的聚合接受一个将一维数组转化为标量值的函数，比如sum等，而广泛意义上的分组运算可以将数组转为数组，主要是transform和apply函数。另外数据分析中，透视表和交叉表也会经常用到。

--------------------

## 一、分组级运算及转换

### 1、transform

和agg不用的是，transform函数会将其应用的函数应用到各个分组，如果各个分组产生的是一个标量值，则该值就会被广播出去，下面是一个例子解释他们之间的区别：

```python
df = DataFrame({'key1':['a', 'b', 'b', 'b', 'a'], 'key2': ['one', 'two', 'one', 'two', 'one'], 'data1':np.random.randn(5), 'data2':np.random.randn(5)})
"""
	data1	data2	key1	key2
0	-0.723126	0.385757	a	one
1	0.110773	-0.141002	b	two
2	1.274471	-0.200288	b	one
3	-0.866229	0.030493	b	two
4	1.691484	0.924895	a	one
"""

df.groupby('key1').agg('mean')
"""
	 data1	     data2
key1		
a	0.484179	0.655326
b	0.173005	-0.103599
"""

df.groupby('key1').transform('mean')
"""
	 data1	     data2
0	0.484179	0.655326
1	0.173005	-0.103599
2	0.173005	-0.103599
3	0.173005	-0.103599
4	0.484179	0.655326
"""
```

- 实现分组距平化(某个数和平均值的差值)：

```python
def demean(arr):
    return arr - arr.mean()

demeaned = arr.groupby(key).transform(demean)
```

### 2、apply

apply函数将待处理的对象分成多个片段，然后对各个片段调用传入的函数，最终将各个片段组合在一起。apply相比transform和agg来说更通用，并且可以给函数传入指定的参数：`arr.groupby(key).apply(arrs, arg1=0)`。由于apply函数相当灵活，这里举几个例子。

apply应用举例：



## 二、透视表和交叉表

### 1、透视表

透视表根据一个或多个键进行聚合，并根据行和列的分组键将数据分配到各个矩形区域。使用DataFrame或pandas的pivot_table函数即可实现：

```python
df
"""
	one	two	three four five	six
1	 1	 2	 3	    a	Y	F
2	 4	 5	 6	    a   Y	T
3	 7	 8	 9	    b	N	F
4	 10	11	12	    b	N	T
5	 13	14	15	    a	Y	F
"""

df.pivot_table(index=['four', 'six'], columns='five')
"""
           one	   two	   three
five	N	Y	N	Y	N	Y
four six						
a	 F	NaN	7.0	NaN	8.0	NaN	9.0
     T	NaN	4.0	NaN	5.0	NaN	6.0
b	 F	7.0	NaN	8.0	NaN	9.0	NaN
     T	10.0NaN	11.0NaN	12.0NaN
"""

```

可以指定要聚合的列，及分组后的列和行，详细参数如下：

| 参数名 | 说明 |
| :--- | :--- |
| values | 待聚合的列名，默认聚合所有数值列 |
| index | 用于分组的列名或者其他分组键，放在透视表的行 |
| columns | 用于分组的列名或者其他分组键，放在透视表的列 |
| aggfunc | 聚合函数或函数列表，默认为mean |
| fill_valus | 用于替换结果表中的缺失值 |
| margins |  添加行列小计和总计，默认为False |

### 2、交叉表 

交叉表是一种用于计算分组频率的特殊透视表：

```python
df
"""
 Gender	isSmoking
1	M	True
2	M	True
3	F	True
4	M	False
5	F	False
6	F	True
"""

pd.crosstab(df.Gender, df.isSmoking, margins=True)
"""
isSmoking	False	True	All
Gender			
F	        1	    2	    3
M	        1	    2	    3
All	        2	    4	    6
"""
```

第一个参数和第二个参数分别指列和行