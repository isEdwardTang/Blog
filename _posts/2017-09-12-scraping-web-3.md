---
layout: post
title:  "Python网络爬虫之Scrapy框架基础教程一"
categories: Python
tags: Python crawler Scrapy
author: Edward
---

* content
{:toc}

参考Scrapy1.4教程整理，详细见文档：[Scrapy英文文档](https://doc.scrapy.org/en/latest/intro/tutorial.html)




## 一、Scrapy结构

- 首先安装Scrapy的库，选择1.4的版本已经支持python3了，但是如果是在windows上安装会出现很多的问题，详细去谷歌相应的解决方案（windows就是个坑）。

- 安装完之后配置Scrapy的环境变量，这样可以在shell或cmd中直接使用Scrapy的命令。

- 在某个目录下使用命令`scrapy startproject 工程名称(比如tutorial)`构建Scrapy的框架目录。

scrapy框架的目录如下：

```python
tutorial/
    scrapy.cfg            # deploy configuration file

    tutorial/             # project's Python module, you'll import your code from here
        __init__.py

        items.py          # project items definition file

        pipelines.py      # project pipelines file

        settings.py       # project settings file

        spiders/          # a directory where you'll later put your spiders
            __init__.py
```

## 二、spiders

在spiders包下放置具体的“爬虫”(spider),spider需要继承`scrapy.spiders`，其属性和方法介绍如下：
- name属性：唯一标识spider，也是运行爬虫时的name参数
- start_requests()方法：返回请求的迭代器或一个list
- parse(response)方法：处理响应，response是一个TextResponse的实例，保存了page的内容和相应的方法
- 如果不实现start_requests()方法，可以定义一个start_urls，包含需要请求的url

使用`scrapy crawl 爬虫name`来运行爬虫

## 三、Scrapy Shell

使用`scrapy shell "url"`：打开Scrapy的shell，可以使用选择器筛选相应URL的内容

筛选的方法如下：
- response.css()：使用选择器提取，返回list
- response.css().extract()：提取内容，返回list
- response.css().extract_first()
- response.css().re()：使用正则
- response.xpath()：使用xpath表达式

## 四、yield

在parse中通过yeild中返回提取的数据构成的字典：

```python
def parse(self, response):
    for quote in response.css('div.quote'):
        yield {
            'text': quote.css('span.text::text').extract_first(),
            'author': quote.css('small.author::text').extract_first(),
            'tags': quote.css('div.tags a.tag::text').extract(),
        }
```

## 五、保存为json

保存为json数据的命令：

- scrapy crawl spiderName -o spiderName.json 保存为json
- scrapy crawl spiderName -o spiderName.jl 保存为json Line

## 六、添加链接

使用urljoin构建绝对URL：

```python
def parse(self, response):
    for quote in response.css('div.quote'):
        yield {
            'text': quote.css('span.text::text').extract_first(),
            'author': quote.css('small.author::text').extract_first(),
            'tags': quote.css('div.tags a.tag::text').extract(),
        }

    next_page = response.css('li.next a::attr(href)').extract_first()
    if next_page is not None:
        next_page = response.urljoin(next_page)
        yield scrapy.Request(next_page, callback=self.parse)
```

使用response.follow()可以直接使用相对的url，并可以返回request:

```python
def parse(self, response):
    for quote in response.css('div.quote'):
        yield {
            'text': quote.css('span.text::text').extract_first(),
            'author': quote.css('span small::text').extract_first(),
            'tags': quote.css('div.tags a.tag::text').extract(),
        }

    next_page = response.css('li.next a::attr(href)').extract_first()
    if next_page is not None:
        yield response.follow(next_page, callback=self.parse)
```

follow()除了可以接受一个string，还可以接受一个链接：

```python
for href in response.css('li.next a::attr(href)'):
    yield response.follow(href, callback=self.parse)
```

默认Scrapy不会访问同样的路径

## 七、传参数

使用`scrapy crawl quotes -o quotes-humor.json -a tag=humor`传参数

这里的tag是参数：

通过`tag = getattr(self, 'tag', None)`获取