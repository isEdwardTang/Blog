---
layout: post
title: "Bootstrap总结一"
categories: CSS
tags:   primer Bootstrap CSS
author: Edward
---

* content
{:toc}

在这个前框框架横行的年代，react，vue.js，angularJs等大量前端框架涌现，不过由于现在开发经验少，js只用到了jQuery，而css方面用了少量的Bootstrap，这里参考网上资料做个总结。

--------------------

## 一、源码  

Bootstrap的目录结构如下：

bootstrap/

├── less/

├── js/

├── fonts/

├── dist/

│   ├── css/

│   ├── js/

│   └── fonts/

└── docs/


其中，less/、js/ 和 fonts/ 目录分别包含了 CSS、JS 和字体图标的源码。我们重点关注less这个目录。

最关键的是bootstrap.less、variables.less、utilities.less、mixins文件夹。

bootstrap主文件，把所有的组件样式都放在一起了，编译起来就是这个文件。

variables.less是变量定义文件，里面定义了各种有关颜色、边距等的变量。

utilities.less为公共定义文件，里面定义了诸如“左浮动”，“右浮动”之类的动作，可以通过引用其中的class，实现相应的动作。

mixins文件夹里面包含了各种less文件，用于定义各种组件的具体样式。我们可以引用对应组件的class，达到对各个组件样式的控制。

以后可以参考这些文件的源码来添加相应的样式。

## 二、特点

Bootstrap那么好用，主要是它强大的栅格系统和一些预定义的样式。

### 1、栅格系统

栅格系统通过一系列的row和column的组合来创建页面布局，同时能够兼顾不同的屏幕尺寸，
一下是从官网上截取的栅格参数：

|超小屏幕 手机 (<768px)|小屏幕 平板 (≥768px)|中等屏幕|桌面显示器 (≥992px)|大屏幕 大桌面显示器 (≥1200px)|
|:-------|:-----:|:-----:|:-----:|:-----:|
|栅格系统行为|总是水平排列|开始是堆叠在一起的，当大于这些阈值时将变为水平排列
|.container最大宽度|None （自动）|750px|970px|1170px|
|类前缀|.col-xs-|.col-sm-|.col-md-|.col-lg-|
|列数|12|
|最大列）宽|自动|~62px|~81px|~97px|
|槽宽|30px（每列左右均有 15px）|
|可嵌套|是|
|偏移|是|
|列排序|是|

首先需要为页面内容和栅格系统包裹一个.container容器，
.container类用于固定宽度并支持响应式布局的容器。
.container-fluid类用于100%宽度，占据全部viewport的容器。

所有的列一般放在row中，分成12列：

```css
<div class="row">
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4">.col-md-4</div>
</div>
<div class="row">
  <div class="col-md-8">.col-md-8</div>
  <div class="col-md-4">.col-md-4</div>
</div>
```

使用.col-*-offset-*可以实现列向右偏移指定column的宽度：

```css
<div class="row">
  <div class="col-md-4">.col-md-4</div>
  <div class="col-md-4 col-md-offset-4">.col-md-4 .col-md-offset-4</div>
</div>
```

row中还可以嵌套row

### 2、预定义样式

比如对于button，就有btn-default，btn-primary，btn-success等等一系列不同的样式，我们直接引用就好，这里待后期详细整理。