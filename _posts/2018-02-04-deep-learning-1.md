---
layout: post
title: "深度学习"
categories: MachineLearning
tags:   datamining machineLearning conclusion
author: Edward
---

* content
{:toc}

--------------------

前向传播

反向传播

vectorization：减少for循环的使用

激活函数的使用：
sigmoid：用于二分类的输出层(0 ~ 1)
tanh：一般情况下比sigmoid效果要好(-1 ~ 1)
ReLU：一般情况下都会使用，但是在z小于0时增长率为0
leaky ReLU：有些情况下会使用，z小于0时依然有增长率

公式：

参数：W, b
超参数：学习率、迭代数、隐层数量、隐层神经元数量、激活函数的选择
