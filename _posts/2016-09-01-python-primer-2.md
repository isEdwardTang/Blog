---
layout: post
title:  "Python入门二：函数"
categories: Python
tags:  primer python
author: Edward
---

* content
{:toc}

函数在Python中的精妙用法...

--------------------

## 一、函数的定义和使用

### 1、基本结构

```python
# def 函数名(参数):
#   """
#   文档字符串
#   """
#   函数体
#   返回值
```

### 2、函数名

和变量名命名规则一致，最好不要与内置函数名相同

### 3、参数

和C/C++不同，参数无需指定类型，直接交由解释器去判断：

- 对于number， str， tuple等不可变的对象，相当于传值，即是传递了拷贝
- 对于list，dict，set等可变对象，相当于引用传递，内部更改会影响外部的值

a.普通参数：和c类似，但是无需指定类型，所以任何类型都可以传递给函数

```python
def func(argument):
    print(argument)


func("string")
func(4)
```

b.默认参数：与c++中一样，也能在定义时给参数指定一个缺省的值，但是必须放在参数列表后面位置

```python
def func(name, age = 20):
    print(name, age)

func("Edward")
func("Edward", 18)
```

c.动态参数：对于动态参数而言，最大好处是可以灵活的使用参数，而无须考虑其个数，其通过tuple(一般用*args表示)和dict(一般用**kwargs)的特性来实现：

- 对于tuple，一般用户用a, b, c, ... 的形式，会被解释器自动转化为一个tuple来存储，解决了任意数量的普通参数的传递
- 对于dict，一般用户用x1 = a1, x2 = a2, x3 = a3,...的形式，会被转化为一个dict来存储，解决了任意数量的关键词参数的传递

```python
def func(*args, **kwargs):
    for i in args:
        print(i)
    for k, v in kwargs.items():
        print("%s = %s" % (k, v))


func("Edward", 19)
func(name = "Edward", age = 19)
func("Edward", "Tang", age = 19)
```

也可以直接将一个tuple或list传递给args, 将一个dict传递给kwargs，但要注意此时必须在引用实参的时候加上*或**:

```python
tup = ("Edward", 19)
dic = dict(name = "Edward", age = 19)
func(*tup)
func(**dic)
# 如果不加*， 会被认为是tuple的一个元素
```

### 4、文档字符串

写函数时，最好在内部最开始加一个docstrings，即文档字符串，方便其他人理解函数的功能
其有下面几个要求：

- 使用三个双引号来区别多行注释
- 第一行作为函数功能的简要概述，最好以大写字母开头，句号结尾，无需明确对象的类型和名字
- 第二行为空
- 后面叙述函数的具体功能，一定要有函数的参数以及返回值的详细描述
- 可以用__doc__来引用模块的文档字符串

### 5、函数体

函数的具体实现

### 6、返回值

即将函数的执行结果返回，未指定为None

在Python中，由于tuple的存在，可以一次性返回多个值：

```python
def func(a):
    return a * a, a ** a


x, y = func(4) # x = 16, y = 256
```

### 7、函数的调用

- 由于Python的解释以及执行顺序都是从上往下，所以要想调用函数，必须函数在之前有定义
- 在Python中，未加函数定义的语句属于主体，相当于c中的主函数，一般放在最后，以便调用之前的函数
- 若有几个文件的相互引用，可添加一下代码： 在一个文件中，相当于主函数的入口，但是如果此文件作为模块被其他文件引用，则此段代码由于为False，将不会执行，所以可以用作测试模块的功能

```python
def func()
    pass


if __name__ == "__main__":
    func()
```

## 二、lambda表达式

即一个小的匿名的函数，一般只有函数体很短时使用：

```python
a = lambda x: x ** 2
a(2)
# 4
```

### 1、与filter、map、reduce的结合使用

```python
seq = [1, 76, 5, 44, 13,  5, 23]

a = filter(lambda x : x > 10, seq)
# list(a) = [76, 44, 13, 23]

b = map(lambda x : x ** 2, seq)
# list(b) = [1, 5776, 25, 1936, 169, 25, 529]

from functools import reduce
c = reduce(lambda x, y: x * y, range(1, 100))
# c的结果为99！
```

### 2、与sorted的结合使用

```python
seq = ["Tang", "Edward", "love", "handsome"]
seq = sorted(seq, key=lambda a : a.upper())
# seq = ['Edward', 'handsome', 'love', 'Tang'] 
```

## 三、内置函数

Python内置了丰富的函数，适合于各种类型的对象，下面来详细讨论

### 1、大多数的函数

```python
def abs(*args, **kwargs):
    pass
# 返回参数的绝对值

def all(*args, **kwargs):
    pass
# 返回True如果可变对象所有元素都为真，为空时返回True

def any(*args, **kwargs):
    pass
# 返回False如果可变对象所有元素都为假，为空时返回True

def bin(*args, **kwargs):
    pass
# 返回参数的二进制表示

def hex(*args, **kwargs):
    pass
# 返回参数的十六进制表示

def oct(*args, **kwargs):
    pass
# 返回参数的八进制表示

def callable(i_e_, some_kind_of_function):
    pass
# 返回对象是否可调用

def chr(*args, **kwargs):
    pass
# 返回整数参数对应的ASCII码的字符

def ord(*args, **kwargs):
    pass
# 返回单个字符的unicode值

def delattr(x, y):
    pass
# 删除对象x的‘y’属性（类似于del x.y）

def getattr(object, name, default=None):
    pass
# 返回object的'name'的属性的值，若不存在，返回default

def hasattr(object, name):
    pass
# 返回True如果object对象有指定的‘name’属性

def setattr(x, y, v):
    pass
# 设置x的'y'属性的值为v(类似于x.y = v)，其中y属性可以是不存在的

def dir(p_object=None):
    pass
# 如果没有参数，返回当前范围的参数、方法、定义的list
# 如果有参数，返回参数的属性，方法的list，且存在__dir__会被调用

def divmod(x, y):
    pass
# 返回x//y, x%构成的tuple

def eval(*args, **kwargs):
    pass
# 计算表达式，并返回结果

def exec(*args, **kwargs):
    pass
# 动态执行代码

def repr(obj):
    pass
# 返回obj的可供解释器读取的字符串，可以用eval()求值
# 大多数情况下，eval(repr(obj)) == obj

def exit(*args, **kwargs):
    pass
# 退出

def format(*args, **kwargs):
    pass
# 转化为type(value).__format__(format_spec)

def globals(*args, **kwargs):
    pass
# 返回当前全局变量构成的字典

def locals(*args, **kwargs):
    pass
# 返回当前局部变量构成的字典

def hash(*args, **kwargs):
    pass
# 返回参数(哈希表类型的对象)的哈希值

def help():
    pass
# 返回参数的帮助信息

def id(*args, **kwargs): 
    pass
# 返回参数的内存地址(并非实际内存地址)

def input(*args, **kwargs):
    pass
# 打印提示字符串，并读取输入返回(str类型)

def isinstance(x, A_tuple):
    pass
# 返回x是否为元组A_tuple中其中一个类的实例

def issubclass(x, A_tuple):
    pass
# 返回x是否为元组A_tuple中其中一个类的子类

def iter(source, sentinel=None):
    pass
# 返回第一个参数对象的迭代器，
# 若有第二个参数，当迭代器的__next__返回值为它时抛出异常

def len(*args, **kwargs):
    pass
# 返回容器的item个数

def max(*args, key=None):
    pass
# 返回所有参数中的最大值，或序列中的最大值(容器为空返回key)
    
def min(*args, key=None):
    pass
# 返回所有参数中的最小值，或序列中的最小值(容器为空返回key)

def next(iterator, default=None):
    pass
# 返回迭代器的下一个值，若已经到最后一个返回default

def open(file, mode='r', buffering=None, encoding=None, 
        errors=None, newline=None, closefd=True):
    pass
# 以特定形式打开文件

def pow(*args, **kwargs):
    pass
# 两个参数是返回x**y, 三个参数时返回x**y%z

def print(self, *args, sep=' ', end='\n', file=None): 
    pass
# 打印，默认以空格隔开各打印值，以换行结束，不刷新

def quit(*args, **kwargs): 
    pass
# 退出

def round(number, ndigits=None):
    pass
# 返回number的四舍五入表示

def sorted(*args, **kwargs):
    pass
# 返回递增的排序的list

def sum(iterable， start = 0):
    pass
# 返回序列的和加上start(默认为0)

def vars(p_object=None):
    pass
# 不带参数，返回当前对象属性及属性值的字典
# 带参数，返回参数对应的属性及值的字典

def int(x, base = 10):
    pass
# 返回以base进制表示的x的int形式

def float(x):
    pass
# 返回x的float形式

def bool(x):
    pass
# 返回x的bool表示

def complex(a, b):
    pass
# 返回a+bj

def str(x)：
    pass
# 返回一个str

def dict(x)：
    pass
# 返回一个字典

def list(iterable)：
    pass
# 返回一个list

def tuple(iterable):
    pass
# 返回一个tuple    
    
def set(iterable)：
    pass
# 返回一个set    
    
def frozenset(iterable):
    pass
# 返回一个不可变的set

def enumerate(iterable):
    pass
# 构造序列的下标和值构成的元祖，用于循环遍历

def filter(function or None, iterable)：
    pass
# 返回iterable中能够让function的返回值为真的元素的序列，
# 若function为None, 返回iterable中为真的元素的序列

def map(func, *iterables):
    pass
# 对每一个iterable, 使用func, 并将结果作为list返回

def range(start = 0, stop):
    pass
# 返回一个从start到stop构成的序列，用于遍历

def reversed(seq)：
    pass
# 返回一个seq反转的序列

def type(object):
    pass
# 返回object的类型

def zip(iter1 [,iter2 [...]])：
    pass
# 分别从iter中取下标相同的元素构成tuple，在将各tuple构成list
# 使用zip(*list)解压

# 其他函数
# copyright, credits, license, bytearray, bytes, classmethod,
# memoryview, property, slice, staticmethod, super, compile
```

### 2、内置函数总结

- 数学计算和其他计算：abs, divmod, hash, len, max, min, pow, round, sorted, sum,  reversed
- 逻辑判断：all, any
- 进制转换：bin, hex, oct
- 类型转换：int, float, bool, complex, str, dict, list, tuple, set, frozenset
- 类相关：callable, delattr, getattr, hasattr, setattr, dir, isinstance, issubclass
- 对象和属性：vars, type, id
- 字符串和字符编码：chr, ord, eval, exec, repr, format
- IO相关: input, open, print, exit, quit
- 迭代器和遍历：iter, next, enumerate, range, zip
- 函数相关：filter, map
- 其他：globals, locals, help

3、几个函数详解

- delattr, getattr, hasattr和setattr：

```python
class Student(object):
    def __init__(self, name):
        self.name = name

    def have_class(self):
        print("%s is having class." % self.name)

s = Student("Edward")

# name 以下都必须是字符串格式

# hasattr(object, name), 判断对象是否具有name属性
print(hasattr(s, "name"))    # True
print(hasattr(s, "have_class"))    # True

# getattr(object, name, default=None), 返回对象的name属性的值
# 可以设置default, 但是仅仅是没有找到时返回它，并没有添加
print(getattr(s, "name"))    # Edward
print(getattr(s, "age", 19))  # 19
getattr(s, "have_class")()    # 会运行该属性
print(hasattr(s, "age"))    # False, 并没有添加

# setattr(object, name, value), 设置对象的name的属性值为value
# 若name属性不存在， 还会添加该属性
setattr(s, "name", "Tang")
print(s.name)   # Tang
setattr(s, "age", 19)
print(hasattr(s, "age"))  # True, 会添加该属性

# delattr(object, name) 删除对象的name属性
delattr(s, "name")
print(hasattr(s, "name"))  # False, 已被删除
```

- eval和exec：

```python
# exec(), 动态执行代码
exec("print('Edward Tang')")
 
# eval() 计算表达式的值并放回
a = eval("7 * 6 + 1")
print(a) # 43
```

- filter和map：

```python
def func1(n):
    if n > 10:
        return True
    
def func2(n):
    return n * n

def func3(a, b, c):
    return a * b * c


seq = [1, 76, 5, 44, 13, 3, 5, 23]
li1 = [4, 5, 6, 8]
li2 = [9, 7, 10, 6]
li3 = [5, 4, 3, 1]


# filter对seq中的每一个元素执行func1, 如果为True, 返回原列表的这些值
rt1 = filter(func1, seq)
print(list(rt1))

# map对seq中的每一个元素执行func2，返回这些值执行的结果构成的序列
rt2 = map(func2, seq)
print(list(rt2))

# 若func有多个参数，可以提供多个序列，分别依次带入，返回结果
rt3 = map(func3, li1, li2, li3)
print(list(rt3))

# 在functools中还存在一个reduce的函数
# reduce(func, seq, start) func接受两个参数，
# 对seq中两两的数进行递归调用，并返回
from functools import reduce
def  func(a, b):
    return a * b
rt = reduce(func, range(1, 100))
# 计算99的阶乘
```

- sorted：  

```python
# sorted(iterable, key=None, reverse=False)
# key可以用函数或lambda表达式
# 指定reverse = True会降序排序
# sorted只是返回一个排序好的序列，并不改变原序列

# 普通排序
seq = [1, 76, 5, 44, 13, 3, 5, 23]
seq = sorted(seq, reverse=True) # 降序

#使用lambda
seq = ["Tang", "Edward", "love", "handsome"]
seq = sorted(seq, key=lambda a : a.upper())

# 对列表的某项排序
arr = [['Tang', 89], ['Edward', 79], ['Hu', 67], ['Wang', 80]]
arr = sorted(arr, key=lambda a : a[1])

# 对类按照某项排序
class Person(object):
    def __init__(self, name, age):
        self.name = name
        self.age = age
p1 = Person('Edward', 18)
p2 = Person('Wang', 25)
p3 = Person('Hu', 20)
p4 = Person('Liang', 22)
for item in sorted([p1, p2, p3, p4], key=lambda p : p.age):
    print(item.name, end=',')

# operator模块还有itemgetter, attrgetter两个函数
# 所以以上最后两个例子还可以表示为
# sorted(arr, key=itemgetter(1))
# sorted([p1, p2, p3, p4], key=attrgetter('age'))
```

- enumerate和zip： 

```python
# enumerate(iterable, start=0)
# 用于循环中，同时得到iterable的值和计数
lst = ['Edward', 'Tang', 'Wang', 'Hu']
for index, item in enumerate(lst):
    print(index, item)

# zip(iter1 [,iter2 [...]])
# 分别从iter中取下标相同的元素构成tuple，再将各tuple构成list
# 使用zip(*list) 做相反的操作
x = [1, 2, 3]
y = [4, 5, 6]
z = [7, 8, 9]
w = zip(x, y, z)
print(list(w))  # [(1, 4, 7), (2, 5, 8), (3, 6, 9)]
# 用在循环中
for a, b, c in zip(x, y, z):
    print(a, b, c)
```

## 四、迭代器与生成器

### 1、迭代器

a.通过iter()构造一个迭代器，然后就可以通过__next__()来访问下一个元素：

a = iter([3, 6, 1, 9])
a.__next__()   # 3
a.__next__()   # 6

b.迭代器只能往前，不能后退，且只能从头到尾依次访问

c.当数据量很多时，用迭代器来遍历，因为迭代器读取数据时，不是把所有的数据都加载到内存中，而是读取到某个元素时才开始

d.可迭代对象：

- Python内置了很多可迭代对象，如list, dic, str等，所有我们可以通过for循环方便地遍历每一个元素，可以通过collections模块的Iterable来判断是否是可迭代的：   

```python
from collections import Iterable
lst = [1, 5, 6, 9]
isinstance(lst, Iterable)   # True 
```

### 2、生成器
当协同程序暂停的时候，可以获得其中一个的返回值，当调用回到程序中时，能够传入额外或者改变了的参数，但仍能够从上次离开的地方继续

a.通过()构造一个生成器，和迭代器类似，再通过__next()__来访问下一个元素：

```python
a = (x * x for x in range(1, 10))
print(a.__next__())    # 1    
print(a.__next__())    # 4
```

b.yeild:用在函数中，类似于return(只是暂停下来，需要通过__next__()或next(f)访问)

```python
def func(n):
    a = 1
    while a < n:
        yield a 
        a += 2

f = func(10)
print(f.__next__())    # 1 
print(f.__next__()) # 3

# 通过yield还可以模拟实现多线程
```

c.send:与__next__()相比，可以传递一个参数给yield

```python
def func(n):
    a = 1
    while a < n:
        b = (yield a)
        if b == None:
            b = 0
        a += b

f = func(10)
print(f.__next__())    # 1
print(f.__next__())    # 1
print(f.send(5))          # 6
print(f.__next__())    # 6
```

d.close:通过f.close()来关闭生成器(不可以通过next继续访问)

## 五、装饰器

### 1、基本语法

@装饰器函数(可选参数)
def 被装饰函数(可选参数)：
　　pass

- 装饰器函数一般会将真正需要执行的函数包裹在内，并返回
- 解释过程中，一般不会执行函数，但会执行迭代器函数，并将其返回值赋给被装饰的函数

### 2、几种情况

a.无参数装饰器：

```python
def deco(func):
   def inner():
       print("Edward")
       print("tang")
       return func()
   return inner


@deco
def func():
    print("handsome")

# 并不一定需要以返回func()的方式执行func(这种情况函数需要最后执行),可以先将其返回值保存在一个变量中，最后将其返回
16 def inner():
　　print("Edward")
　 rt = func()
　　print("tang")
   return rt

# 相当于重新定制了func
```

b.被装饰函数含一个或多个参数：

```python
def deco(func):
    def inner(str1):
        print("Edward")
        return func(str1)
    return inner

@deco
def func(str1):
    print(str1)

func("Tang")

# 保持inner()函数的参数和原来的func()一样多即可
```

c.迭代器函数含参数：

- 由于迭代器在解释阶段就会被执行，所有当包裹一层函数时会抵消它的执行，
- 但是，当给迭代器加上参数时，也相当于执行了一次，所有必须提供两层的内部定义的函数

d.多个装饰器：

```python
def de1(func):
    def inner():
        print("Edward")
        return func()
    return inner

def de2(func):
    def inner():
        print('tang')
        return func()
    return inner


@de1
@de2
def func():
    print("handsome")

func()

# 相当于func = de1(de2(func()))
```

f.functools.wraps:可以保留被装饰函数原来的一些属性，如__name__, __doc__等  

```python
def deco(func):
    # @functools.wraps(func)
    def inner():
        print("Edward")
        print("tang")
        return func()
    return inner

@deco
def func():
    """ A hansome boy! """
    print("handsome")

print(func.__name__)
print(func.__doc__)

# 会输出 inner和None
# 如果去掉注释,  输出func和A handsome boy!
```

## 六、偏函数

即将任意数量的参数的函数转化成另一个带剩余参数的函数对象，需要导入functools模块的partial：

```python
from operator import add, mul
from functools import partial

add1 = partial(add, 1)
mul100 = partial(mul, 100)

print(add1(99))  # 100
print(mul100(99))  # 9900
```

简单应用(摘自 《Core Python Programming》)：

```python
"""easy_gui.py"""

from functools import partial
import tkinter
# Tkinter模块是python中一个能快速创建GUI的标准库

root = tkinter.Tk()
# 创建一个顶层窗口对象
MyButton = partial(tkinter.Button, root, fg='white', bg='blue')
# 用偏函数设置按钮的默认属性
b1 = MyButton(text='Button 1')
b2 = MyButton(text='Button 2')
qb = MyButton(text='QUIT', bg='red', command=root.quit)
b1.pack()
b2.pack()
qb.pack(fill=tkinter.X, expand=True)
root.title('PFAs!')
root.mainloop()
```
