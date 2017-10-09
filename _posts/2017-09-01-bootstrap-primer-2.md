---
layout: post
title: "Bootstrap总结二"
categories: CSS
tags:   primer bootstrap css
author: Edward
---

* content
{:toc}

这次主要整理bootstrap中常用的预定义样式。

--------------------

## 一、文字排版

### 1、对齐

.text-left | 左对齐
.text-center | 居中
.text-right | 右对齐
.text-justify | 两端对齐
.text-nowrap | 文字不换行

### 2、改变大小写

.text-lowercase | 文本全部小写
.text-uppercase | 文本全部大写
.text-capitalize | 单词首字母大写

### 3、引用

.blockquote-reverse	| 设定引用右对齐

### 4、列表

.list-unstyled | 无样式列表
.list-inline | 列表项放在同一行
.dl-horizontal | 定义列表水平排列

## 二、表格

.table | 表格基本样式
.table-striped | 给&lt;tbody&gt;之内的每一行增加斑马条纹样式（不支持IE8）
.table-bordered | 为表格和其中的每个单元格增加边框
.table-hover | &lt;tbody&gt;内鼠标悬停
.table-condensed | 单元格内的padding减半
.table-responsive | 包含&lt;table&gt;，使其变成响应式

## 三、表单

.form-control | 在表单控件上使用，宽度变为100%
.form-group | 用于包含label和表单控件的div，获得最优排列
.form-inline | 用于form上，使其内容左对齐并且表现为inline-block
.form-horizonta | 用于form上，将form-group中的label标签和控件组水平并排布局
.checkbox-inline | 在label上应用，使多选框排列在一行
.radio-inline | 在label上应用，使单选框排列在一行
.form-control-static | 将静态文本（如p）和label放在同一行
.help-block | 在表单控件后的标签使用，使其占满宽度
.input-lg | 大控件
.input-sm | 小控件
.form-group-lg | 大form-group
.form-group-sm | 小form-group

## 四、按钮

.btn | 为按钮添加基本样式
.btn-default | 默认/标准按钮
.btn-primary | 原始按钮样式（未被操作）
.btn-success | 表示成功的动作
.btn-info | 该样式可用于要弹出信息的按钮
.btn-warning | 表示需要谨慎操作的按钮
.btn-danger | 表示一个危险动作的按钮操作
.btn-link | 让按钮看起来像个链接 (仍然保留按钮行为)
.btn-lg | 大按钮
.btn-sm | 小按钮
.btn-xs | 超小按钮
.btn-block | 块级按钮(宽度100%)
.active | 按钮被点击
.disabled | 禁用按钮

其实，其他表单控件也有类似样式，这里不再累述

## 五、其他

- 对于文本标签、控件、背景，都可以设置和按钮一样的text-*，bg-*样式
- .caret使某个元素具有下拉菜单的功能
- .pull-left和.pull-right使元素浮动
- .center-block使块级元素内容居中
- 父元素添加.clearfix清除浮动
- .show和.hidden强制任意元素显示或隐藏，.invisible被用来仅仅影响元素的可见性
