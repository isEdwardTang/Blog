---
layout: post
title: "机器学习之一决策树"
categories: MachineLearning
tags:   datamining machineLearning decisionTree
author: Edward
---

* content
{:toc}

从最简单和常见的决策树开始学习机器学习！

--------------------

## 一、决策树基本概念

### 1、基本流程

- 使用递归，递归返回的条件：
    - 当前结点为空，或当前结点包含的样本全属于同一个类别
    - 当前属性集为空，或所有样本在所有属性取值相同
- 每次从属性集中选择最优的划分属性
- 对于该属性的每一个取值，生成一个分支

### 2、划分属性

- 信息熵Ent(D)：描述样本集合D的纯度，Ent越小，纯度越高
![Ent(D)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Ent.JPG)

- 信息增益Gain(D,a)：使用属性a来划分D的纯度的提升，Gain越大，则使用属性a划分纯度越高
    - 对于取值数目多的属性有偏好
![Gain(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gain.JPG)

- 增益率Gain_ratio(D,a)：信息增益和属性a的个数的商
    - 对于取值数目较少的有偏好，一般选择信息增益高于平均水平的属性，再选择其中增益率最高的
![Gain_ratio(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gain_ratio.JPG)
![IV](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/IV.JPG)

- 基尼值Gini(D)：反映从数据集D中随机选取两个样本，其类别不一致的概率，Gini越小，纯度越高
![Gini(D)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gini.JPG)

- 基尼指数Gini_index(D,a)：以属性a划分后的数据集的基尼值加权之和，基尼指数越小，选择a属性划分越好
![Gini_index(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gini_index.JPG)

## 二、剪枝

降低过拟合，基本策略有预剪枝和后剪枝

### 1、预剪枝

对每一个结点在划分前进行估计，如果当前划分不能带来决策树泛化能力的提升，则停止划分并将该结点标记为叶结点

- 决策树的很多分支没有展开，降低了过拟合的风险，减少了训练时间和测试时间开销
- 某些划分虽不能提高当前的泛化性能，但后续可能会导致性能的提高，因此预剪枝禁止划分它们可能会导致欠拟合

### 2、后剪枝

先生成一个完整的决策树，然后自底向上，对于非叶子结点，如果将其子树替换成叶结点能带来决策树泛化能力的提升，则将该子树替换为叶结点

- 保留了更多的分支，欠拟合风险小，泛化能力优于预剪枝
- 需要在完全生成决策树之后，自底向上对所有非叶子结点考察，训练的时间开销大

## 三、连续属性和缺失值处理

### 1、连续属性

采用二分法处理，即取连续属性在样本中相邻属性值（从小到大排序）的平均值作为候选划分点，

然后就采用和离散属性相同的方法指标进行划分属性

- 当使用连续属性划分时，该属性依然可以作为后代属性的划分标准

### 2、缺失值处理

下面三个定义量分别表示：无缺失值样本所占的比例，无缺失值样本中第k类所占的比例，无缺失值样本中在属性a上取各个值的样本所占的比例：

![缺失值公式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/loss_value.JPG)

则可以推广信息增益：

![缺失值信息增益](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/loss_gain.JPG)

![缺失值熵](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/loss_ent.JPG)

## 四、多变量决策树

单变量决策树的分类边界的每一段都是与坐标轴平行，而多变量决策树的边界不是单个属性，而是多个属性的线性组合。

## 五、常见算法

### 1、ID3

每次选择的属性都是Gain最大的

### 2、C4.5

选择最大的Gain_radio的属性来进行选择结点，同时可以处理连续型和缺失值

### 3、CART

每次都选择当前数据集中具有最小Gini_radio的属性作为结点划分决策树，对于连续属性，采用和C4.5相同的方法，未避免过拟合，会采用剪枝

## 六、sklearn包



