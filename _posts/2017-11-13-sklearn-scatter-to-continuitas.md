---
layout: post
title: "scikit-learn中离散特征二值化"
categories: MachineLearning
tags:   datamining machineLearnings 
author: Edward
---

* content
{:toc}

在学习机器学习中遇到的小问题，直接从[scikit-learn中离散特征二值化](http://blog.csdn.net/u012328159/article/details/71617381)这篇博客中摘抄过来。

--------------------

## 一、One-Hot Encoding

使用sklearn.preprocessing的OneHotEncoder类实现热编码：

```python
data = pd.DataFrame({'name':['Tom','Andy','David'],'age':[20,21,22],'height':[175,165,180]})
'''
   age  height   name
0   20     175    Tom
1   21     165   Andy
2   22     180  David
'''
arr = OneHotEncoder(sparse = False).fit_transform(data[['age']])
'''
array([[ 1.,  0.,  0.],
       [ 0.,  1.,  0.],
       [ 0.,  0.,  1.]])
'''
```

但是OneHotEncoder不能处理字符串。

## 二、LabelBinarizer

sklearn.preprocessing的LabelBinarizer可以对字符串进行操作

```python
arr = LabelBinarizer().fit_transform(data['name'])
'''
array([[0, 0, 1],
       [1, 0, 0],
       [0, 1, 0]], dtype=int32)
'''
```

但是LabelBinarizer只能针对以为数组，不能处理多个特征

## 三、get_dummies

pandas的get_dummies()函数可以解决问题

```python
arr = pd.get_dummies(data)
'''
   age  height  name_Andy  name_David  name_Tom
0   20     175          0           0         1
1   21     165          1           0         0
2   22     180          0           1         0
'''
```

## 四、DictVectorizer

sklearn的feature_extraction模块中提供了DictVectorizer类，即把字典向量化，采用0/1二值向量化

```python
arr = DictVectorizer(sparse=False).fit_transform(data.to_dict(orient='record'))
'''
array([[  20.,  175.,    0.,    0.,    1.],
       [  21.,  165.,    1.,    0.,    0.],
       [  22.,  180.,    0.,    1.,    0.]])
'''
```
