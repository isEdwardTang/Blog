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
![Ent(D)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Ent.jpg)

- 信息增益Gain(D,a)：使用属性a来划分D的纯度的提升，Gain越大，则使用属性a划分纯度越高
    - 对于取值数目多的属性有偏好
![Gain(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gain.jpg)

- 增益率Gain_ratio(D,a)：信息增益和属性a的个数的商
    - 对于取值数目较少的有偏好，一般选择信息增益高于平均水平的属性，再选择其中增益率最高的
![Gain_ratio(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gain_ratio.jpg)
![IV](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/IV.jpg)

- 基尼值Gini(D)：反映从数据集D中随机选取两个样本，其类别不一致的概率，Gini越小，纯度越高
![Gini(D)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gini.jpg)

- 基尼指数Gini_index(D,a)：以属性a划分后的数据集的基尼值加权之和，基尼指数越小，选择a属性划分越好
![Gini_index(D,a)](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gini_index.jpg)

## 二、剪枝

降低过拟合，基本策略有预剪枝和后剪枝

### 1、预剪枝

### 2、后剪枝

## 三、连续属性和缺失值处理

### 1、连续属性

### 2、缺失值处理

## 四、多变量决策树

## 五、常见算法

### 1、ID3

### 2、C4.5

### 3、CART

### 4、OC1

