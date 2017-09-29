---
layout: post
title:  "Python入门一：基本数据类型"
categories: Python
tags:  primer Python
author: Edward
---

* content
{:toc}

作为一个刚入门编程的大一狗，第一次写博客，希望能对自己学的知识进行巩固和提升，也希望记录自己成长的过程。

学习Python，一是因为暑假学的c++头疼，听说Python简单，那我就试试吧，二是因为Python形势一片大好，算是附和潮流吧！

--------------------

## 一、初识Python

### 1、第一个Python代码

```python
print("Hello World")
```

依然是熟悉的Hello World， 对于只学过c和c++的我来说，着实有点奇怪，怎么main()没了(其实是有的)，头文件也没了，甚至连一句语句的末尾标识逗号也不见踪影。

### 2、概览

用下面一段猜大小的代码码来解释一下python与c（c++）的区别

C:
```c
#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main(void)
{
    int try_num, true_num, x, count;

    while(1)
    {
        printf("请选择: 1.猜大小 2.退出: ");
        scanf("%d", &x);
        if(x == 2)
            break;
        srand(time(0));
        true_num = rand() % 100 + 1;
        printf("请输入你猜的数字（1-100）: ");
        scanf("%d", &try_num);
        count = 1;
        while(try_num != true_num)
        {
            if(try_num >= 1 && try_num <= 100)
            {
                if(try_num > true_num)
                    printf("你猜大了！\n");
                else
                    printf("你猜小了！\n");
            }
            else
                printf("你输入的数字有误！\n");
            printf("请再次输入你猜的数字: ");
            scanf("%d", &try_num);
            count++;
        }
        printf("你终于猜对了, 共用了%d次.\n", count);
    }

    return 0;
}
```

Python:
```python
import random


while True:
    x = int(input("请选择: 1.猜大小 2.退出: "))
    if x == 2:
        break
    true_num = random.randint(1, 100)
    try_num = int(input("请输入你猜的数字（1-100）: "))
    count = 1
    while try_num != true_num:
        if try_num in range(1, 101):
            if try_num > true_num:
                print("你猜大了！")
            else:
                print("你猜小了！")
        else:
            print("你输入的数字有误！")
        try_num = int(input("请再次输入你猜的数字: "))
        count += 1
    print("你终于猜对了, 共用了%d次" % count)
```
能清楚的看出，用Python写出的代码较c简洁美观，没有冗余，在语法上的几点区别总结如下：

- 变量没有类型的声明，而是根据右侧表达式推断
- 语句结尾没有分号
- 循环语句和条件语句均以冒号标志其内部
- 以缩进而不是大括号来区分作用域
- ...

两者也具有高级语言的类似特点：

- 都有条件语言，循环语言，判断语言等，大体用法相同，最大区别是in的使用，类似于c++11中的范围for
- 都有基本的运算符，但是python增加了**，//，<>，去掉了逻辑运算符中的符号表达，全部由and，or，not等- 关键词表示
- ...

## 二、基本数据类型

与c不同，Python的面向对象特征更加明显，连int，float等也有自己的方法；
与c++相比，Python的list，tuple，dict 等相较与STL的容器更容易使用，内置的方法也较丰富

### 1、int， float， complex

```python
# int 方法
def bit_length(self):
    pass
# 返回该整数用二进制表示时的最小位数

def __divmod__(self, *args, **kwargs):
    pass
# 返回一个tuple, 包含两个元素，分别为self 与 argument相除的商和余数


# float 方法
def as_integer_ratio(self):
    pass
# 返回一个tuple， 即将float转化为分数形式

def fromhex(self, string):
    pass
# 返回16进制表示的string转化为的float

def hex(self): 
    pass
# 与fromhex（）相反

def is_integer(self, *args, **kwargs):
    pass
# 返回 bool，判断float是否为整数


# complex 方法
def conjugate(self):
    pass
# 返回复数的共轭复数
```
对于complex a， 可以通过a.real和a.imag使用其实部和虚部

### 2、bool

True, False
例如， 可以

```python
a = True
while a:
    # ...
    if ...:
        a = False
```

### 3、str

通过'', "" 或 str()构建

```python
def capitalize(self):
    pass
# 返回str的首字母大写，其余小写的形式， str不变

def casefold(self):
    pass
# 返回str的所有字母变为小写的形式， str不变

def center(self, width, fillchar=None):
    pass
# 返回str居中，长度为width，左右以fillchar填充的形式，str不变

def count(self, sub, start=None, end=None):
    pass
# 返回str中[start, end)范围内sub的数目

def endswith(self, suffix, start=None, end=None): 
    pass
# 返回str的[start, end) 子序列是否以suffix结尾

def expandtabs(self, tabsize=8):
    pass
# 返回str的所有tab变成tabsize长度的空格， str不变

def find(self, sub, start=None, end=None):
    pass
# 返回str的[start, end) 范围内sub的位置， 未找到返回-1

def rfind(self, sub, start=None, end=None): 
    pass
# 与find()不同的是从右向左

def format(self, *args, **kwargs):
    pass
# 返回str的格式化的字符串， 使用{}而非%，str不变

def index(self, sub, start=None, end=None):
    pass
# 返回str的[start, end) 子序列的sub所在的下标， 未找到报错

def rindex(self, sub, start=None, end=None): 
    pass
# 与index()不同的是从右向左

def isalnum(self): 
    pass
# 返回str是否全部由字母和数字构成

def isalpha(self):
    pass
# 返回str是否全部由字母构成

def isdigit(self):
    pass
# 返回str是否全部由数字构成

def islower(self):
    pass
# 返回str是否所有字母都是小写

def isupper(self):
    pass
# 返回str是否所有字母都是大写

def isspace(self):
    pass
# 返回str是否全部由空白字符构成

def istitle(self):
    pass
# 返回是否所有单词都是大写开头

def join(self, iterable):
    pass            
# 返回通过指定字符str连接序列iterable中元素后生成的新字符串

def ljust(self, width, fillchar=None): 
    pass
# 返回str左对齐，不足width的以fillchar填充， str不变

def rjust(self, width, fillchar=None): 
    pass
# 返回str右对齐，不足width的以fillchar填充， str不变

def lower(self):
    pass
# 返回str全部小写的拷贝， str不变

def upper(self):
    pass
# 返回str全部大写的拷贝， str不变

def swapcase(self): 
    pass
# 返回str全部大小写交换的拷贝， str不变

def strip(self, chars=None):
    pass
# 返回str移除左右两侧所有chars的拷贝，str不变

def lstrip(self, chars=None): 
    pass
# 返回str移除左侧所有chars的拷贝，str不变

def rstrip(self, chars=None):
    pass
# 返回str移除右侧所有chars的拷贝，str不变

def partition(self, sep):
    pass
# 返回str以sep分割的前，sep，后部分构成的tuple，
# 未发现返回sep和两个空字符构成的tuple

def rpartition(self, sep):
    pass
# 和partition()不同的是从右向左

def replace(self, old, new, count=None):
    pass
# 返回str把count数目的old替换为new的拷贝，str不变

def split(self, sep=None, maxsplit=-1):
    pass
# 返回一个以sep分隔str的maxsplit(默认最大)的list，str不变

def rsplit(self, sep=None, maxsplit=-1):
    pass
# 和split()不同的是从右向左

def splitlines(self, keepends=None):
    pass
# 返回一个以\n或\r或\r\n分隔的list，若keepends=true，保留换行

def startswith(self, prefix, start=None, end=None):
    pass
# 返回str的[start, end)范围内是否以prefix开头

def title(self):     
    pass
# 返回所有单词是大写开头的拷贝，str不变

def zfill(self, width):
    pass
# 返回str的以width为长度，不够左侧补0的拷贝(不会截短)，str不变

def maketrans(self, *args, **kwargs):
    pass
# 返回生成的一个翻译表，与translate()搭配使用

def translate(self, table): 
    pass
# 根据maketrans()生成的table来翻译str，返回拷贝，str不变
```

a.对str中的方法的总结：

- 大小写，空格与table，特定格式等的转化，替换： capitalize，casefold，expandtabs，format，lower，upper，swapcase，replace，title，maketrans，translate
- 填充与移除字符串，连接与分隔字符串： center，strip，lstrip，rstrip，join，ljust，rjust，partition，rpartition，split，rsplit，splitlines，zfill
- 子序列数目，位置：count，find，rfind，index，rindex
- 判断字母，数字，大小写，空格，开头，结尾 ：endswith，isalnum，isalpha，isdigit，islower，isupper，isspace，istitle，startswith
- 和左右扫描方向有关的方法一般还包括一个r__()方法，表示从右向左扫描
- 所有方法均不改变str，只是返回一个拷贝或bool

b.几个方法详解：

- format:

```python
# 通过位置
string1 = "{0} is the most {1} teacher of life"
str1 = string1.format("Suffering", "powerful")
# str1 = "Suffering is the most powerful teacher of life"
string2 = "{0}, {1}, {0}"
str2 = string2.format("Edward", "Tang"}
# str2 = "Edward, Tang, Edward"

# 通过关键词
string = "{name} is  {age}"
str = string.format(name="Edward", age=19)
# str = "Edward is 19"

# 填充和对齐
# ^、<、>分别是居中、左对齐、右对齐，后面带宽度
# :号后面带填充的字符，只能是一个字符，不指定的话默认是用空格填充
string1 = "{: >6}"
str1 = string1.format("Ed")
# str1 = "    Ed"
string2 = "{:*<6}"
str2 = string2.format("Ed")
# str2 = "Ed****"

# 控制精度
string = “{:.2f}”
str1 = string.format(3.1415926)
# str1 = "3.14"

# 金额分隔符
string = "{:,}"
str = string.format(1234567)
# str = "1,234,567"
```

- maketrans和translate：

```python
# s.maketrans('s1', 's2') s1 和 s2 的长度必须一致，生成一个转换表
# s.translate(table) 对字符串s按照table里的字符映射关系替换
s = "I was a handsome boy"
table = s.maketrans("abcde", "12345")
str = s.translate(table)
# str = "I w1s 1 h1n4som5 2oy"
```

- join和split：

```python
# join用于用指定str连接参数的str序列
lst = ['a', 'b', 'c', 'd']
s = '-'.join(lst)
# s = "a-b-c-d"

def accum(s):
    return '-'.join(c.upper() + c.lower() * i for i, c in enumerate(s))
# s = "abcd"，返回 “A-Bb-Ccc-Dddd”

# split用于用指定参数拆分str
s = "a-b-c-d"
lst = s.split('-')
# lst = ['a', 'b', 'c', 'd']
```

c.索引和切片：
Python中的索引和C类似，但是可以从右边开始：

```python
word = "python"
# word[0] = 'p'
# word[5] = 'n'
# word[-1] = 'n', 表示最后一个， -0和0一样
```

除了索引， 还支持切片：

```python
word = "python"
# word[0: 2] = 'py'
# word[2: 5] = 'tho'
# word[: 2] = 'py', 等同于[0: 2]
# word[3:] = 'hon'， 等同于[3: len(word)]
# word[::-1] = "nohtyp"，反转字符串
```

切片和c++中的迭代器类似，都是为单闭合区间；
切记str是const的， 不可以通过赋值等改变它们

### 4、list

通过[]或list()构建

```python
def append(self, p_object):
    pass
# 添加元素p_object到list末尾,p_object可以是任何类型

def clear(self):
    pass
# 清空list中的元素

def copy(self):
     pass
# 返回一个list的浅拷贝

def count(self, value):
    pass
# 返回list中的value的个数

def extend(self, iterable)
    pass
# 添加整个iterable到list末尾，扩展list

def index(self, value, start=None, stop=None):
    pass
# 返回子序列[start, stop)中value第一次出现的下标，未找到报错

def insert(self, index, p_object):
    pass
# 插入一个p_object到下标为index的元素之前

def pop(self, index=None):
    pass
# 弹出index位置的元素并返回此元素, list为空或index超出范围会报错

def remove(self, value):
    pass
# 清除list中第一个值为value的元素，不返回此值

def reverse(self):
    pass
# 反转整个list

def sort(self, key=None, reverse=False):
    pass
# 排序list，key可以为lambda或cmp，reverse为True需要反转
```

a.对list中方法的总结：

- 添加：append, extend, insert
- 删除：clear, pop, remove
- 搜素：count, index
- 拷贝：copy
- 排序：sort
- 反转：reverse
- 与str不同，list中元素大都直接修改list，返回None而不是拷贝

b.几个方法详解：

- append和extend：

```python
lst = [1, 5, 4, 3, 8]
lst.append(3) 
# lst = [1, 5, 4, 3, 8, 3]
lst.append([1, 2, 3]) 
# lst = [1, 5, 4, 3, 8, 3, [1, 2, 3]]，始终把参数当做一个元素
lst.extend([1, 2, 3])
#[1, 5, 4, 3, 8, 3, [1, 2, 3], 1, 2, 3]，合并为一个list
```

c.索引和切片：
与str基本一致，但是由于list可变，还存在一个del语言：

```python
lst = [3, 4, 5, 6, 7]
del lst[0]
# lst = [4, 5, 6, 7]
del lst[1:3]
# lst = [4, 7]
del lst[:]
# lst = []
```

### 5、tuple

通过()或tuple()构建(括号可以省略), 只包含一个元素时，在元素后面添加逗号

```python
def count(self, value):
    pass
# 返回tuple中value的个数

def index(self, value, start=None, stop=None):
    pass
# 返回子序列[start, stop)中第一个值为value的下标
```

tuple和list的区别在于其不能改变，所有很多方法没有
tuple也有索引和切片，不再赘述
要想对tuple进行强制修改，可以通过list()构造

### 6、dict

:通过{}或dict()构建

```python
def clear(self): 
    pass
# 清空dict中的元素

def copy(self):
    pass
# 返回dict的一个拷贝

def fromkeys(*args, **kwargs):
    pass
# 返回一个dict，所有的key都对应同一个value（默认为None）

def get(self, k, d=None):
    pass
# 返回key为k时对应的value，如果不存在，返回d

def setdefault(self, k, d=None):
    pass
# 返回key为k时对应的value，如果不存在，添加一个k: d

def items(self): 
    pass
# 返回dict中所有key, value构成的dict_items()

def keys(self):
    pass
# 返回dict中所有key构成的dict_keys()

def values(self)：
    pass
# 返回dict中所有value构成的dict_values()

def pop(self, k, d=None):
    pass
# 弹出dict中k所对应的value，没找到返回d

def popitem(self):
    pass
# 随机弹出dict中一个(key, value)，dict为空时出错

def update(self, E=None, **F):
    pass
# 用另一个dict F 来更新原dict， 返回None
```

a.对dict中方法的总结：

- 添加：直接用dic[key] = value即可添加
- 删除：clear, pop, popitem
- 查找, 引用：get, setdefault, items, keys, values
- 构建：copy, fromkeys, update
- 与list类似，但由于是无序的，所有没有下标的操作，且popitem弹出的元素也是随机的

b.几个方法详解：

- pop和popitem:

```python
dic = {'k1': 'v1', 'k2': 'v2', 'k3': 'v3'}
# key为str的构建时也可以写成 dic = dict(k1 = 'v1', k2 = 'v2', k3 = 'v3)
k = dic.pop('k1')
# k = 'v1'且 dic = {'k2': 'v2', 'k3': 'v3'}
item = dic.popitems()
# item = （‘k2’, 'v2'）或('k3', v3') 因为dic是无序的，且dic会随之变化
```

- get和setdefault: 

```python
dic = {'k1': 'v1', 'k2': 'v2', 'k3': 'v3'}
s1 = get('k1')  # s1 = dic['k1']
s2 = get('k4', 'v4')  # s2 = 'v4'
s1 = setdefault('k1')  # s1 = dic['k1']
s2 = setdefault('k4', 'v4')  # dic['k4'] = 'v4'
```

- items, keys, values:

```python
dic = {'k1': 'v1', 'k2': 'v2', 'k3': 'v3'}
for k in dic.keys():
    print(k) 
for v in dic.values():
    print(v)
for k, v in dic.items():
    print(k, v)
# 分别输出了dic中所有的key， value和键值对
```

-  fromkeys和update：

```python
# fromkeys第一个参数可以是任意类型的序列，
# 第二个参数为空默认value都为None
dic = dict.fromkeys(('k1', 'k2', 'k3'))
# dic = {'k2': None, 'k1': None, 'k3': None}
dic = dict.fromkeys(('k1', 'k2', 'k3'), 520)
# dic = {'k2': 520, 'k3': 520, 'k1': 520}

# update将dic1更新， 返回None
dic1 = {'k1': 13, 'k2': 14, 'k3': 520}
dic2 = {'k4': 'Edward', 'k3': '250'}
dic = dic1.update(dic2)
# dic = None
# dic2 = {'k1': 13, 'k2': 14, 'k3': 250, 'k4': 'Edward'}
```

### 7、set

通过set()构建

```python
def add(self, *args, **kwargs):
    pass
# 向set中添加一个元素，返回None

def clear(self, *args, **kwargs):
    pass
# 清空set中的元素

def copy(self, *args, **kwargs):
    pass
# 返回一个set的浅拷贝

def difference(self, *args, **kwargs):
    pass
# 返回一个set，其中不含参数集合中的元素，差集

def difference_update(self, *args, **kwargs): 
    pass
# 和difference()相比，set自身更新为差集，返回None

def symmetric_difference(self, *args, **kwargs):
    pass
# 返回集合之间的对称差集

def symmetric_difference_update(self, *args, **kwargs):
    pass
# 和symmetric_difference()相比，set自身更新为对称差集，返回None

def intersection(self, *args, **kwargs):
    pass
# 返回set和参数集合的交集

def intersection_update(self, *args, **kwargs):
    pass   
# 和intersection()相比，set自身更新为交集，返回None

def union(self, *args, **kwargs):
    pass
# 返回set和参数集合的并集 
  
def update(self, *args, **kwargs):
    pass
# 和union()相比，set自身更新为并集，返回None

def discard(self, *args, **kwargs):
    pass
# 清除set中的参数元素，返回None， 若没有不做任何事，

def isdisjoint(self, *args, **kwargs):
    pass
# 返回集合之间是否交集为空

def issubset(self, *args, **kwargs):
    pass
# 返回是否set为参数集合的子集

def issuperset(self, *args, **kwargs):
    pass    
# 返回是否set为参数集合的父集

def pop(self, *args, **kwargs):
    pass
# 弹出set中一个随机的值并返回，set为空会出错

def remove(self, *args, **kwargs):
    pass
# 清除set中的参数元素，返回None，没有会出错
```

a.对set中方法的总结:

- 差集，交集，并集运算：difference, difference_update, symmetric_difference, symmetric_difference_update, intersection, intersection_update, union, update
- 添加元素：add
- 删除元素：clear, discard, remove, pop
- 拷贝：copy
- 判断空集，父集，子集：isdisjoint, issubset, issuperset
- 集合间的运算都有两个版本，分别直接在原set上操作和返回一个拷贝
- 与dict相比，没有key，也是无序的，所有没有下标操作，pop也是随机弹出元素

b.集合的运算符：

a, b, c均为集合

- 差集：c = a - b 等同于 c = a.difference(b)

    a -= b 等同于 a.difference_update(b)

- 对称差集：c = a ^ b 等同于 c = a.symmetric_difference(b)

    a ^= b 等同于 a.symmetric_difference_update(b)

- 交集：c = a & b 等同于 c = a.intersection(b)

    a &= b 等同于 a.intersection_update(b)

- 并集：c = a | b 等同于 c = a.union(b)

    a |= b 等同于 a.update(b)

- 判断子集： a <= b 等同于 a.issubset(b)

- 判断父集： a >= b 等同于 a.issupperset(b)
