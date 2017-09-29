---
layout: post
title:  "Python网络爬之使用BeautifulSoup"
categories: Python
tags: Python crawler
author: Edward
---

* content
{:toc}

这是我读《Web Scraping with Python》这本书中总结而来。从网络爬取我们所需要的东西是一件非常有意思的，让我们一步步开始吧！而掌握爬虫的基础是解析html文档，这里需要掌握BS这个库。





## 一、BeautifulSoup对象

直接使用BeautifulSoup的构造器获得对象：

```python
html = urlopen("http://www.pythonscraping.com/pages/page3.html")
bsObj = BeautifulSoup(html)
```

使用bsObj.tag获得相应的Tag Object：

```python
tags = bsObj.h1
```

使用get_text()获得标签的内容NavigableString

还有Comment对象，标志注释

## 二、find和findAll

find和findAll使用基本相同，只是find之后查到满足条件的第一个tag，而findAll返回一个tag列表：

- findAll(tag, attributes, recursive, text, limit, keywords)
- find(tag, attributes, recursive, text, keywords)

各个参数解释如下：

- tag: string 或者 list,比如"h1"或者{"h1", "h2", ...}
- attributes: dictinary, 比如{{"class":"green", "class":"red"}}
- recursive: boolean，findall默认是True，会循环递归dom树
- text: string，匹配标签内容
- limit：findall的limit值为1时，等同于find
- keyword: 使用特定属性，如bsObj.findAll(id="text")
    注意，不可以使用class，替代方法是bsObj.findAll(class_="green")
    或者使用attribute：bsObj.findAll("", {"class":"green"}

## 三、遍历Dom

使用如下属相获取tag标签的相应文档树上的其他标签：

- children
- descendants
- next_siblings and previous_siblings
- next_sibling and previous_sibling
- parent and parents

## 四、正则

在find和findAll的字符串中，可以使用Regular Expressions正在快速爬取所需内容，Python中的常用正则符号如下：

Commonly used regular expression symbols

|符号 | 解释|
|:--: | :--|
\* | 匹配之前的字符或表达式0到多次
\+ | 匹配之前的字符或表达式0或1次
[] | 匹配其中的某一个字符
() | 分组的子表达式
{m, n} | 匹配之前的字符或表达式m到n次
[^] | 匹配不在其中的字符
&#124; | 匹配左边或右边的字符或表达式
. | 匹配任意字符
^ | 从头开始匹配
\ | 转义
$ | 匹配最后的字符
?! | 不包含后面的字符


## 五、其他

活动标签的属性：

- myTag.attrs 获得所有的属性的list
- myImgTag.attrs['src'] 获得相应的属性值

使用lambda：

findall接受函数参数，其函数必须接收一个tag类型的参数，必须返回boolean
如：soup.findAll(lambda tag: len(tag.attrs) == 2)