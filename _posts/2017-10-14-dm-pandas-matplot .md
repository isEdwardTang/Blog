---
layout: post
title: "数据挖掘之数据可视化二"
categories: DataMining
tags:	python primer datamining
author: Edward
---

* content
{:toc}

pandas封装了matplotlib的绘图函数，并结合DataFrame和Series等数据类型，使绘图更简洁。

--------------------

## 一、线型图

默认Series和DataFrame的plot方法生成的是线型图。

- 直接调用Series对象的plot方法即可以其索引作为x轴，绘制二维图

```python
s = Series(np.random.randn(10).cumsum(), index=np.arange(0, 100, 10))
s.plot()
```

![Series.plot方法绘图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/series_fig.svg)

| 参数 | 说明 |
| :--- | :--- |
| kind | 可以是'line', 'bar', 'barh', 'kde' |
| logy | 再y轴上使用对数标尺 |
| use_index | 将对象的索引用作刻度标签 |
| rot | 旋转刻度标签(0到360） |
| xticks | 用作X轴刻度的值 |
| yticks | 用作y轴刻度的值 |
| xlim | x轴的界限 |
| ylim | y轴的界限 |
| grid | 显示轴网格线，默认打开 |

- 调用DataFrame对象的plot方法会再一个subplot中为各列绘制一条线，并自动创建图例

```python
df = DataFrame(np.random.randn(10, 4).cumsum(0), columns=['A', 'B', 'C', 'D'], index=np.arange(0, 100, 10))
df.plot()
```
![DataFrame.plot方法绘图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dataframe_fig.svg)

| 参数 | 说明 |
| :--- | :--- |
| subplots | 将各个DataFrame列绘制到单独的subplot中 |
| sharex | subplots为True时，共用一个X轴 |
| sharey | subplots为True时，共用一个y轴 |
| figsize | 表示图像大小的元祖 |
| title | 表示图像标题的字符串 |
| legend | 添加图例(默认为True |
| sort_columns | 按照排序后绘制各列，默认为当前列顺序 |

## 二、柱状图 

在使用plot方法时，参数kind指定为'bar'为垂直柱状图，'barh'为水平柱状图 

Series：

```python
fig, axes = plt.subplots(2, 1)
data = Series(np.random.rand(16), index=list('abcdefghijklmnop'))
data.plot(kind='bar', ax=axes[0], color='k', alpha=0.7)
data.plot(kind='barh', ax=axes[1], color='k', alpha=0.7)
```

![series柱状图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/series_bar.svg)

而对于DataFrame，会将每一行的值分为一组：

```python
df = DataFrame(np.random.rand(6, 4), index=['one', 'two', 'three', 'four', 'five', 'six'], columns=pd.Index(['A', 'B', 'C', 'D'], name='Genus'))
df.plot(kind='bar')
```

![DataFrame柱状图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dataframe_bar.svg)

设置stacked=True，则DataFrame生成堆积柱状图：

![DataFrame堆积柱状图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dataframe_barh_stack.svg)

## 三、直方图和密度图

直方图是对值频率进行离散化显示的柱状图，使用hist方法，使用参数bins来指定直方的数量：

```python
s = Series(np.random.randn(100))
s.hist(bins=30)
```

![直方图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/hist.svg)

而密度图是观测数据的连续概率分布的估计，也称KDE图，在调用plot时加上kind='kde'即可绘制：

```python
s = Series(np.random.randn(100))
s.plot(kind='kde')
```

![密度图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/svg.svg)

通常情况下，直方图和密度图通常放在一起绘制：

```python
comp1 = np.random.normal(0, 1, size=200) # N(0, 1)
comp2 = np.random.normal(10, 2, size=200) # N(10, 4)
values = Series(np.concatenate([comp1, comp2]))
values.hist(bins=100, alpha=0.3, color='k', normed=True)
values.plot(kind='kde', style='k--')
```

![直方图和密度图混合](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/hist_kde.svg)

## 四、散点图

使用scatter方法即可绘制散点图：

```python
macro = pd.read_csv('macrodata.csv')	# statsmodels的macrodata数据集
data = macro[['cpi', 'm1', 'tbilrate', 'unemp']]
trans_data = np.log(data).diff().dropna()
plt.scatter(trans_data['m1'], trans_data['unemp'])
```

![散点图](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/scatter.svg)

通过scatter_matrix()方法可以创建散点图矩阵：

```python
pd.plotting.scatter_matrix(trans_data, diagonal='kde', color='k', alpha=0.3)
```

![散点图矩阵](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/scatter_matrix.svg)










