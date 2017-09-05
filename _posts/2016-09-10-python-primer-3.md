---
layout: post
title:  "Python入门三：文件操作"
categories: Python
tags:  primer Python
author: Edward
---

* content
{:toc}

每种语言都有其文件流的相应用法，这次介绍Python中的文件流。





## 一、文件操作

### 1、文件对象

和c一样，要想对一个文件进行操作，需要获取该文件的对象：

```python
f = open("xxx") # 打开文件并获取文件对象
f.xxx  # 对文件进行某些操作
f.close() # 关闭文件
```

### 2、访问模式

open函数除了接受一个文件名参数外，还可以设定文件的访问模式(open其他的参数不太能理解）

- 无   以只读方式打开，文件必须存在
- r     以只读方式打开，文件必须存在
- w    以只写方式打开， 先删除原有内容再写入新内容，文件不存在创建新文件
- a    以追加写方式打开，在原有文件末尾添加新内容，文件不存在创建新文件
- \+  r+可读写，文件必须存在，从开头开始写(只覆盖原内容的前面部分)；
　　w+可读写，文件不存在创建新文件，删除原内容后再写；
　　a+可读写，文件不存在创建新文件，在原内容末尾开始写
- t　  文本模式(默认)
- b    二进制模式，如rb, wb, ab, r+b, w+b, a+b等
- U    通用换行符格式(将\r, \n, \r\n 都转化为\n)，不建议使用
 
## 二、文件内置方法

假设现在有一个同级目录下的文件test.txt:

```python
I was a handsome boy!
I love China!
Hello python!
```

### 1、输入

- read(n)->str 读取指定字节到字符串中，默认读到文件末尾

```python
f = open('test.txt')
print(f.read(5))    # 读取5个字节
print(f.read())      # 读取剩余所有字符串
f.close()

"""输出：
I was
 a handsome boy!
I love China!
Hello python!
"""
```

- readline(n)->str 读取指定字节到字符串中，默认读到行结尾(最后一行读到文件结尾)

```python
f = open("test.txt")
print(f.readline(5))    # 读取5个字节
print(f.readline())      # 读取到这一行的末尾
f.close()


"""输出：
I was
 a handsome boy!
"""
```

- readlines()->list 读取所有剩余的行，作为字符串列表返回，其中包括换行符

```python
f = open("test.txt")
print(f.readlines()) 
f.close()

"""输出：
['I was a handsome boy!\n', 'I love China!\n', 'Hello python!']
"""
```

### 2、输出

- write(str)->int 将指定字符串写入文件中，返回字符串的长度

```python
f = open('test.txt', 'w+')
print(f.write("I love China!"))  # 返回写入的长度
f.close()
```

- writelines(lst) 将一个字符串列表写入文件中，换行符不会被加入

```python
f = open('test.txt', 'w')
f.writelines(['I am handsome!\n', 'I love China!\n', 'Hello Python!'])
f.close()
# 需要手动添加换行符
```

### 3、移动

- seek(offset, 0) 移动文件指针， 0表示从开头开始，1表示从当前位置，2表示从文件末尾，需要以b形式打开

```python
f = open("test.txt", 'rb')
print(f.read(5))
f.seek(12, 1)    # 文件指针从当前位置移动
print(f.read(5))
f.close()

"""输出：
b'I was'
b'boy!\r'
"""
```

- tell()->int 告诉当前文件指针的位置

### 4、迭代

文件支持和其他可迭代对象一样的迭代访问，并且与readlines()相比更高效

```python
f = open('test.txt')
for eachLine in f:
    print(eachLine.strip())   # 需要手动地去除末尾的换行符
f.close()

"""输出：
I was a handsome boy!
I love China!
Hello python!
"""
```

### 5、其他

- fileno()->int 返回底层的打开文件的描述符
- flush() 直接把内部缓冲区的数据立即写入文件
- truncate()->int 截取文件到文件指针位置，可以指定或用f.tell()，返回截断后的长度
 
## 三、文件内置数据属性

- f.closed 文件关闭时为True
- f.encoding 文件所使用的编码
- f.mode 文件打开时的访问模式
- f.name 文件名

```python
1 f = open('test.txt')
2 print(f.closed, f.encoding, f.mode, f.name)
3 f.close()
4 
5 """输出：
6 False cp936 r test.txt
7 """
```

## 四、with语句

用于常常会忘带关闭文件，可以把文件对象的作用域放在with as中，当离开作用域后，文件自动关闭

```python
with open('test.txt') as f:
    pass
```