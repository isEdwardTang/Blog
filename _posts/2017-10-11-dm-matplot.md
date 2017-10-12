---
layout: post
title: "数据挖掘之数据可视化一"
categories: DataMining
tags:	python primer datamining
author: Edward
---

* content
{:toc}

绘图是数据分析中一个非常重要的工作，python中有很多可视化工具，这里主要介绍最常用的matplot。

--------------------

## 一、启用matplot

- 在ipython中，使用%matplotlib inline启动

- 在ipython中，使用%gui启动GUI事件循环集成

- 在pycharm等IDE中，需要显式使用show()方法

使用import matplotlib.pyplot as plt导入。

## 二、Figure和Subplot

### 1、使用figure和add_subplot

- 首先需要创建一个Figure：`fig = plt.figure()`

- 需要在Figure中使用add_subplot创建一个或多个subplot：`ax1 = fig.add_subplot(2, 2, 1)`，即可选中2x2的subplot中的第1个

- 使用plot方法绘制图形：`plt.plot(randn(50).cumsum(), 'k--')`，会使用最后一次创建的subplot进行绘图，或者调用add_subplot返回的 AxesSubplot对象的实例方法绘制：`ax1.hist(randn(100), bins=20, color='k', alpha=0.3)`

figure即最终绘制的图形。

figure的参数


add_subplot的参数



### 2、使用subplots

创建figure和subplot可以合并到一步，即使用：`fig, axes = plt.subplots()`，subplots函数返回一个figure和一个Axes数组构成的元组，这样我们可以直接通过axes来获取各个subplots。

subplots的参数介绍如下：

| 参数 | 说明 |
| :--- | :--- |
| nrows | subplot的行数 |
| ncols | subplot的列数 |
| sharex | 所有subplot应该使用的x轴刻度 |
| sharey | 所有subplot应该使用的y周刻度 |
| subplot_kw | 用于创建各个subplot的关键字的字典 |
| **fig_kw | 创建figure的其他关键字，如figsize |

### 3、调整间距

使用figure的subplots_adjust方法修改间距：`subplots_adjust(left=None, bottom=None, right=None,top=None, wspace=None, hspace=None)`，其中wspace和hspace可以用来调整间距

其他参数的作用

## 三、颜色、标记、线型

matplotlib的plot函数接受一个x和y坐标，即一个表示颜色和线型的字符串缩写，如`ax.plot(x, y, 'g--')`；或者分别指定颜色和线型：`ax.plot(x, y, linestyle='--', color='g')`；还可以使用marker参数来指定标记，以及使用drawstyle来指定插入的方式：

plot的具体参数

linestyle

color
常用颜色可以用其的缩写词，要使用其他颜色可以指定rgb值

## 四、刻度、标签、图例



## 五、注解

## 六、保存图表