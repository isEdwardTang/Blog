---
layout: post
title: "用Python实现图片转字符画"
categories: Python
tags:   Python practice
author: Edward
---

* content
{:toc}

从实践楼上学习过来的，这里整理一下。




## 一、知识储备

### 1、灰度值

颜色的黑白程度，范围从0-256，白色为255，黑色为0。

### 2、颜色和灰度值的关系

颜色的rgb值，可以映射到灰度值上，计算公式：
gray ＝ 0.2126 * r + 0.7152 * g + 0.0722 * b

即任何一种颜色，都可以用灰度值来表示出

### 3、设计思路

用一个足够长的不重复的列表，计算出颜色的灰度值，将灰度值取整映射到相应位置的字符上，即实现了简单的字符画

## 二、相关库

### 1、命令行解析

使用argparse对命令行参数进行解析

```python
import argparse

parser = argparse.ArgumentParser()  # 获得解析器

parser.add_argument()   # 添加命令行参数

args = parser.parse_args() # 获取参数
```

### 2、图片处理

使用PIL的Image的getpixel()方法获得相应点上的像素值

```python
from PIL import Image

im = Image.open(IMG)    # 打开图片获得Image对象
im = im.resize((WIDTH, HEIGHT), Image.NEAREST)  # 重新设置图片大小

im.getpixel((j, i)) # 获得指定点上的像素的元组
```

## 三、实践

全量的代码如下(参考实验楼教程)：

```python
#!/usr/bin/env python
# encoding: utf-8

"""
@version: ??
@author: Edward
@license: Apache Licence 
@file: ascii.py.py
@time: 2017/9/7 22:50
"""

from PIL import Image
import argparse

# 命令行输入参数处理
parser = argparse.ArgumentParser()

# 参数
parser.add_argument('file')     # 输入文件
parser.add_argument('-o', '--output')   # 输出文件
parser.add_argument('--width', type=int, default=80)    # 输出字符画宽
parser.add_argument('--height', type=int, default=80)   # 输出字符画高

# 获取参数
args = parser.parse_args()

IMG = args.file
WIDTH = args.width
HEIGHT = args.height
OUTPUT = args.output

# 字符画用到的字符集
ascii_char = list("$@B%8&WM#*oahkbdpqwmZO0QLCJUYXzcvunxrjft/\|()1{}[]?-_+~<>i!lI;:,\"^`'. ")


# 将256灰度映射到70个字符上
def get_char(r, g, b, alpha=256):
    if alpha == 0:
        return ' '
    length = len(ascii_char)
    gray = int(0.2126 * r + 0.7152 * g + 0.0722 * b)

    unit = (256.0 + 1) / length
    return ascii_char[int(gray / unit)]

if __name__ == '__main__':

    im = Image.open(IMG)
    im = im.resize((WIDTH, HEIGHT), Image.NEAREST)

    txt = ""

    for i in range(HEIGHT):
        for j in range(WIDTH):
            txt += get_char(*im.getpixel((j, i)))
        txt += "\n"

    print(txt)

    # 字符画输出到文件
    if OUTPUT:
        with open(OUTPUT, 'w') as f:
            f.write(txt)
    else:
        with open("output.txt", 'w') as f:
            f.write(txt)
```
