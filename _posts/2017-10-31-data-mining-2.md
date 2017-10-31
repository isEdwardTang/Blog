---
layout: post
title: "数据挖掘导论整理一之距离度量公式"
categories: 
tags:   datamining
author: Edward
---

* content
{:toc}

部分公式的Python实现

--------------------

## 一、距离公式

### 1、Euclidean distance

```python
def euclidean(vector_a, vector_b):
    return np.sqrt((vector_a - vector_b).dot((vector_a - vector_b).T))
```

### 2、Manhattan Distance

```python
def manhattan(vector_a, vector_b):
    return np.abs(vector_a - vector_b).sum()
```

### 3、Chebyshev Distance

```python
def chebyshev(vector_a, vector_b):
    return np.abs(vector_a - vector_b).max()
```

### 4、Jaccard similarity coefficient

```python
def jaccard(vector_a, vector_b):
    up = np.double(np.bitwise_and((vector_a != vector_b), np.bitwise_or(vector_a != 0, vector_b != 0)).sum())
    down = np.double(np.bitwise_or(vector_a != 0, vector_b != 0).sum())
    return up / down
```

### 5、Cosine Similarity

```python
def cosine(vector_a, vector_b):
    return np.dot(vector_a, vector_b) / (np.linalg.norm(vector_a) * np.linalg.norm(vector_b))
```

### 6、Pearson correlation

```python
def pearson(vector_a, vector_b):
    a = vector_a - np.mean(vector_a)
    b = vector_b - np.mean(vector_b)
    return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
```

### 7、Mahalanobis Distance

```python

```

## 二、scipy中的函数