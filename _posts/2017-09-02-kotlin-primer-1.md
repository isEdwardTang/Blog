---
layout: post
title: "Kotlin学习记录1"
categories: Kotlin
tags:   primer Kotlin
author: Edward
---

* content
{:toc}

今年谷歌开发者大会kotlin宣布作为安卓开发的官方语言，看来Google是要真的准备要和oracle对着干啊，估计未来必是一片光芒。撑着年轻抓紧时间学习！





## 一、语法糖

kotlin中的语法糖是在太多了，用起来只能说，贼爽（虽然抄了C#和Python很多^-^)。

### 1、null safe

在Java中动不动就会抛空指针，要么就得加一堆判断，而kotlin是空安全的。kotlin默认引用都是非空的，
要想允许为null，必须：

```kotlin
var a: String = "edward"  // 不能为null
var b: String? = "edward" // 可以为null
```

这样，你就可以对a为所欲为了。
另外，如果对一个nullable的引用调用方法，可以使用safe call：

```kotlin
b?.length
```

### 2、string template

可以直接在字符串中使用$引用外部变量，再也不用使用字符串拼接拼来拼去了：

```kotlin
val a = "edward"
println("My name is $a")
```

还可以使用${}来调用方法：

```kotlin:
var a = "edward"
println("edward's length is ${a.length}")
```

注意如果字符串中有$时，通过${'$'}来转义

### 3、when expression

怎么用怎么爽，比switch强多了

```kotlin
when(obj) {
    1 -> "one"
    "Hello" -> "Greeting"
    is Long -> "Long"
    !is String -> "Not a String"
    else -> "Unknown"
}
```

### 4、if expression

和Python中的列表生成式差不多，这样就直接可以用if来给变量赋值了

```kotlin
val max = if (a > b) a else b
```

### 5、collection literals

再也不用先声明一个list，再一个个初始化了：

```kotlin
var args = arrayOf(1, 3, 5)
```

注意这样生成的list是只读的

### 6、date class

现在已经习惯了这样的操作，写了一个pojo类，首先对它的属性生成getter和setter，但其实这是个没有意思的重复工作，kotlin完美解决了这个问题：

```kotlin
data class Customer(val name: String, val email: String)
```

当我们这样定义时，kotlin会为我们自动提供一下方法：

- getters and setters for all properties
- equals()
- hashCode()
- toString()
- copy()
- component1(), component2(), …, for all properties

### 7、extension function

例如：

```kotlin
fun String.spaceToCamelCase() { ... }
"Convert this to camelcase".spaceToCamelCase()
```

这样我们可以直接使用某个类的extend方法，要是在java中，我们只能通过继承来实现了

### 8、singleton

kotlin中创建一个单例十分简单，直接定义一个object就好

```kotlin
object Resource {
    val name = "Edward"
}
```

### 9、with

当调用同一个对象多个方法时，可以使用with语法来简化：

```kotlin
 var s = "Edward"
with(s) {
    println(length)
    println(hashCode())
}
```

### 10、operator overloading

在c++和Python下有运算符重载，可以在Java中就消失了，而kotlin中提供了这样的功能：
通过实现相应的方法，实现重载：

比如，重载+：

```kotlin
data class Point(val x: Int, val y: Int)
operator fun Point.plus(val point: Point) = Point(x + point.x, y + point.y)
Point(1, 2) + Point(3, 4) // Point(x=4, y=6)
```

### 11、其他

- range：1..10，相当于1到10
- 函数默认值：可以直接在定义函数时给函数设置默认值
- is和in：判断是否是某种类型或在某个范围内
- 别名：可以使用as给包定义别名，使用typealias给类型定义别名
- ...
