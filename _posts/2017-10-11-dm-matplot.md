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

figure的参数：

| 参数 | 说明 |
| :--- | :--- |
| num | 如果是int，则作为该figure的唯一标识，如果是string，则作为title使用，如果不存在，则会自动创建一个 |
| figsize | 一个表示图形width、height(inches)的元组 |
| dpi | 图形的分辨率 |
| facecolor | 图形的背景色 |
| edgecolor | 图形的边框色 |
| frameon | 默认为True，如果是False，则不会绘制图形的框架 |
| clear | 默认为False，如果是True，则图形已经存在会被clear掉 | 


add_subplot方法可以使用三个整数作为参数：`fig.add_subplot(2, 2, 1)`，分别表示subplot的行数、列数和这个subplot所在的位置，返回一个Axes，并且这三个参数可以简写成一个：`fig.addsubplot(221)`。

### 2、使用subplots

创建figure和subplot可以合并到一步，即使用：`fig, axes = plt.subplots()`，subplots函数返回一个figure和一个Axes数组构成的元组，这样我们可以直接通过axes来获取各个subplots。

subplots的参数介绍如下：

| 参数 | 说明 |
| :--- | :--- |
| nrows | subplot的行数 |
| ncols | subplot的列数 |
| sharex | 所有subplot应该使用的x轴刻度 |
| sharey | 所有subplot应该使用的y轴刻度 |
| subplot_kw | 用于创建各个subplot的关键字的字典 |
| **fig_kw | 创建figure的其他关键字，如figsize |

### 3、调整间距

使用figure的subplots_adjust方法修改间距：`subplots_adjust(left=None, bottom=None, right=None,top=None, wspace=None, hspace=None)`，其中wspace和hspace可以用来调整subplot之间的间距，而其他四个参数分别指的是figure的左下角的坐标和右上角的坐标。

## 三、颜色、标记、线型

matplotlib的plot函数接受一个x和y坐标，即一个表示颜色和线型的字符串缩写，如`ax.plot(x, y, 'g--')`；或者分别指定颜色和线型：`ax.plot(x, y, linestyle='--', color='g')`；还可以使用marker参数来指定标记，以及使用drawstyle来指定插入的方式。

### 1、坐标

有以下几种方式来指定要描绘的坐标或图形：

- 直接分别指定x和y：`ax.plot(x, y)`，则可绘制y关于x的二维图形

- 只指定y：`ax.plot(y)`，则把y数组的inde作为x来绘制

- 含有多条曲线，必须同时指定x, y, 以及其他颜色线型的参数：`ax.plot(x1, y1, 'g^', x2, y2, 'g-')`

### 2、线型或者标记的字符

可以在参数中直接使用字符串，或使用参数linestyle和marker

| 字符 | 描述 |
| :--- | :--- |
| '-' | 实线 |
| '--' | 虚线 |
| '-.' | 点划线 |
| ':' | 点线 |
| '.' | 点标记 |
| ',' | 像素标记 |
| 'o' | 圆圈标记 |
| 'v' | 下三角标记 |
| '^' | 上三角标记 |
| '<' | 左三角标记 |
| '>' | 右三角标记 |
| '1' | 下花三角标记 |
| '2' | 上花三角标记 |
| '3' | 左花三角标记 |
| '4' | 右花三角标记 |
| 's' | 正方形标记 |
| 'p' | 五边形标记 |
| '*' | 星标记 |
| 'h' | 六边形1标记 | 
| 'H' | 六边形2标记 |
| '+' | 十字标记 |
| 'x' | x标记 |
| 'D' | 菱形标记 |
| 'd' | 瘦菱形标记 | 
| '\|' | 垂直线标记 |
| '_' | 水平线标记 |


### 3、颜色

常用颜色可以用其的缩写词，要使用其他颜色可以指定rgb值，或者用四个元祖表示其rgba值，或者直接使用其灰度值。可以直接使用字符串(放在线型和标记之前），或者直接使用color参数

常用颜色的缩写：

| 字符 | 颜色 |
| :--- | :--- |
| 'b' | 蓝色 |
| 'g' | 绿色 |
| 'r' | 红色 |
| 'c' | 青绿色 |
| 'm' | 洋红色 |
| 'y' | 黄色 |
| 'k' | 黑色 |
| 'w' | 白色 |


## 四、刻度、标签、图例

- 通过set_xticks和set_xticklabels来调节x轴刻度及标签，需要分别传入对应的list

- 通过set_xlabel为x轴设置名称

- y轴同理

- 通过set_title设置标题

- 在添加调用ax.plot方法通过label属性添加图例，之后调用ax.legend()或plt.legend()来自动创建图例

legend的参数loc可以用来指定图例的位置：默认指定'best'就好

## 五、注解

注解可以通过text、arrow、annotate等函数进行添加：

- text可以将文本绘制在图表的指定坐标(x, y)，并且可以加上自定义的格式，如：`ax.text(x, y, 'Hello World!', family='monospace', fontsize=10)

- annotate

- 绘制图形 add_patch方法：

使用plt的各种图形的方法构造图形，再使用ax.add_patch()方法添加图形

## 六、保存图表

通过plt.savefig方法可以将当前图表保存，或者使用实例方法fig.savefig

参数如下：

| 参数 | 说明 |
| :--- | :--- |
| fname | 文件名或文件对象，图像格式由文件拓展名推断 |
| dpi | 图像的分辨率，默认为100 |
| facecolor、edgecolor | 图像的背景色，默认为白色(w) |
| format | 显示地设置文件格式('png', 'svg', 'pdf', 'ps', 'eps'等) |
| bbox_inches | 图表需要保存的部分，如果设置为tight，则去去除图表周围的空白部分 |

通过plt.rc()方法设置配色方案。

