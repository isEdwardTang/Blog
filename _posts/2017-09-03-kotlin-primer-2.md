---
layout: post
title: "Kotlin学习记录2"
categories: Kotlin
tags:   primer Kotlin
author: Edward
---

* content
{:toc}

这次主要介绍kotlin中基本的数据类型。

--------------------

## 一、基本数据类型

在kotlin中，一切都是对象，所有基本数据类型也有其属性和方法。

### 1、Numbers

包括Double、Float、Long、Int、Short、Byte，

方法：

重载方法：

```kotlin
public operator fun compareTo(other: Number): Int   // 比较
public operator fun plus(other: Number): Number // 加
public operator fun minus(other: Number): Number  // 减
public operator fun times(other: Number): Number    // 乘
public operator fun div(other: Number): Number  // 除
public operator fun rem(other: Number): Number  // 求余
public operator fun inc(): Number   // 自增
public operator fun dec(): Number   // 自减
public operator fun unaryPlus(): Number // 正号
public operator fun unaryMinus(): Number    // 负号

// 整型特有
public operator fun rangeTo(other: Number): LongRange   // a..b
```

类型转化：

```kotlin
toByte(): Byte
toChar(): Char
toShort(): Short
toInt(): Int
toLong(): Long
toFloat(): Float
toDouble(): Double
```

位运算：

```kotlin
shl(bits) – signed shift left (Java's << )
shr(bits) – signed shift right (Java's >> )
ushr(bits) – unsigned shift right (Java's >>> )
and(bits) – bitwise and
or(bits) – bitwise or
xor(bits) – bitwise xor
inv() – bitwise inversion 
```

### 2、Char和Boolean

kotlin中的Char不能被当做数字对待，Char和Boolean具有和Number相同的方法

### 3、Array

创建数组的方式：

- 使用Array(size: Int, init: (Int) -> T)创建指定长度和值的数组
- 使用arrayOf(vararg elements: T): Array<T>快速创建数组
- 使用arrayOfNulls(size: Int): Array<T?>创建指定长度的空数组

数组的取值和赋值：

```kotlin
public operator fun get(index: Int): T // 相当于value = arr[index]
public operator fun set(index: Int, value: T): Unit // 相当于arr[index] = value
```

除了Array外，还可以创建指定了类型的数组：ByteArray、CharArray、ShortArray、IntArray、LongArray、FloatArray、BooleanArray，分别有对应的*arrayOf构建方法。

### 4、String

String在kotlin中也是不可变的，它具有以下从Java中继承来的方法：

```kotlin
String?.equals(other: String?, ignoreCase: Boolean = false): Boolean
String.replace(oldChar: Char, newChar: Char, ignoreCase: Boolean = false): String
String.replace(oldValue: String, newValue: String, ignoreCase: Boolean = false): String
String.replaceFirst(oldChar: Char, newChar: Char, ignoreCase: Boolean = false): String
String.replaceFirst(oldValue: String, newValue: String, ignoreCase: Boolean = false): String
String.toUpperCase(): String
String.toLowerCase(): String
String.toCharArray(): CharArray
String.toCharArray(destination: CharArray, destinationOffset: Int = 0, startIndex: Int = 0, endIndex: Int = length): CharArray
String.format(vararg args: Any?): String
String.Companion.format(format: String, vararg args: Any?): String
String.format(locale: Locale, vararg args : Any?) : String
String.Companion.format(locale: Locale, format: String, vararg args: Any?): String
CharSequence.split(regex: Pattern, limit: Int = 0): List<String>
String.substring(startIndex: Int): String
String.substring(startIndex: Int, endIndex: Int): String
String.startsWith(prefix: String, ignoreCase: Boolean = false): Boolean 
String.startsWith(prefix: String, startIndex: Int, ignoreCase: Boolean = false): Boolean
String.endsWith(suffix: String, ignoreCase: Boolean = false): Boolean
String(bytes: ByteArray, offset: Int, length: Int, charset: Charset): String
String(bytes: ByteArray, charset: Charset): String
String(bytes: ByteArray, offset: Int, length: Int): String
String(bytes: ByteArray): String
String(chars: CharArray): String
String(chars: CharArray, offset: Int, length: Int): String 
String(codePoints: IntArray, offset: Int, length: Int): String
String(stringBuffer: java.lang.StringBuffer): String
String(stringBuilder: java.lang.StringBuilder): String
String.codePointAt(index: Int): Int
String.codePointBefore(index: Int): Int
String.codePointCount(beginIndex: Int, endIndex: Int): Int
String.compareTo(other: String, ignoreCase: Boolean = false): Int
String.contentEquals(charSequence: CharSequence): Boolean
String.contentEquals(stringBuilder: StringBuffer): Boolean
String.intern(): String
CharSequence.isBlank(): Boolean 
String.offsetByCodePoints(index: Int, codePointOffset: Int): Int 
CharSequence.regionMatches(thisOffset: Int, other: CharSequence, otherOffset: Int, length: Int, ignoreCase: Boolean = false): Boolean
String.regionMatches(thisOffset: Int, other: String, otherOffset: Int, length: Int, ignoreCase: Boolean = false): Boolean
String.toByteArray(charset: Charset = Charsets.UTF_8): ByteArray
String.toPattern(flags: Int = 0): java.util.regex.Pattern
String.capitalize(): String
String.decapitalize(): String
CharSequence.repeat(n: Int): String

```

其他：
- 切片：String在kotlin可以通过[index]来获取相应字符，同时具有和Python用法一样的切片，功能十分强大，具体参考我的另一篇博客：[Python入门一：基本数据类型](http://www.isedwardtang.com/2016/08/20/python-primer-1/)
- 元字符串：kotlin具有row string，同样和Python一样，不解释
- 字符串模板：语法糖中有涉及