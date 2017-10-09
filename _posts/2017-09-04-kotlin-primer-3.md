---
layout: post
title: "Kotlin学习记录3"
categories: Kotlin
tags:   primer kotlin
author: Edward
---

* content
{:toc}

这次总结kotlin的其他语法和类的相关知识。

--------------------

## 一、其他特殊语法

### 1、for循环

对于实现了iterator()、next()、hasNext()方法的，可以使用for in语法，有三种形态：

直接遍历：

```kotlin
for (item: Int in ints) {
    // ...
}
```

遍历的同时获取下标：

```kotlin
for (i in array.indices) {
    print(array[i])
}
```

遍历的同时获取下标和值：

```kotlin
for ((index, value) in array.withIndex()) {
    println("the element at $index is $value")
}
```

### 2、loop@标记

在Java中，想要跳出循环可以使用标记，而在kotlin中，同样也有，不过功能更加强大。

跳出多层循环：

```kotlin
loop@ for (i in 1..100) {
    for (j in 1..100) {
        if (...) break@loop
    }
}
```

跳出lambda表达式：

```kotlin
fun foo() {
    ints.forEach lit@ {
        if (it == 0) return@lit
        print(it)
    }
}
```

也可以使用隐式方法，保证函数名和label一致：

```kotlin
fun foo() {
    ints.forEach {
        if (it == 0) return@forEach
        print(it)
    }
}
```

## 二、类

### 1、构造器

kotlin中的构造器分为两种：primary constructor 和 secondary constructor

- primary constructor：

在header上使用constructor关键字，可以在init中初始化：

```kotlin
class Person constructor(firstName: String) {
    init {
        // ...
    }
}
```

没有annotations和visibility modifiers时，constructor可以被省略

简明的声明属性的方法：

```kotlin
class Person(val firstName: String, val lastName: String, var age: Int) {
    // ...
}
```

含有注解的情况：

```kotlin
class Customer public @Inject constructor(name: String) {
   // ...
}
```

- secondary constructor：

在body中使用constructor关键字：

```kotlin
class Person {
    constructor(parent: Person) {
        parent.children.add(this)
    }
}
```

含有primary constructor时，secondary constructor需要delegate primary constructor，可以使用this关键字：

```kotlin
class Person(val name: String) {
    constructor(name: String, parent: Person) : this(name) {
        parent.children.add(this)
    }
}
```

非抽象类没有声明primary constructor时，会有默认构造器

### 2、创建实例

和Java不一样，在kotlin中创建实例不需要使用new

```kotlin
val invoice = Invoice()
val customer = Customer("Joe Smith")
```

### 3、继承

所有类默认继承Any(含有equals、hashCode和toString方法)

继承使用：基类语法：

```kotlin
open class Base(p: Int)
class Derived(p: Int) : Base(p)
```

默认kotlin中所有类都是final的，要想实现继承，需要加open关键字

### 4、重写方法

- 需要重写的方法，显式加open修饰
- 被重写的方法，使用override修饰
- 没有被open修饰的父类方法，子类要么override，要么不写
- 没有被open修饰的类，不可以加open修饰给方法

子类override可以被它的子类重写，不想这样，声明为final：

```kotlin
open class AnotherDerived() : Base() {
    final override fun v() {}
}
```

### 5、重写属性

- 和重写方法使用一样
- val属性可以被var属性覆盖
- 使用super调用父类方法

内部类中，使用super@Outer获得外面的类：

```kotlin
class Bar : Foo() {
    override fun f() { /* ... */ }
    override val x: Int get() = 0
    inner class Baz {
        fun g() {
            super@Bar.f() // Calls Foo's implementation of f()
            println(super@Bar.x) // Uses Foo's implementation of x's getter
        }
    }
}
```

### 6、多继承

在多继承中，相同方法必须重写，可以使用super<Base>获得某个父类：

```kotlin
open class A {
    open fun f() { print("A") }
        fun a() { print("a") }
    }
    interface B {
        fun f() { print("B") } // interface members are 'open' by default
        fun b() { print("b") }
    }
    class C() : A(), B {
    // The compiler requires f() to be overridden:
    override fun f() {
        super<A>.f() // call to A.f()
        super<B>.f() // call to B.f()
    }
}
```

### 7、抽象类

使用abstract关键字
