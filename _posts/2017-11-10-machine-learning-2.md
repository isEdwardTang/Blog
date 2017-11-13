---
layout: post
title: "机器学习之二神经网络"
categories: MachineLearning
tags:   datamining machineLearning neturalNetworks
author: Edward
---

* content
{:toc}

神经网络的有关学习知识。

--------------------

## 一、神经元模型

### 1、M-P神经元模型

神经元接收来自其他n个神经元的输入信号，通过带权重的连接进行传递，然后将接收到的总的输入值和神经元的阈值比较，通过激活函数处理产生该神经元的输出。

![M-P模型](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/m-pmodel.png)

### 2、激活函数

理想中使用阶跃函数作为激活函数，但是其不连续，一般使用Sigmod函数：

![阶跃函数和Sigmod函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/activation_function.png)

### 3、感知机

感知机通常由两层神经元组成，输入层接收外界输入信号后传递给输出层，输出层是M-P神经元，输入层的神经元之间进行与或非等运算：

![感知机](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/perceptron.png)

感知机每次权重的调整如下：

![调整感知机权重](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/perceptron_adjust.png)

由于感知机只有一层功能神经元，只能进行线性可分的问题的训练，学习能力有限。

### 4、多层网络

和感知机相比，多层网络使用了多层神经元，每层神经元和下一层的神经元全互连，中间的神经元称为隐含层，隐含层和输出层都是具有激活函数的功能神经元，输入层仅仅是接收输入：

![多层前馈网络](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/multi-layer-feedforward-netural.png)

## 二、误差逆传播算法

BP算法指的是误差逆传播(error BackProgation)算法或反向传播算法，可用来解决多层前馈神经网络。

### 1、梯度下降

BP算法基于梯度下降策略，即每次对参数进行调整时都是以目标的负梯度方向调整

### 2、BP算法

如图所示：

![BP算法变量符号](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-flag.png) ，输出层神经元阈值和隐层神经元阈值分别用&theta;和&gamma;表示

每次训练的目的就是不断地改变连接权和阈值，使最终的网络的均方误差最小：

![神经网络的输出](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-output.png)<br />
![均方误差](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-error.png)

进行一系列的推导，我们知道了每次连接权和阈值的更新公式：

![输出层连接权](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-output-weight.png)<br />
![其他更新公式](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-other-update.png)

其中，&eta;表示学习率，其他所用公式如下，其中g表示输出层的梯度项，e表示隐层的梯度项
![BP所用公式g](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-gradient-g.png)<br />
![BP所用公式b](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-b.png)<br />
$$e^h$$ ![BP所用公式e](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-gradient-e.png)

有时候为了精细化处理，输出层和隐层所用的学习率可以不必相等

### 3、BP算法的工作流程

- 输入训练集D和学习率&eta;
- 在(0,1)范围内初始化网络中所有连接权和阈值
- 对于所有的样本点，计算当前样本的输出y，及g和e
- 更新连接权和阈值
- 重复操作

### 4、累计BP算法

之前我们使用的是标准BP算法，是对于某一个输出神经元的均方误差最小，而BP实际是要最小化训练集上的累计误差：

![累计误差](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-error-cum.png)

- 一般先使用累计BP算法使累计误差下降到一定程度，再使用标准BP算法

### 5、隐藏神经元个数的确定

使用试错法

### 6、过拟合

- 早停：将数据分成训练集和验证集，训练集用来计算梯度、更新连接权、阈值，验证集用来估计误差，若训练集误差降低但验证集误差升高，则停止训练，并返回具有最小验证集误差的连接权和阈值。
- 正则化：在误差目标函数中增加一个用于描述网络复杂度的部分，如下，其中&gamma;对经验误差和网络复杂度进行折中，常使用交叉验证法来估计：

![调整后的误差目标函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/BP-E-adjust.png)

### 7、全局最小和局部最小

使用梯度下降，得到的可能只是一个局部的最小值，常常使用以下策略跳出局部最小：

- 以多组不同参数值初始化多个神经网络，按照标准方法训练后，取其中误差最小的解作为最终的参数
- 使用模拟退火算法，每一步都以一定的概率接受比当前解更差的结果（有助于跳出局部最小）。在每步迭代的过程中，接受次优解的概率要随着时间的推移逐渐降低
- 使用随机梯度下降，在计算梯度时加上随机因素（即使陷入局部极小点，计算中的梯度可能不为0，就有可能跳出局部最小
- 使用遗传算法

## 四、其他算法

### 1、RBF

径向基函数网络（Radial Basic Function），单隐层前馈神经网络，使用径向基函数作为隐层激活函数，输出层为隐层神经元的线性组合：

![RBF网络](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/RBF.png)

q为隐层神经元的个数，c和w表示隐层神经元的中心和权重，&rho;表示径向基函数，定义为样本x到数据中心ci之间欧式距离的单调函数，常用的为高斯径向基函数：

![高斯径向基函数](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/RBF-function.png)

训练步骤：
- 确定神经元中心c，常使用随机采样、聚类等
- 利用BP算法来确定w<sub>i</sub>和&beta;<sub>i</sub>

### 2、ART

自适应谐振网络（Adaptive Resonanse Theory）是一种竞争型学习（输出神经元相互竞争，每次只能有一个获胜的神经元被激活，其他被抑制），由比较层、识别层、识别阈值和重置模块构成：

- 比较层负责接收输入样本、并将其传递给识别层神经元。
- 识别层每一个神经元对应一个模式类（某类别的子类），神经元数目可以在训练过程中动态增长以增加新的模式类

竞争的方式：

- 计算输入向量和每个识别层神经元的模式类的代表向量之间的距离，取最小者，并让其他神经元抑制
- 如果输入向量和获胜神经元对应的代表向量的相似度大于识别阈值，则将当前输入样本规为该代表向量所属类别，同时更新连接权，使以后相似输入样本对该模式类的相似度更高
- 如果相似度不大于阈值，重置模块会重新增设一个新的神经元，其代表向量为当前输入向量

### 3、SOM

自组织映射网络（Self-Organizing Map）是一种竞争学习型的无监督神经网络，可以将高维输入数据映射为低维，同时保持其拓扑结构。
输出层神经元一般以矩阵方式排列在二维空间中 。

训练步骤：
- 计算输入样本和每一个输出层神经元的权向量的距离，距离最近的神经元称为最佳匹配单元
- 最佳匹配单元及其邻近神经元的权向量将被调整，使得这些神经元和输入样本距离缩小
- 不断迭代，直至收敛

### 4、级联相关网络

级联相关网络（Cascade-Correlation）是一种结构自适应网络，网络结构也是其训练的目标之一。

训练过程：
- 开始训练时，只有输入层和输出层
- 级联：随着训练进行，新的隐层神经元加入，新的神经元加入时，其输入端连接权是固定的
- 相关：最大化新神经元的输出和网络误差之间的相关性来训练相关的参数

### 5、Elman

ELman网络是一种递归神经网络（网络中允许出现环形结构，让一些神经元的输出反馈回来作为输入信号），结构和多层前馈网络相似，但隐层神经元的输出被反馈回来，与下一时刻输入层神经元提供的信号一起作为输入。

### 6、Boltzmann机

Boltzmann机是一种基于能量的模型，其神经元分为显层和隐层，显层表示数据的输入输出，隐层为数据的内在表达，Boltzmann机的能量定义为：

![Boltzmann机能量](https://raw.githubusercontent.com/isEdwardTang/Blog/gh-pages/images/Boltzmann-energy.png)

其中，w表示连接权，s表示激活或者抑制状态（0或1），&theta;表示阈值。

由于标准的Boltzmann机复杂度高，一般采用受限的Boltzmann机（RBM），只保留显层和隐层的连接，采用CD算法（对比散度Contrastive DIvergence）

### 7、深度学习

深度学习采用多隐层神经网络。常用的算法包括DBN和CNN。

## 五、sckit-learn的神经网络库

使用sklearn.neural_network.MLPClassifier来直接对多层感知机分类：

MLPClassifier的参数解释如下：

| 参数 | 说明 |
| :---: | :---: |
| hidden_layer_sizes | 元组，表示每一个隐层的神经元个数 |
| activation | 隐层激活函数，默认为relu，即f(x) = max(0, x)，还可以使用identity、logistic、tanh |
| ... | ... |




