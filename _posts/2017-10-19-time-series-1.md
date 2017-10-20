---
layout: post
title: "数据分析之时间序列一"
categories: DataMining
tags:   python primer datamining
author: Edward
---

* content
{:toc}

在数据分析中，时间序列都是一种重要的数据形式，主要有三种形式：时间戳(timestamp)、 固定时期(period)、时间间隔(interval)。而pandas已经封装好了大数据量的对时间序列进行切片、聚合、重采样的高效方法。

--------------------

## 一、python中的时间

### 1、数据结构

python标准库中提供了表示日期和时间的数据结构，以及日历方面的功能，主要是datetime、time、calendar模块。

- datetime模块的数据类型：

| 类型 | 说明 |
| :--- | :--- | 
| date | 日期 |
| time | 时间 |
| datetime | 日期和时间 |
| timedelta | 两个datetime之间的差 |

### 2、转换

- 使用str(value)或者value.strftime(pattern)将日期类型转换为字符串类型，其中的pattern可以指定日期格式

- 使用datetime.strptime(value, pattern)可以按照指定的格式将字符串转换为日期

- 使用dateutil包中的parser.parse方法可以直接解析字符串将其转化为datetime类型

datetime的格式定义(pattern)如下：

| 代码 | 说明 |
| :--- | :--- | 
| %Y | 4位数的年 |
| %y | 2位数的年 |
| %m | 2位数的月 |
| %d | 2位数的日 |
| %H | 24小时制的时 |
| %I | 12小时制的时 | 
| %S | 秒0-61(60和61用于闰秒) |
| %w | 用整数表示的星期几(0-6,0表示星期日) |
| %U | 每年的第几周(0-53第0周指每年第一个星期日之前的几天) |
| %W | 每年的第几周(0-53第0周指每年第一个星期一之前的几天) |
| %z | 以+HHMM或-HHMM表示的UTC时区偏移量，如果时间对象为native，则返回空串 |
| %F | %Y-%m-%d的简写 |
| %D | %m/%d/%y的简写 |

不同国家可能时间表示就不一样，还有基于特定环境的格式：

| 代码 | 说明 |
| :--- | :--- |
| %a | 星期几的简写 |
| %A | 星期几的全称 |
| %b | 月份的全称 | 
| %B | 月份的全称 |
| %c | 完整的日期和时间 |
| %p | 不同环境中的AM或PM |
| %x | 适合当前环境的日期格式 |
| %X | 适合当前环境的时间环境 |

## 二、时间序列 

TimeSeries指的是索引为DatetimeIndex的Series，如果索引都是有datetime组成的，那就是一个DatetimeIndex。TimeSeries和其他的Series具有一致的功能，比如对不同索引之间的算术运算会自动按日期对齐。

### 1、索引和切片

和Series一样，对于TimeSeries对索引和数据选取的方式一致，但是更简单的方式是直接通过传入一个字符串来选取：`ts['20111011']`，甚至可以传入年或月等，选取这一段时间内的序列：`ts['2011']`。当然也可以使用
切片来操作：`ts['1/6/2017', '1/72017']`，或者使用等价的实例方法：`ts.truncate(after='', before='')`。

有些情况下，会存在一个时间点上含有多个数据，这时候对这个时间序列进行索引，可能会产生标量值或者切片，也可以使用索引的is_unique方法来判断索引是否唯一

### 2、生成日期范围

使用pandas的date_range方法可以生成一段时间范围内的DatatimeIndex，默认按天计算：

- 指定两个时间段的日期：

```python
pd.date_range('10/1/2017', '10/20/2017')
"""
DatetimeIndex(['2017-10-01', '2017-10-02', '2017-10-03', '2017-10-04',
               '2017-10-05', '2017-10-06', '2017-10-07', '2017-10-08',
               '2017-10-09', '2017-10-10', '2017-10-11', '2017-10-12',
               '2017-10-13', '2017-10-14', '2017-10-15', '2017-10-16',
               '2017-10-17', '2017-10-18', '2017-10-19', '2017-10-20'],
              dtype='datetime64[ns]', freq='D')
"""
```

- 指定开始时间和periods，或者结束时间和periods可以生成指定长度的日期：`pd.date_range(start='1/1/2017', period=20)`

- 可以指定freq参数，可以选取时间间隔内的满足频率要求的日期：`pd.date_range('1/1/2017', '5/1/2017', freq='BM')`。关于具体的频率参数的含义，如下：

| 别名 | 偏移量类型 | 说明 |
| :--- | :--- | :--- |
| D | Day | 每日 |
| B | BusinessDay | 每工作日 |
| H | Hour | 每时 |
| T或min | Minute | 每分 |
| S | Second | 每秒 |
| L或ms | Milli | 每毫秒 |
| U | Micro | 每微妙 |
| M | MonthEnd | 每月最后一天 |
| BM | BusinessMonthEnd | 每月最后一个工作日 |
| MS | MonthBegin | 每月第一天 |
| BMS | BusinessMonthBegin | 每月第一个工作日 |
| W-MON、W-TUE··· | Week | 每周，从指定的星期几算起 |
| WOM-1MON、WOM-3FRI··· | WeekOfMonth | 每月第几周的星期几 |
| Q-JAN、Q-FEB··· |  QuarterEnd | 以指定月份结束的年度中每个季度最后一个月最后一天 |
| BQ-JAN、BQ-FEB··· |  BusinessQuarterEnd | 以指定月份结束的年度中每个季度最后一个月最后一个工作日 |
| QS-JAN、QS-FEB··· | QuarterBegin | 以指定月份结束的年度中每个季度最后一个月第一天 |
| BQS-JAN、BQS-FEB··· | BusinessQuarterBegin | 以指定月份结束的年度中每个季度最后一个月第一个工作日 |
| A-JAN、A-FEB··· | YearEnd | 每年指定月份的最后一天 |
| BA-JAN、BA-FEB··· | BusinessYearEnd | 每年指定月份的最后一个工作日 |
| AS-JAN、AS-FEB··· | YearBegin | 每年指定月份的第一天 |
| BAS-JAN、BAS-FEB··· | BusinessYearBegin | 每年指定月份的第一个工作日 |

同时，频率也可以和数字混合使用，比如：`4H`；各个不同的频率也可以叠加使用，比如：`4H25T`

- 指定normalize参数为True即可规范化时间戳，即时间都是00:00:00

### 3、移动数据

Series和DataFrame都有一个shift方法，可以保持索引不变，对数据进行前移或后移

## 三、时区处理
