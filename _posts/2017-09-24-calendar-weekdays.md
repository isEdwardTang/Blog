---
layout: post
title:  "Calendar之根据当前日期获取本周各个日期"
categories: Java
tags: Java 
author: Edward
---

* content
{:toc}

Java关于日期的一个小技巧。




## 一、Calendar之根据当前日期获取本周各个日期

代码如下：

```java
Calendar cal = Calendar.getInstance();  
// 判断要计算的日期是否是周日，如果是则减一天计算周六的，否则会出问题，计算到下一周去了
int dayWeek = cal.get(Calendar.DAY_OF_WEEK);// 获得当前日期是一个星期的第几天
if (1 == dayWeek) {  
    cal.add(Calendar.DAY_OF_MONTH, -1);  
}
// 设置一个星期的第一天，按中国的习惯一个星期的第一天是星期一  
cal.setFirstDayOfWeek(Calendar.MONDAY);  
// 获得当前日期是一个星期的第几天  
int day = cal.get(Calendar.DAY_OF_WEEK);  
// 根据日历的规则，给当前日期减去星期几与一个星期第一天的差值  
cal.add(Calendar.DATE, cal.getFirstDayOfWeek() - day + i - 1); // 星期i的日期
```