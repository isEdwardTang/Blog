---
layout: post
title: "Calendar的那些神坑"
categories: Java
tags:  bug Java
author: Edward
---

* content
{:toc}






Calendar算是现在java.util中关于日期比较常用的一个类了，用了几次发现这里面还有很多坑的，，，。


## 一、Calendar.MONTH

这个绝对算是一个巨大的坑了，由于思维方式的不同，我们都知道数组的下标一般都是从0开始的，没想到，月份也是，，，。当我们set或者get月份的时候，其实是实际的月份减1。

## 二、set方法

set(field, value)这个方法不仔细想清楚直接乱用还是会经常出一些莫名其妙的错误的。
比如月和时时：

- 当设置的Field为MONTH时，如果粗心没有考虑天数的话，就有问题了，比如1月31号，如果不小心设置月份为1，你会发现实际的日期变为了3月2号或3号了。内部的思维大概是这样，如果能在下个月找到这一天，那就直接设置这个Field，但是如果找不到的话，那就往后推30天，这时候月份和天数的Field可能都会变。

- 当设置的Field为HOUR时，可不要直接设置这个属性，因为Calendar默认是12小时制的，你设置HOUR为5，说不定是17时，所以还是用HOUR_OF_DAY吧。

## 三、add方法

主要还是关于月份的，这可能和set方法有点区别了，上面提到，如果直接set为某个月的话，不一定是这个月，但是add的算法又是另一套思路。add添加月份时一定能保证月份正确，比如1月31号，add了一个月，这时候实际的日期是2月底了，如果add两个月，变成3月底。它的思路是，月份直接往后推，如果在这个月能找到这一天的话，直接设置，但是如果找不到的话，那就往前推，一般就是最后一天。

## 四、月底

设置月底的方式总结了两种：

方法一：

```java
cal.set(Calendar.DAY_OF_MONTH, 1); // 设置为当月的第一天
cal.roll(Calendar.DAY_OF_MONTH, -1); // 回滚一天，也就是最后一天
```

方法二：

```java
cal.set(Calendar.DAY_OF_MONTH, cal.getActualMaximum(Calendar.DAY_OF_MONTH)); // 设置为月的最大天数
```
