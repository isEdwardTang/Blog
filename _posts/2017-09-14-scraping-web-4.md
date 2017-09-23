---
layout: post
title:  "Python网络爬虫之Scrapy框架基础教程二"
categories: Python
tags: Python crawler Scrapy
author: Edward
---

* content
{:toc}

主要是有关Scrapy的命令和参数用法，详细见文档：[Scrapy英文文档](https://doc.scrapy.org/en/latest/intro/tutorial.html)



## 一、配置设置

scrapy.cfg配置文件的位置：
- /etc/scrapy.cfg or c:\scrapy\scrapy.cfg (system-wide),
- ~/.config/scrapy.cfg ($XDG_CONFIG_HOME) and ~/.scrapy.cfg ($HOME) for global (user-wide) settings, and
- scrapy.cfg inside a scrapy project’s root

## 二、命令行命令：

`scrapy startproject <project_name> [project_dir]`：在project_dir目录下创建Scrapy工程，没有指定project_dir则是本目录

`scrapy genspider [-t template] <name> <domain>`：在当前的spiders目录下创建一个名为name的spider，-t可以指定模板(可以使用-l查看所有的模板)，domain可以指定spider的属性，如start_urls和allowed_domains

`scrapy crawl <spider>`：使用爬虫spider进行爬取

`scrapy check [-l] <spider>`：运行contract检查

`scrapy list`：列出当前工程所有的spider

`scrapy edit <spider>`：使用环境变量或设置中的编辑器编辑spider

`scrapy fetch <url>`：输出指定url内容
- 参数：
    - --spider=SPIDER 使用指定的spider来爬取
    - --headers 输出响应头(默认输出响应正文)
    - --no-redirect 不重定向

`scrapy view <url>`：打开浏览器查看指定url
- 参数：
    - --spider=SPIDER 使用指定的spider来爬取
    - --no-redirect 不重定向

`scrapy shell [url]`：打开Scrapy shell
- 参数：
    - --spider=SPIDER 使用指定的spider来爬取
    - -c code 直接运行code命令并退出
    - --no-redirect 不重定向，默认只是此处指定的url，进入shell后将失效

`scrapy parse <url> [options]`：解析url
- 参数：
    - --spider=SPIDER 使用指定的spider来爬取
    - --a NAME=VALUE 设置spider参数
    - --callback or -c 指定用于解析响应的方法
    - --pipelines 通过pipelines处理items
    - --rules or -r 使用CrawlSpider规则去寻找回调方法去解析响应
    - --noitems 不显示被爬取的item
    - --nolinks 不显示提取的链接
    - --nocolour 不使用pygments使输出有颜色
    - --depth or -d 设置递归的层数
    - --verbose or -v 打印每一层的深度

`scrapy settings [options]`：获得Scrapy设置的值

`scrapy runspider <spider_file.py>`：直接运行某个爬虫文件，不需要创建工程

`scrapy version [-v]`：打印Scrapy的版本

`scrapy bench`：运行一个快速的benchmark测试


