---
layout: post
title: 爬取boss直聘岗位"
categories: 
tags:   datamining
author: Edward
---

* content
{:toc}

想看看一下当下数据挖掘的工作需要掌握的能力，所以用scrapy写了一个小爬虫爬取boss直聘上有关数据挖掘的有关岗位的要求。

--------------------

## 一、搭建环境

使用scrapy的方法这里这就多说了，pip一下就ok了，如果是windows下可能麻烦一点，再在工作空间下使用：`scrapy startproject boss_zhipin`，目录结构如下：

![scrapy结构](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/scrapy_structure.JPG)

其中，
- spider文件夹存放的是具有的爬虫实现的文件夹
- items.py是我们需要爬取的内容的实体类
- middlewares.py是关于IP代理和user_agent的类
- settings.py是全局的配置文件

话不多说，开干！

## 二、书写爬虫

### 1、items

这次爬虫我主要爬取的内容很简单，就是关于数据挖掘的工作岗位的要求，顺便把工作职位和公司名称也捞一下，items只有这三个：

```python
class BossZhipinItem(scrapy.Item):
    # define the fields for your item here like:
    # name = scrapy.Field()
    job_name = scrapy.Field()
    job_company = scrapy.Field()
    job_content = scrapy.Field()
```

### 2、spider

boss直聘上关于数据挖掘的搜索页的URL是：https://www.zhipin.com/c101010100/h_101010100/?query=数据挖掘&page=xx&ka=page-xx，再深入研究一下每一页的页面，可以发现其中的我们需要页面的格式。这里我使用的是xpath而不是是css结合正则，因为相比而言，xpath可能更方便一点，详细的关于xpath的说明请参考：[xpath常用方法](http://www.xoxxoo.com/article/show/i/379.html)。不多说，直接贴代码：

```python
class ZhipinSpider(Spider):
    name = 'zhipin'
    allowed_domains = ['www.zhipin.com']    # 一定不要加协议
    start_urls = [u"https://www.zhipin.com/c101010100/h_101010100/?query=数据挖掘&page="
                  + str(i) + "&ka=page-" + str(i) for i in range(1, 21)]

    def parse(self, response):
        url_list = response.xpath('//div[@class="job-primary"]/div/h3/a/@href').extract()
        for link in url_list:
            try:
                url = "https://" + self.allowed_domains[0] + link
                yield Request(url=url, callback=self.parse_detail)
            except Exception:
                continue

    def parse_detail(self, response):
        item = BossZhipinItem()
        item['job_name'] = response.xpath('//div[@class="info-primary"]/div[@class="name"]/text()').extract_first()
        item['job_company'] = response.xpath('//div[@class="info-company"]/h3/a/text()').extract_first()
        item['job_content'] = "".join(response.xpath('//div[@class="job-sec"]/div[1]//text()').extract())
        yield item
```

这里有几个注意点：

- allowed_domains不要加协议，而爬取时参数要加
- xpath方法返回的是一个对象，使用extract获得内容的列表

## 三、保存

这里内容没有很复杂，直接保存在本地文件即可。在 piplines中写保存的类方法：

```python
class BossZhipinPipeline(object):

    def __init__(self):
        self.file = open('job.txt', 'w+')

    def process_item(self, item, spider):
        try:
            self.file.write("-------" + item['job_name'] + ":" + item['job_company'] + "---------\n" + item['job_content'] + "\n\n")
        except Exception:
            pass
        return item

    def close_spider(self, spider):
        self.file.close()
```

简单解释一下：

- __init__方法是在spider开启就会执行
- process_item方法在我们在spider中返回一个item时执行
- close_spider在spider最终关闭执行

还要在settings.py中开启，最好为了防止乱码，限定item的编码：

```python
FEED_EXPORT_ENCODING = 'utf-8'
ITEM_PIPELINES = {
   'boss_zhipin.pipelines.BossZhipinPipeline': 300,
}
```

## 四、对付防爬

很多网站设置了防爬策略，boss直聘也会，如果请求过多，在24小时内就不能再被访问，返回403，我也调到这个坑里面去了，搜了一下对付防爬的策略，大致一下几种：

- 设置请求等待时间：在settings.py中设置download_delay，虽然爬取的时间会被延长，但是会减少被ban的几率

```python
DOWNLOAD_DELAY = 3
```

- 禁用cookie：这里不用说了吧

```python
COOKIES_ENABLED = False
```

- 使用user agent池：编写自己的UserAgentMiddle中间件，每次发送请求时随机选择一个user-agent：

```python
class RotateUserAgentMiddleware(UserAgentMiddleware):
    def __init__(self, user_agent=''):
        self.user_agent = user_agent

    def process_request(self, request, spider):
        ua = random.choice(self.user_agent_list)
        if ua:
            request.headers.setdefault('User-Agent', ua)
    # the default user_agent_list composes chrome,IE,firefox,Mozilla,opera,netscape
    # for more user agent strings,you can find it in
    # http://www.useragentstring.com/pages/useragentstring.php

    user_agent_list = [
        "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/22.0.1207.1 Safari/537.1",
        "Mozilla/5.0 (X11; CrOS i686 2268.111.0) AppleWebKit/536.11 (KHTML, like Gecko) Chrome/20.0.1132.57 Safari/536.11",
        "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/536.6 (KHTML, like Gecko) Chrome/20.0.1092.0 Safari/536.6",
        "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/536.6 (KHTML, like Gecko) Chrome/20.0.1090.0 Safari/536.6",
        "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.1 (KHTML, like Gecko) Chrome/19.77.34.5 Safari/537.1",
        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/536.5 (KHTML, like Gecko) Chrome/19.0.1084.9 Safari/536.5",
        "Mozilla/5.0 (Windows NT 6.0) AppleWebKit/536.5 (KHTML, like Gecko) Chrome/19.0.1084.36 Safari/536.5",
        "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1063.0 Safari/536.3",
        "Mozilla/5.0 (Windows NT 5.1) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1063.0 Safari/536.3",
        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_0) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1063.0 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1062.0 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1062.0 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1061.1 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1061.1 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1061.1 Safari/536.3",
        "Mozilla/5.0 (Windows NT 6.2) AppleWebKit/536.3 (KHTML, like Gecko) Chrome/19.0.1061.0 Safari/536.3",
        "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/535.24 (KHTML, like Gecko) Chrome/19.0.1055.1 Safari/535.24",
        "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/535.24 (KHTML, like Gecko) Chrome/19.0.1055.1 Safari/535.24"
       ]
```

还要在settings.py中启用：

```python
DOWNLOADER_MIDDLEWARES = {
    'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
    'boss_zhipin.rotate_useragent.RotateUserAgentMiddleware': 400,
    ...
}
```

- 使用IP池：使用其他的ip进行代理访问，网站可以找到大量的透明IP，贴网址：[代理IP](http://www.xicidaili.com/nt/)，策略和user-agent类似，也是发送请求时随机选取一个ip进行访问：

```python
class ProxyMiddleware(object):

    # overwrite process request
    def process_request(self, request, spider):
        # Set the location of the proxy
        proxy = random.choice(self.PROXIES)
        if proxy['user_pass'] is not None:
            request.meta['proxy'] = "http://%s" % proxy['ip_port']
            encoded_user_pass = proxy['user_pass']
            request.headers['Proxy-Authorization'] = 'Basic ' + encoded_user_pass
            print("**************ProxyMiddleware have pass************" + proxy['ip_port'])
        else:
            print("**************ProxyMiddleware no pass************" + proxy['ip_port'])
            request.meta['proxy'] = "http://%s" % proxy['ip_port']

    PROXIES = [
        {'ip_port': '27.205.95.106:9999', 'user_pass': ''},
        {'ip_port': '122.72.18.35:80', 'user_pass': ''},
        {'ip_port': '61.155.164.109:3128', 'user_pass': ''},
        {'ip_port': '115.212.97.241:9999', 'user_pass': ''},
        {'ip_port': '183.15.27.96:9999', 'user_pass': ''},
        {'ip_port': '49.117.167.47:9999', 'user_pass': ''},
    ]
```

同样要设置启动：

```python
DOWNLOADER_MIDDLEWARES = {
    ...
    "scrapy.downloadermiddlewares.httpproxy.HttpProxyMiddleware": 110,
    'boss_zhipin.rotate_useragent.ProxyMiddleware': 100,
}
```

## 五、结果

大功告成，在项目目录下使用命令：`scrapy crawl boss_zhipin`，爬取一段时间，爬取到的部分内容如下：

```txt
-------数据挖掘工程师 :京东商城---------

                            岗位职责：1、通过深度数据挖掘，产出数据分析报告，指导业绩及产品改进；2、针对用户、流量、销售等专题，进行深入研究，发现问题并给出改进建议和计划；3、负责搜索推荐等产品的策略实现和优化。任职要求：1、计算机、统计、数学等相关专业，本科以上学历；2、1-3年数据分析或数据挖掘经验，有推荐算法经验者优先；3、熟练使用Python、R等数据分析工具，熟悉各种算法的应用场景；4、具备较强的抗压能力及自主学习能力，敢于面对挑战。
                            海阔凭鱼跃，天高任鸟飞
                                亦庄科创十一街京东总部
                                
                            

-------数据挖掘 :京东商城---------

                            职位描述：1、参与京东智慧供应链优化选品模型搭建和具体问题解决方案的设计工作；2、负责对品类划分、替代性、决策树等对供应商商品进行建模、模型优化和提升；3、负责利用数据挖掘、机器学习相关算法，对零售供应链相关各环节进行分析；4、负责跟进供应链优化、选品优化、机器学习、数据挖据等，并实际运用到产品系统中；任职要求：1、硕士或以上学历，计算机、数理统计、运筹学、机器学习等相关专业；2、至少1-3年及以上海量数据挖掘和数据分析经验，能独立构建模型，提供相应算法；3、熟练编程，具有独立实现算法和调优的经验，对数据敏感，具有良好的逻辑思维能力；4、有供应链商品优化领域经验优先，有基于运筹学的最优化经验者优先。5、熟悉R、Python等编程语言（至少会一种），熟练Hadoop,spark,R,Hive等大数据处理工具。6、优秀的团队合作精神、诚实、勤奋、严谨。
                            
                                北京大兴区科创十一街与经海一路交叉口
                                
                            

-------机器学习/数据挖掘工程师 :小灵花科技---------

                            工作职责：1、应用机器学习、数据挖掘等技术，对海量数据进行挖掘，发现其潜在关系，指导业务发展； 2、深化用户分类，用户属性挖掘以及用户体系建设；3、能够进行数据建模和预测分析，需求数据层面的价值任职资格：1、具有机器学习/数据挖掘/信息检索/自然语言处理/文本分类与聚类/统计数学等任一领域相关的理论背景：2、对数据结构和算法设计有较为深刻的理解；3、精通一门或多门开发语言（C++、Python和Java等）；4、熟练掌握一种数据库，例如MySQL，精通SQL语言，并有实际应用和开发经验。具备以下条件者优先1、有Hadoop、Hive、Hbase、spark、storm、elasticsearch等海量数据研发经验优先；2、有用户行为、兴趣建模、用户画像等相关经验者优先；3、有个人技术博客或活跃在各技术社区。
                            北京小灵花信息技术有限公司成立于2017年，是一家由前央企高管团队组建的智能大数据风控科技公司，在金融，计算机应用，传媒等多个领域有着强大的技术资源及行业资源。现已获得上市公司千万级天使轮融资，并受到多家央企跟上市公司的融资关注。
                                北京市 海淀区 天创科技大厦 2层208
```