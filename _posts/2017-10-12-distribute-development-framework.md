---
layout: post
title: "分布式框架培训"
categories: Java
tags:	java distribute framework
author: Edward
---

* content
{:toc}

前一阵子项目为了进度，也考虑到项目未来的需求，采用了集中式开发的框架。现在随着项目的深入，慢慢发觉到了项目存在的瓶颈问题(其实主要还是需求方提的要求)，于是整个系统准备大改，将要改成分布开发框架。今天下午组织人帮我们培训了一下，这里简单总结一下。

--------------------

## 一、分布式系统

### 1、CAP和BASE理论

CAP分别指Consistence一致性、 Availability可用性、NetWork partioning分区容错性。即对于一个分布式系统来说，所有的节点在同一个时间内够访问到同一份的数据副本；每次请求一个非故障的节点都能获得非错的响应(并不保证最新)，；分布式系统在遇到某节点或网络分区故障时，仍能够对外提供一致性和可用性的服务。

对于一个分布式系统来说，最多只能满足CAP中的两项：

三种方式：

- CA without P：不允许分区，则强一致性和可用性可以得到保证。但是一般情况下，分区都会存在，所以一般指的是各个子系统能够保持CA。

- CP without A：如果不要求可用性，相当于每个请求都需要在Server之间强一致，而P（分区）会导致同步时间无限延长，如此CP也是可以保证的。很多传统的数据库分布式事务都属于这种模式。

- AP wihtout C：要高可用并允许分区，则需放弃一致性。一旦分区发生，节点之间可能会失去联系，为了高可用，每个节点只能用本地数据提供服务，而这样会导致全局数据的不一致性。现在众多的NoSQL都属于此类。

BASE理论是指Basically Available(基本可用)、Soft State(软状态)、Eventual Consistency(最终一致性)。即在分布式系统出现障碍时，允许损失部分可用性，保证核心可用；允许系统存在中间状态，而该中间状态不会影响整体的可用性；所有副本经过一段时间后，最终能够达到一致的状态。

### 2、分布式和集群

这里有一个很形象的例子：小饭店原来只有一个厨师，切菜洗菜备料炒菜全干。后来客人多了，厨房一个厨师忙不过来，又请了个厨师，两个厨师都能炒一样的菜，这两个厨师的关系是集群。为了让厨师专心炒菜，把菜做到极致，又请了个配菜师负责切菜，备菜，备料，厨师和配菜师的关系是分布式，一个配菜师也忙不过来了，又请了个配菜师，两个配菜师关系是集群。

总结来说：分布式指的是把一个业务拆成多个业务，分别部署在不同的服务器上，分布式解决的是高并发的问题；而集群指的是同一个业务在多台机器上，它解决的是可用性的问题。

## 二、DUBBO

目前大部分公司采用的分布式框架是阿里的Dubbo(实际上是当当的dubbox)，它是一个rpc框架，除此之外，还有百度的bRpc，谷歌的gRpc。

dubb的架构如下图：

![Dubbo 架构](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dubbo-architecture.png)

其中分为注册中心Registry， 消费者Consumer，提供这Provider，监控中心Monitor。

- Registry是注册服务和发现服务的地方，所有的Provider需要在上面注册，以便Consumer调用

- Provider是暴露服务的服务提供方

- Consumer是调用远方服务的服务消费方

- Monitor是统计服务的调用次调和调用时间的监控中心

目前一般使用的注册中心apache的zookper。

## 三、分布式开发方式

以前我们集中式开发调用的方式一般是通过Controller调用Service层，Service调用DAO层，而在分布式开发中，由于不同的服务是相互分隔开的，而相互之间的调用是通过dubbo的服务，基本的数据流向或者调用方式是这样：在每个服务上，通过Provider暴露服务，Provider主要负责业务的逻辑，Provider来调用Service，Service来调用Dao；对于其他的服务，在zookeeper上注册Provider后，其他的服务通过Consumer来调用其所需要的Provider；而对于特殊的服务，比如门户，需要通过它的Controller来调用Manager(Service)，然后Manager来调用其Consumer，用Consumer来去调用其他的服务。