---
layout: post
title: "机器学习六之聚类"
categories: MachineLearning
tags:   datamining machineLearning clustering
author: Edward
---

* content
{:toc}

聚类任务是指在无监督学习中，通过对无标记的训练样本学习来将其划分为若干个通常是不相交的子集，即簇(cluster)，每个簇都可能对应一些潜在的概念(类别)。

--------------------

## 一、聚类度量

### 1、性能度量

聚类效果好要求簇内相似度高且簇间相似度低。聚类性能度量有两类，外部指标和内部指标，外部指标表示将聚类结果和某个参考模型进行比较，内部指标直接考察聚类结果。

a表示集合包含在聚类划分的簇，也包含参考模型的簇的样本对，b表示包含在聚类划分的簇，不包含参考模型的簇的样本对，c表示不在聚类划分的簇，包含在参考模型的簇的样本对，d表示都不包含。则定义一些性能度量外部指标有以下：

- Jaccard参数(Jaccard Cofficient，简称JC):

![Jaccard参数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Jaccard-Coefficient.JPG)

- FM指数(Fowlkes and Mallows Index，简称FMI):

![FM指数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Fowlkes-and-Mallows-Index.JPG)

- Rand指数(Rand Index，简称RI):

![Rand指数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Rand-Index.JPG)

上述结果在[0,1]区间，值越大越好。

c表示簇的划分，定义如下式子：dist表示两个样本之间的距离，&mu;表示簇C的中心点。则avg表示簇C内样本的平均距离，diam对应簇C内样本减的最远距离，dmin表示两个簇之间最近样本的距离，dcen表示两个簇中心点间的距离。

![聚类簇划分公式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/clustering-divide-function.JPG)

基于这些公式，导出常用的性能度量内部指标有以下：

- DB指数(Davies-Bouldin Index，简称DBI)：

![DB指数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Davies-Bouldin-Index.JPG)

- Dunn指数(Dunn Index，简称DI)：

![DI指数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Dunn-Index.JPG)

### 2、距离度量

- 距离度量的性质：非负性、对称性、直递性(三角不等式)。

- 对于有序距离，常用闵可夫斯基距离：

![闵可夫斯基距离](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Minkowski-distance.JPG)

当p趋于无穷时得到切比雪夫距离，当p=2时得到欧式距离，p=1时得到曼哈顿距离。

- 对于无序距离，可采用VDM距离：

![VDM距离](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/VDM-distance.JPG)

- 常使用闵可夫斯基距离和VDM距离结合处理混合属性：

![混合属性距离](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/mixing-distance.JPG)

- 对于样本空间中不同属性的重要性不同时，可使用加权距离

## 二、原型聚类算法

原型聚类算法先对原型初始化，然后对原型进行迭代更新求解。

### 1、k均值算法(k-means)

k均值算法对于给定的簇C={C<sub>1</sub>,C<sub>2</sub>,C<sub>k</sub>}，最小化均方误差：

![k均值均方误差](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/k-means-error.JPG)<br />

![k均值均值向量](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/k-means-vector.JPG)

E越小簇内相似度越高，但最小化E一般不可取，所以采用贪心策略迭代求解，过程如下：
- 从数据集D中随机选择k个样本作为初始化均值向量
- 分别计算每一个样本与各均值向量的距离
- 根据距离最近的均值向量确定该样本的簇标记
- 将该样本划分到相应的簇
- 分别对于每一个均值向量，计算新的均值向量:
![均值向量更新公式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/k-means-vector-update.JPG)
- 如果和之前的均值向量不用，则更新该均值向量
- 直到所有的均值向量不变时结束

### 2、学习向量量化(LVQ)

LVQ(Learning Vector Quantization)假设数据样本带有类别标记，利用样本的监督信息来辅助聚类。过程如下：
- 初始化一组原型向量
- 从样本集D随机选取样本
- 计算样本与每一个原型向量的距离
- 找出与该样本距离最近的原型向量
- 判断该样本的标记是否与原型向量的类别标记一致
- 一致和不一致分别按照如下公式更新该原型向量：
![原型向量更新公式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/model-vector-update.JPG)
- 循环迭代，知道满足条件

### 3、高斯混合聚类

高斯混合聚类(Mixture-of-Gaussian)通过概率模型来表达聚类原型。对于随机向量x，服从高斯分布时的概率密度函数如下：

![高斯分布概率密度函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Gaussian-Probability-Density-Function.JPG)

其完全由均值向量&mu;和协方差矩阵&Sigma;确定，记为p(x|&mu;,&Sigma;)，则定义高斯混合分布：

![高斯混合分布](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Mixture-of-Gaussian-Function.JPG)

记&gamma;<sub>ji</sub>表示样本x<sub>i</sub>由第i个高斯混合成分生成的概率，

![高斯混合成分后验概率](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Mixture-of-Gaussian-after-probility.JPG)

则每个样本的簇标记即是最大化这个值的高斯混合成分。详细过程如下：

- 初始化高斯混合分布的模型参数{(&alpha;<sub>i</sub>,&mu;<sub>i</sub>,&Sigma;<sub>i</sub>)}
- 分别计算各样本由各混合成分生成的后验概率
- 对于每一个高斯混合成分，用如下式更新模型参数：

![高斯混合分布新参数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Mixture-of-Gaussian-update-param.JPG)

- 迭代直到满足终止条件
- 对于每一个样本，分别根据如下式确定该样本的簇标记，并将该样本划到相应的簇：

![高斯混合分布簇标记](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Mixture-of-Gaussia-Label.JPG)

## 三、密度聚类

密度聚类(density-based clustering)假设聚类结构能通过样本分布的紧密程度确定，从样本密度的角度考察样本之间的可连接性，并基于可连接样本不断拓展聚类簇以获得最终的聚类结果。

常用的有DBSCAN算法(Density-Based Spatial Clustering of Applications wiht Noise)，基于邻域参数来刻画样本分布的紧密程度。对于数据集D={x<sub>1</sub>,x<sub>2</sub>,...x<sub>m</sub>}，有如下概念：

![密度聚类有关概念](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/density-based-clustering-concept.JPG)

则基于以上概念，定义簇为由密度可达关系导出的最大的密度相连样本集合。算法过程如下：

- 初始化核心对象集合&Omega;
- 对于每一个样本x<sub>j</sub>，确定其&epsilon;-领域，如果该样本的&epsilon;-领域大于等于指定的Minpts，则将其加入到核心对象集合中&Omega;去
- 初始化聚类簇数k=0，以及未访问的样本集合&Gamma;
- 迭代如下过程
- 随机选取一个核心对象，找到其密度可达的所有样本，生成一个聚类簇
- 更新簇数k，未访问的样本集合&Gamma;，以及核心样本集合&Omega;
- 直到核心对象集合&Omega;为空时停止迭代

## 四、层次聚类

层次聚类(hierachial clustering)试图在不同层次上对数据集进行划分，从来形成树形的聚类结构，采用自顶向上的聚类策略或者自顶向下的分拆结构。

AGENS算法(AGlomerative NESting)算法是一种自底向上聚合策略的层次聚类算法。其每一步找出聚类最近的两个聚类簇进行合并，不断重复直至达到预设的聚类簇的个数。对于两个聚合簇的计算，常采用如下策略去计算：

![层次聚类距离计算](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/hierachial-clustering-distance.JPG)

距离计算一般使用豪斯多夫距离：

![豪斯多夫距离](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Hausdorff-distance.JPG)

AGNE算法的详细过程如下：

- 初始化单样本聚类簇(每一簇只含有一个样本)
- 初始化聚内簇的距离矩阵
- 找出距离最近的两个聚类簇，合并
- 更新聚类簇和距离矩阵
- 知道聚类簇的个数达到预设的个数时停止迭代

其中，距离的计算可以采用最小距离、最大距离、平均距离，相应的算法称为单链接、全链接、均链接