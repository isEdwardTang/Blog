---
layout: post
title:  "Python网络爬虫之开始爬虫"
categories: Python
tags: Python crawler
author: Edward
---

* content
{:toc}

主要介绍爬虫爬取网页的技巧和注意事项。





## 一、爬虫的技巧

### 1、防止重复爬取

将每次爬取的网页放在set中，每次判断将要爬取的网页不再set中才处理

### 2、递归次数

Python中，递归次数不宜太多，递归层数只允许1000层

### 3、使用随机数

每次从所有将要爬取的网页中选取下一个爬取的网页时，使用随机数可以最大限度地保证不重复。

### 4、异常

在爬取的过程中，要充分考虑异常的情况，防止过程scratch

### 5、重定向

包括服务器的重定向和客户端的重定向，对于服务器的重定向，使用Python3的urllib库可以自动解决

## 二、爬取网页的步骤

- 获得所有链接 
- 判断链接已经存在，do nothing
- 判断链接不存在，添加到set()中
- 递归不存在的连接
- 循环重复
这里的链接包括内部链接和外部链接

## 三、封装方法

方法如下：

```python

from urllib.request import urlopen
from bs4 import BeautifulSoup
import re
import datetime
import random

pages = set()
random.seed(datetime.datetime.now())

#Retrieves a list of all Internal links found on a page
def getInternalLinks(bsObj, includeUrl):
    internalLinks = []
    #Finds all links that begin with a "/"
    for link in bsObj.findAll("a", href=re.compile("^(/|.*"+includeUrl+")")):
        if link.attrs['href'] is not None:
            if link.attrs['href'] not in internalLinks:
                internalLinks.append(link.attrs['href'])
    return internalLinks

#Retrieves a list of all external links found on a page
def getExternalLinks(bsObj, excludeUrl):
    externalLinks = []
    #Finds all links that start with "http" or "www" that do
    #not contain the current URL
    for link in bsObj.findAll("a",href=re.compile("^(http|www)((?!"+excludeUrl+").)*$")):
        if link.attrs['href'] is not None:
            if link.attrs['href'] not in externalLinks:
                externalLinks.append(link.attrs['href'])
    return externalLinks

def splitAddress(address):
    addressParts = address.replace("http://", "").split("/")
return addressParts

def getRandomExternalLink(startingPage):
    html = urlopen(startingPage)
    bsObj = BeautifulSoup(html)
    externalLinks = getExternalLinks(bsObj, splitAddress(startingPage)[0])
    if len(externalLinks) == 0:
        internalLinks = getInternalLinks(startingPage)
        return getNextExternalLink(internalLinks[random.randint(0, len(internalLinks)-1)])
    else:
        return externalLinks[random.randint(0, len(externalLinks)-1)]

#Collects a list of all external URLs found on the site
allExtLinks = set()
allIntLinks = set()
def getAllExternalLinks(siteUrl):
    html = urlopen(siteUrl)
    bsObj = BeautifulSoup(html)
    internalLinks = getInternalLinks(bsObj,splitAddress(siteUrl)[0])
    externalLinks = getExternalLinks(bsObj,splitAddress(siteUrl)[0])
    for link in externalLinks:
        if link not in allExtLinks:
            allExtLinks.add(link)
            print(link)
    for link in internalLinks:
        if link not in allIntLinks:
            print("About to get link: "+link)
            allIntLinks.add(link)
            getAllExternalLinks(link)


```

## 四、使用框架

基本上所有的爬取的步骤都是：find all links on a page, evaluate the difference between
internal and external links, go to new pages，所以可以使用框架来做，最著名的是Scrapy，可惜不能支持Python3，以后整理用法
