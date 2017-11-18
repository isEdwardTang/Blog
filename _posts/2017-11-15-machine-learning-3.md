---
layout: post
title: "机器学习三之支持向量机"
categories: MachineLearning
tags:   datamining machineLearning svm
author: Edward
---

* content
{:toc}

这一块推理过程有点多，没怎么特别理解，稍微整理一下。

--------------------

## 一、支持向量机

### 1、基本型

如下图，分类问题的最基本思想就是基于数据集D，在样本空间中找到一个划分超平面，将不同类别的样本分开：

![分类问题](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/svm-basic-problem.JPG)

即划分平面可用：w<sup>T</sup>+b=0表示，w为法向量，决定超平面的方向，b为位移量。距离超平面最近的训练样本点使样本分类正确，称为支持向量。两个异类支持向量的超平面距离之和称为间隔：

![支持向量和间隔](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/supportvector-margin.JPG)

需要最大化间隔，即最小化w<sup>-1</sup>，加上限制条件，得出支持向量机(SVM)的基本型：

![SVM基本型](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/svm-basic-model.JPG)
 
### 2、对偶问题

计算SVM基本型的问题是一个凸二次规划问题，使用对偶问题求解，其对偶问题为：

![对偶问题1](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dual-problem-1.JPG)<br />

![对偶问题2](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/dual-problem-2.JPG)

满足KKT约束，即：

![KKT约束](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/KKT.JPG)

分析这个式子，容易知道支持向量机的一个重要性质：训练完成后，大部分的训练样本都不需要保留，最终模型仅仅与支持向量有关。

求解该问题问题，使用通用的二次规划问题求解会造成大量的开销，可以使用SMO算法(Sequential Minimal Optimization)。SMO算法的思路是：固定a<sub>i</sub>之外的所有参数，然后求a<sub>i</sub>上的极值。(因为存在约束条件，固定其中一个之外的变量，则该变量可以导出)，具体流程是：

- 选取一对需更新的变量a<sub>i</sub>和a<sub>j</sub>
- 选取变量时，尽量使所选取的两变量所对应样本之间的间隔最大，这样会给目标函数带来更大的变化
- 固定其余之外的参数，求解对偶式获得更新后的a<sub>i</sub>和a<sub>j</sub>

### 3、核函数

对于线性不可分问题，不能用之前的方法解决，，可以将原始空间映射到一个更高维的特征空间，使用在这个空间内线性可分，类似的，模型为：

![高维线性可分问题](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-model.JPG)

目标函数为：

![高维目标函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-target.JPG)

对偶问题为：

![高维对偶问题](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-dual-problem.JPG)<br />

![高维对偶问题2](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-dual-problem-2.JPG)

为了解决高维空间的内积问题，定义一个核函数：

![核函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-function.JPG)

求解核函数时，有一个定理：只要一个对称函数所对应的核矩阵半正定，则可以作为核函数使用。核函数对于支持向量机的性能至关重要，所以需要小心选择，常见的核函数如下：

![常用核函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/kernel-function-frequent.JPG)

此外，核函数的线性组合、直积，以及对于任意函数g(x)，g(x)&kappa;(x,z)g(z)等均是核函数。

## 二、软间隔和正则化

### 1、软间隔

确定一个线性可分的平面很容易造成过拟合，缓解的一个方法是允许支持向量机在部分样本处出错。优化目标可写成：

![软间隔优化目标](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/soft-margin-target.JPG)

其中C是一个常数，后面的函数是0/1损失函数，在参数小于0时为1，否则为0。但是该函数数学性质不太好，通常用一些替代损失函数来替代，常见的有：

![替代损失函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/surrogate-loss-function.JPG)<br />

![三种常见的替代损失函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/surrogate-loss-function-graph.JPG)

以hinge损失为例，目标函数为：

![hinge目标函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/hinge-target.JPG)

令后面一部分为松弛变量，则可得到软间隔支持向量机：

![软间隔支持向量机](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/soft-margin-svm.JPG)<br />

![软间隔支持向量机2](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/soft-margin-svm-2.JPG)

求出对偶问题为：

![软间隔对偶问题](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/soft-margin-dual-problem.JPG)

类似得，KTT条件为：

![软间隔KTT条件](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/soft-margin-ktt.JPG)

分析知，最终模型仅仅与支持向量有关，保持了稀疏性。

### 2、正则化

使用不同的损失函数可以得到不同的表达，一般形式为：

![优化目标一般形式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/general-target.JPG)

第一项是结构风险，用来描述f的某些性质；第二项是经验风险，用于描述模型和训练数据的契合度；C用于对两者折中。这种表达方式称为正则化。

## 三、支持向量回归

对于回归问题，假设我们能容忍&epsilon;的偏差，则支持向量回归(SVR)的基本型为：

![SVR基本型](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-basic-model.JPG)

其中C为正则化常数，l为&epsilon;-不敏感损失函数：

![不敏感损失函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-intensitive-loss.JPG)

同样，应付松弛变量，则基本型改写为：

![SVR目标函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-target.JPG)<br />

![SVR目标函数2](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-target-2.JPG)

得到对偶问题：

![SVR对偶问题](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-dual-problem.JPG)

KTT条件为：

![SVR-KTT条件](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/SVR-KTT.JPG)

## 四、sklearn使用

这里不做整理，参考网上博客：[sklearn支持向量机](http://blog.sina.com.cn/s/blog_62970c250102xg0g.html)
