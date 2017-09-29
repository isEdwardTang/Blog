---
layout: post
title:  "自动化构建工具之Gradle"
categories: BuildTool
tags: BuildTool Gradle
author: Edward
---

* content
{:toc}

gradle是一个新型的构建工具，由于使用grooxy这种动态语言而不是xml进行构建，相比maven有很多优势，简单学习一下。




## 一、构建工具

构建工具的特点：依赖管理，测试、打包、发布，自动化

主流构建工具：

- ant：编译、测试、打包
- mavan：添加依赖管理、发布，使用xml文件进行管理
- gradle：在maven的基础上，使用grooxy进行管理

## 二、下载安装

- 下载压缩包：http://gradle.org，官网很慢，可以去其他地方找资源
- 配置环境变量：GRADLE_HOME
- 添加path：GRADLE_HOME/bin

## 三、Groovy基础

- 完全兼容Java语法
- 分号可选
- 类、方法默认为public
- 自动添加getter/setter
- 属性可以用点号获取
- 函数的最后一个表达式的值作为返回值
- ==等同于equals()，不会抛出空指针
- 自带assert语句，可以在任何地方使用
- 可选类型定义，使用def定义对象
- 可选的括号，函数调用的括号可以省略
- 字符串三种形式：普通字符串使用单引号，双引号可以插入变量，三个单引号可以换行
- 集合api：
    - 使用def list = []定义list，使用list << 追加集合元素，默认为ArrayList
    - 使用def map = [key : value]定义map，使用map.key = value追加map元素，使用map.key或者map[key]获取元素，对应HashMap
- 闭包：一个代码块，可以包含参数或者不包含

```groovy
def c1 = {
    v ->
        println v
}

def c2 = {
    println "hello"
}

def method1(Closure closure) {
    closure("param")
}

def method2(Closure closure) {

}

method1(c1)
method2(c2)
```

## 四、项目构建

### 1、插件配置

在build.gradle中配置构建的插件：

- apply plugin: 'java' jar包构建
- apply plugin: 'war' war包构建

### 2、构建操作

在idea中打开gradle窗口，在Tasks中会显示各种配置中的构建方式，如clear、build、jar、war等，这里构建方式是由于在build.gradle中配置的插件而自带的任务

### 3、项目和任务

项目(org.gradle.api.Project)：相当于一个组件，比如jar或war，当构建启动后，Gradle会基于build.gradle实例化一个Project类，并且能够通过project变量使其隐式可用。

- 属性：group name version 唯一确定一个组件
- 方法：
    - apply 应用一个插件
    - dependencies 依赖
    - repositories 仓库
    - task 声明任务
- 定义属性：
    - ext
    - gradle.properties

任务(org.gradle.api.Task)：包括任务动作和任务依赖

- 方法：
    - dependsOn 任务所依赖的任务
    - doFirst、doLast 任务执行前后的动作
    - 每一个插件会带几个任务
- 自定义创建任务：

    task 任务名 {

    }

```groovy
def createDir = {
    path ->
        File dir = new File(path)
        if (!dir.exists()) {
            dir.mkdirs()
        }
}

task makeJavaDir() {
    def paths = ['src/main/java', 'src/main/resources', 'src/test/java', 'src/test/resources']
    doFirst {
        paths.forEach(createDir)
    }
}

task makeWebDir() {
    dependsOn 'makeJavaDir'
    def paths = ['src/main/webapp']
    doLast {
        paths.forEach(createDir)
    }
}
```

### 4、构建声明周期：

- 初始化(初始化项目)
- 配置(配置代码，生成task的依赖关系和执行图，，比如确定task的依赖顺序)
- 执行(动作代码)

## 五、依赖管理：

### 1、仓库

工件坐标：group、name、version

仓库：存放jar包
- 公共仓库：mavenLocal/mavenCentral/jcenter
- 自定义maven仓库，最常见，公司私服
- 文件仓库

### 2、依赖的传递性

### 3、自动化依赖管理

依赖管理(构建脚本)通过网络从远程仓库下载jar包到本地仓库，构建使用时从本地仓库加载jar包，多次使用时会加入缓存

### 4、依赖阶段配置

使用compile、runtime、testCompile、testRuntime等任务，
compile大部分情况都可以使用，runtime在接口时不需要编译依赖，testXXX是测试脚本的依赖

写法：

```groovy
dependencies {
    testCompile group: 'junit', name: 'junit', version: '4.12'
}
```

### 5、配置仓库

```groovy
repositories {
    maven { // 公司私服
        url ''
    }
    mavenLocal()  // 本地
    mavenCentral() // 远程maven中心服务器
}
```

### 6、解决版本冲突

查看依赖报告：help下的dependencies任务查看具体的依赖

强制一个版本，默认为默认最高版本，可以修改默认策略：

```groovy
configurations.all {
    resoultionStrategy {
        failOnVersionConflict()
    }
}
```

解决冲突：

排除传递性依赖：

```groovy
compile () {
    execude group: "", module: ""
}
```

强制指定一个版本：

```groovy
configurations.all {
    resoultionStrategy {
        force ""
    }
}
```

## 六、多项目构建

allproject = rootProject + subProjects

对子项目的依赖：`compile project(":子项目名")`

配置allProject：在setting.gradle中配置

```groovy
rootProject.name = 
include "子项目名"
include ""
```

在rootProject中统一配置插件：

```groovy
allprojects {
    apply plugin: 'java'
    sourceCompatibility = 1.8
}
```

配置子项目依赖:

```groovy
subprojects {
    repositories {

    }
    dependencies {

    }
}
```

rootProject下新建gradle.properties，统一配置版本：

```groovy
group = 
version = 
```

## 七、测试

测试在test目录
编译结果放在classes下，结果在reports目录下的html格式的测试结果

测试发现：
- 继承TestCase或GroovyTestCase
- 被@RunWith注解的类
- 含有@Test注解的类

执行构建，会运行所有测试代码

## 八、发布

发布到本地和远程仓库：maven-publish插件

```groovy
publishing {
    publication {

    }
    reposities {
        maven {
            name ""
            url ""
        }
    }
}
```

然后执行publishing中相应的任务

其中，提交到公司私服，使用publish
