---
layout: post
title: "机器学习九之计算学习理论"
categories: MachineLearning
tags:   datamining machineLearning computationalLearning
author: Edward
---

* content
{:toc}

计算学习理论(computational learning theory)是通过分析学习任务的困难本质，为学习算法提供理论保证，并根据分析结果指导算法设计。

--------------------

## 一、基本理论   

令h为样本集X到标签集Y的一个映射，其在一个隐含的分布上的泛化误差为：

![h泛化误差]()

h在数据集D上的经验误差为：

![h经验误差]()

定义&epsilon;表示E(h)的上限，表示预先设定的学得模型所应满足的误差要求，称为误差参数。

如果h在数据集D上的经验误差为0，则称h与D一致，否则称其和D不一致。对于任意两个映射，通过不和度(disagreement)来度量两者的差别：

![不合度]()

常用到的不等式如下：

- Jensen不等式：对于任意的凸函数f(x)，有：

![Jensen不等式]()

- Hoeffding不等式：如果x<sub>1</sub>，x<sub>2</sub>，...，x<sub>m</sub>为m个独立随机变量，且满足0<=x<sub>i</sub><=1，则对任意&epsilon;>0有：

![Hoeffding不等式]()

- McDiarmid不等式：如果x<sub>1</sub>，x<sub>2</sub>，...，x<sub>m</sub>为m个独立随机变量，且对任意1<=i<=m，函数f满足：

![McDiarmid不等式]()

## 二、PAC学习

PAC指概率近似正确(Probably Approximately Correct)，即以较大的概率学得的模型尽可能接近目标概念。

### 1、概念和概念类

c表示概念(concept)，指的是从样本空间X到标记空间Y的映射，真实标记为y。
如果对于任何样例(x,y)有c(x)=y成立，则称c为目标概念。
所有目标概念构成的集合，称为概念类(concept class)，用符号C表示。

### 2、假设和假设空间

对于学习算法&zeta;，他所考虑的所有可能的概念的集合称为假设空间(hypothesis space)，用符号H表示。
h属于H，称为假设(hypothesis)。

### 3、可分与不可分

若目标概念c属于H，则H中存在假设能将所有示例按与真实标记一致的方式完全分开，称为该问题对于学习算法&zeta;是可分的(separable)或者一致的(consistent);
若目标概念c不属于H，则H中不存在任何假设能将所有示例完全正确分开，称该问题对于学习算法&zeta;是不可分的(non-separable)或者(non-consistent)

### 4、PAC定义

- PAC辨识(PAC Identify)：

![PAC辨识]()

- PAC可学习(PAC Learnable)：

![PAC可学习]()

- PAC学习算法(PAC Learning Algorithm)：

![PAC学习算法]()

- 样本复杂度(Sample Complexity)：

![算法复杂度]()

## 三、假设空间

假设空间H有限时，称H为有限假设空间，否则为无限假设空间。

### 1、有限假设空间

- 可分情况：有限假设空间H都是PAC可学习的，所需要的样例数目为

![有限可分的样例数目要求]()

输出假设h的泛化误差随样例数目的增多而收敛于0，收敛速度为O(1/m)

- 不可分情况：样例数目较大时，h的经验误差是其泛化误差的近似。当假设空间H给定时，其中必存在一个泛化误差最小的假设。在不可分的情况下，有不可知PAC可学习(agnostic PAC learning)

![不可知PAC可学习]()

同理，在不可知可学习下，若学习算法的时间满足多项式条件，称算法为不可知PAC学习算法，满足条件的最小m称样本复杂度。

### 2、VC维

- 增长函数(growth function): 表示假设空间H对m个示例所能赋予标记的最大可能数，描述了假设空间H的表示能力

![增长函数]()

- 对分(dichotomy)和打散(shattering)：对于二分类问题，H中的假设对示例赋予标记的每种可能结果称为D的一种对分。若假设空间H能实现示例D上的所有对分，即增函数为2的m次方，称D能被假设空间H打散

- VC维： 指能被H打散的最大示例集的大小，即

![VC维]()

计算方式：若存在大小为d的数据集能被H打散，但不存在任何大小为d+1的数据集能被H打散，则VC维是d

- Sauer引理：若假设空间H的VC维为d，则对任何m有

![Sauer引理]()

若m>=d，则有

![]()

- VC维的泛化误差界：

![VC维的泛化误差界]()

即基于VC维的泛化误差界是分布无关(distribution-free)、数据独立的(data-independent)的

- 任何VC维有限的假设空间H都是不可知PAC可学习的

## 四、 Rademacher复杂度


## 五、稳定性