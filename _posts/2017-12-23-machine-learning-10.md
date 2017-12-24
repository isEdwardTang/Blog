---
layout: post
title: "机器学习十之半监督学习"
categories: MachineLearning
tags:   datamining machineLearning 
author: Edward
---

* content
{:toc}

对于未标记样本，通过专家知识的查询来获得其标记，称为主动学习(active learning);而让学习器不依赖外界交互、自动利用未标记样本来提升学习性能，就是半监督学习(semi-supervised learning)。

--------------------

## 一、基本理论

将未标记样本的数据分布和列表标记相联系的假设，常使用聚类假设(cluster assumption)和流形假设(manifold assumption)：聚类假设假设数据存在簇结构，同一个簇的样本属于同一个类别；流形假设假设数据分布在一个流形结构上，临近的样本拥有相似的输出。

半监督学习可划分为纯半监督学习(pure)和直推学习(transductive learning)：前者假设训练数据中的未标记样本并非待预测的数据，后者假设训练数据中的未标记样本就是待预测数据。

## 二、生成式方法

生成式方法假设所有数据都是由一个潜在的模型生成的，而未标记样本可看做是模型的缺失参数，通常可使用EM算法进行极大似然求解。以高斯混合模型为例，即数据样本满足如下概率分布：

![高斯混合概率分布]()

令f(x)表示f对x的预测标记，&Theta;属于{1,...N}表示样本x隶属的高斯混合成分，D<sub>l</sub>表示有标记样本集，D<sub>u</sub>表示未标记样本集，则D<sub>l</sub>&cup;D<sub>u</sub>的对数似然为：

![生成式对数似然]()

使用EM算法求解，过程如下：

- E步：根据当前模型参数计算未标记样本属于各高斯混合成分的概率

![未标记样本高斯概率]()

- M步：基于上述概率更新模型参数，其中l<sub>i</sub>表示第i类有标记样本的数目

![生成式高斯模型参数更新]()

- 重复上述过程，直至收敛，即可获得模型参数

- 基于下式对样本进行分类：

![生成式高斯模型预测函数]()

## 三、半监督SVM

半监督SVM(S3VM)通过找到一个将两类有标记样本分开、且穿过数据低密度区域的划分超平面（SVM是找到最大间隔划分超平面）。

TSVM(Transductive Support Vector Machine)是其中的一种，学习目标如下：

![TSVM学习目标]()

过程如下：

- 使用D<sub>l</sub>训练出一个SVM<sub>l</sub>
- 用SVM<sub>l</sub>对D<sub>u</sub>中的样本进行预测，得到y<sup>^</sup>
- 初始化C<sub>u</sub>远小于C<sub>l</sub>
- 开始循环操作，知道C<sub>u</sub>和c<sub>l</sub>相等
- 求解学习目标，得到划分超平面(w,b)和松弛向量&xi;
- 对于所有未标记的样本，如果存在其中一对未标记的样本的标记指派不同，但对应的松弛变量之和大于2，需要交换两者重新求解目标函数，重新得到划分超平面(w,b)和松弛向量&xi;
- 更新C<sub>u</sub>为min{2C<sub>u</sub>，C<sub>l</sub>}

## 四、图半监督学习

基于D<sub>l</sub>&cup;D<sub>u</sub>构建一个图G=(V,E)，其中结点集合V={x<sub>1</sub>,...,x<sub>l</sub>,...,x<sub>l+u</sub>}，边集E可表示为一个亲和矩阵，用高斯函数定义：

![边集亲和矩阵]()

定义对角矩阵D=diag(d<sub>1</sub>,...,d<sub>l+u</sub>)，对角元素为：

![对角元素]()

定义一个(l+u)x|y|的非负矩阵F，其第i行元素为示例x<sub>i</sub>的标记向量

过程如下：
- 选择折图参数&sigma;和折中参数&alpha;
- 计算得到矩阵W
- 基于W构造标记传播矩阵S=D<sup>-1/2</sup>WD<sup>-1/2</sup>
- 初始化F(0):

![标记矩阵初始化]()

- 迭代F(t+1)=&alpha;SF(t)+(1-&alpha;)Y，直至收敛至F<sup>*</sup>
- 对于未标记样本，利用如下式预测标记：

![未标记样本标记预测]()


## 五、基于分歧的方法

基于分歧的方法(disaggrement-based methods)使用多学习器，协同训练(co-trainging)是此类方法的代表。

## 六、半监督聚类

根据获得的监督信息分为两种

### 1、必连(must-link)与勿连(cannot-link)约束

前者指样本必属于一个簇，后者指样本必不属于一个簇。约束k均值算法(Constrained k-means)是其中的代表，

### 2、少量有标记样本



