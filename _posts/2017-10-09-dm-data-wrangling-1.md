---
layout: post
title: "数据挖掘之数据规整化一"
categories: DataMining
tags:	python primer datamining
author: Edward
---

* content
{:toc}

数据分析和建模大量时间都是用在数据准备上的，而pandas提供了快速合并数据集的方法，主要是merge和concat两个方法。

--------------------

## 一、merge

### 1、merge简介

merge函数可以根据一个或多个键将不同的DataFrame的行连接起来，相当于关系数据库中的连接操作。

```python
df1 = DataFrame({'key': ['b', 'b', 'a', 'c', 'a', 'a', 'b'], 'data1': range(7)})
df2 = DataFrame({'key': ['a', 'b', 'd'], 'data2': range(3)})
pd.merge(df1, df2)
"""
  data1	key	data2
0	0	b	1
1	1	b	1
2	6	b	1
3	2	a	0
4	4	a	0
5	5	a	0
"""
```

### 2、merge使用

- merge默认以类名相同的作为键，如果要指定键，使用on参数，如果列名不同，使用left_on和right_on分别指定
- 要根据多个键进行合并时，传入一个列表即可：on=[]
- 合并后列名相同时，可以使用suffixes参数指定列名后缀，默认是_x，_y
- merge默认是inner连接(交集)，可以用how参数来指定其他连接，如outer(全外连接)、left、right
- 有时候，连接的键位于索引中，可以使用lefter_index=True和right_index=True来指定使用索引

### 3、merge参数

下面是merge函数的参数的说明：

| 参数 | 说明 |
| :--- | :--- |
| left | 参与合并的左侧DataFrame |
| right | 参与合并的右侧DataFrame |
| how | 合并方式，默认为inner，还有outer,left,right |
| on | 用于连接的列名，如果未指定，以left和right的列名的交集作为连接键 |
| left_on | 左侧DataFrame中用于连接的键 |
| right_on | 右侧DataFrame中用于连接的键 |
| left_index | 将左侧的行索引作为连接键 |
| right_index | 将右侧的行索引作为连接键 |
| sort | 根据连接键对合并后的数据进行排序，默认为True |
| suffixes | 字符串元组，用于追加到重叠类名的末尾，默认为('_x', '_y') |
| copy | 默认为True |

### 4、join

还有一个join方法，可以直接按索引合并：`left.join(right)`，默认为左连接。

## 二、concat

之前的合并称为merge，还有一种合并称为concatenation、binding或stacking。

### 1、合并numpy数组

numpy中提供了按照不同轴合并的方法condatencation：

```python
arr = np.arange(12).reshape((3, 4))
np.concatenate([arr, arr], axis=1)  # 按照列合并
"""
array([[ 0,  1,  2,  3,  0,  1,  2,  3],
       [ 4,  5,  6,  7,  4,  5,  6,  7],
       [ 8,  9, 10, 11,  8,  9, 10, 11]])
"""
```

### 2、concat使用

```python
s1 = Series([0, 1], index=['a', 'b'])
s2 = Series([2, 3, 4], index=['c', 'd', 'e'])
s3 = Series([5, 6], index=['f', 'g'])
pd.concat([s1, s2, s3])
"""
a    0
b    1
c    2
d    3
e    4
f    5
g    6
dtype: int64
"""
```

- 默认是在axis=0上合并，可以指定axis
- 默认是并集(outer)，可以指定join="inner"为交集
- 使用keys指定层次化索引
- 如果传入的不是一个列表，而是一个字典，则字典的键作为key

### 3、concat参数

| 参数 | 说明 |
| :--- | :--- |
| objs | 参与连接的pandas对象的列表或字典，唯一必须的参数 |
| axis | 连接的轴，默认为0 |
| join | 连接方式，inner(交集)或outer(并集)，默认为outer |
| join_axes | 指明用于其他n-1条轴的索引，不进行合并操作 |
| keys | 和连接对象有关的值，用于形成连接轴上的层次化索引 |
| levels | 指定用作层次化索引各级别上的索引 |
| names | 用于创建分层级别的名称 |
| verify_integrity | 检查重复情况，默认为False |
| ignore_index | 不保留连接轴上的索引，产生一组新索引range(length) | 

## 三、combine_first

当存在索引部分或全部重叠的数据集时，可以使用np.where来实现：

```python
a = Series([np.nan, 2.5, np.nan, 3.5, 4.5, np.nan], index=['f', 'e', 'd', 'c', 'b', 'a'])
b = Series(np.arange(len(a), dtype=np.float64), index=['f', 'e', 'd', 'c', 'b', 'a']); b[-1] = np.nan
np.where(pd.isnull(a), b, a)
"""
array([ 0. ,  2.5,  2. ,  3.5,  4.5,  nan])
"""
```

series中的combine_first方法，实现的是相同的功能，他能够用参数中的值替换缺失值：`a.combine_first(b)`
