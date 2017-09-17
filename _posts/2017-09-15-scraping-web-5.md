---
layout: post
title:  "Python网络爬虫之Scrapy框架基础教程三"
categories: Python
tags: Python crawler Scrapy
author: Edward
---

* content
{:toc}

，详细见文档：[Scrapy英文文档](https://doc.scrapy.org/en/latest/intro/tutorial.html)




spider：定义如何去爬取一个网站

start_requests：生成请求的URL，即start_urls
parse：请求的回调方法，解析返回的响应，返回提取数据的字典，Item对象，Request对象，或者这些对象的迭代器

爬取的步骤：

定义start_requests()方法生成初始请求去


class scrapy.spiders.Spider：
其他所有的spider必须继承的类，必须提供start_requests()方法的实现，用于发送来自于start_urls属性的请求，并调用parse()方法解析响应

属性：

name：定义spider的名字，必须唯一，如果爬取的是一个单一的网站，一般以这个网站名命名

allowed_domains：包含允许请求的网站的字符串列表，如果OffsiteMiddleware设置的话，不属于这个列表内的不允许被爬取

start_urls：spider首先开始爬取的URL

custom_settings：设置信息的字典

crawler：当初始化类后，from_crawler()方法链接 Crawler对象去这个spider对象所绑定的crawler

settings：一个Setting的实例，运行spider的配置

logger：日志

方法：

from_crawler(crawler, *args, **kwargs)：



