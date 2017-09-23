---
layout: post
title: "初识深度学习"
categories: DeepLearning
tags:   DeepLearning primer
author: Edward
---

* content
{:toc}

主要从李宏毅教授的PPT中整理得出，具体参考：[一天搞懂深度學習](https://link.zhihu.com/?target=http%3A//www.slideshare.net/tw_dsconf/ss-62245351%3Fqid%3D108adce3-2c3d-4758-a830-95d0a57e46bc%26v%3D%26b%3D%26from_search%3D3)





## 一、Deep Learning介绍

### 1、Machine Learning

机器学习就是找到一个最优的函数，能够得到预期的结果。

### 2、深度学习步骤

- step1: define a set of function(通过Netural Network)

- step2: goodness of function

- step3: pick up the best function

### 3、Netural Network

- 神经元(Neuron)：z = a^1w^1 + ... + a^kw^k + ... + a^nw^n + b,
其中w^i为weight，b为bias

- Action Function:

- Sigmoid Function：

- Fully Connect Feedforward Network：包括Input Layer、Hidden Layers、Output Layer

- Tril and Error + Intuition

- Loss: distance between the network output and target，找到最小的Total Loss

### 4、如何知道最优函数

梯度减小(Gradient Descent):

network parameters = {w1, w2, ..., b1, b2, ...}

- 为w选择初始值

- 计算Total Loss和w的导数，负数，增加w，正数，减小w
增加减小的值为learning rate 乘以导数

- 重复，直到导数足够小

- 注意，Gradient descent never guarantee global minima










