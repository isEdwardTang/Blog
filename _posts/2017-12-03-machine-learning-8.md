---
layout: post
title: "机器学习八之特征选择和稀疏处理"
categories: MachineLearning
tags:   datamining machineLearning 
author: Edward
---

* content
{:toc}

特征选择指的是从特定的特征集合中选择出特征子集的过程，和降维一样，都是处理高维数据的主流技术。 主要用在特征工程的过程中。

--------------------

## 一、子集搜索和子集评价

- 子集搜索指的是从指定的特征集合中选取最相关的特征子集，方法有逐渐增加特征的前向搜索和逐渐减少特征的后向搜索以及同时搜索的双向搜索。

- 子集评价指的是计算属性子集的信息增益，来评价不同属性子集的分类的优劣。

## 二、特征选择方法

将特征子集搜索和子集评价结合，可以得到特征选择方法

### 1、过滤式选择

过滤式选择是先对数据集进行特征选择（过滤），然后再训练学习器。特征选择的过程和训练学习器无关。

Relief(Relievent Features)是一种过滤式特征选择方法，原理是：
- 使用以下相关统计量来度量特征的重要性：

![Relief相关统计量](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Relief-correlation-statistic.JPG)

其中，nh样本指的是和该样本同类的最近邻，nm是和该样本异类的最近邻，上标表示各个属性的不同取值

- 对不同样本对于各个属性的相关统计量的计算进行平均，分量值越大，该属性的分类能力就越强

- 选择比指定阈值大的相关统计量对饮的特征即可

而对于多分类问题，使用Relief-F来解决，相关统计量如下：

![Relief-F相关统计量](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Relief-F-correlation-statistic.JPG)

其中，p<sub>l</sub>指的是第l类样本在数据集中所占的比例

### 2、包裹式选择

包裹式选择直接把最终的学习器的性能作为特征子集的评价指标。

LVW(Las Vegas Wrapper)是一种包裹式选择方法，过程如下：

- 初始化特征子集为所有的特征，误差为无穷大
- 循环以下操作，直到满足退出条件
- 随机产生一个特征子集
- 使用该特征子集通过交叉验证估计学习器误差
- 如果该误差比之前的误差小，或者误差相等时特征更少时，更新特征子集

### 3、嵌入式选择

嵌入式选择将特征选择过程与学习器训练过程放在一个优化过程中进行。即在最小化损失函数的基础上，再加上一个正则项，该正则项使用L1范式时称为LASSO（Least Absolute Shrinkage and Selection Operator），使用L2范式时称为岭回归。

![LASSO](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/LASSO.JPG)<br />

![岭回归](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/ridge-regression.JPG)

L1范式和L2范式都可以降低过拟合，但是L1范式还可以更容易获得稀疏解，即特征向量存在零向量。

![L2范式得到稀疏解](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/L2-sparse.JPG)

对于L1正则化问题求解，使用近端梯度下降算法（Proximal Gradient Descent，PGD）。

## 三、字典学习

字典学习指的是学习出一个字典，可以将普通稠密表达的样本转化为合适的稀疏表达形式，使学习任务简化。字典学习最简单的形式如下：

![字典学习形式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dict-learning-model.JPG)

解法和LASSO类似，采用变量交替优化的策略，常用的有基于逐列更新策略的KSVD。

## 四、压缩感知

压缩感知指的是利用信号本身所具有的稀疏性，从部分观测样本中恢复原信号。包括感知测量和重构恢复，分别是利用傅立叶变换、小波变换、字典学习等将原始信号处理获得稀疏样本，及基于稀疏性从少量观测数据中恢复原信号。
