---
layout: post
title: "Java任务调度之Quartz"
categories: Java
tags:   Java scheduling
author: Edward
---

* content
{:toc}

工作做到批量这块，使用的是quartz调度，对底层不是很了解，深入学习一下。

--------------------

## 一、开始Quartz

### 1、引入依赖

```xml
<!-- https://mvnrepository.com/artifact/org.quartz-scheduler/quartz -->
<dependency>
    <groupId>org.quartz-scheduler</groupId>
    <artifactId>quartz</artifactId>
    <version>2.3.0</version>
</dependency>
```

### 2、定义Job类

Job类是实现业务逻辑的代码，即调度器调用的方法，需要实现Job类及其方法：

```java
public class HelloJob implements Job {
    @Override
    public void execute(JobExecutionContext context)
     throws JobExecutionException {
        ...
    }
}
```

### 3、创建JobDetail实例

JobDetail实例需要制定name和group，并绑定job类：

```java
JobDetail jobDetail = JobBuilder
        .newJob(HelloJob.class)
        .withIdentity("myjob", "group1")
        .build();
```

### 4、创建Trigger实例

Trigger实例需要指定name和group，并定义触发时机：

```java
Trigger trigger = TriggerBuilder.
        newTrigger()
        .withIdentity("myTrigger", "group1")
        .startNow()
        .withSchedule(
            SimpleScheduleBuilder
            .simpleSchedule()
            .withIntervalInSeconds(2)
            .repeatForever())
        .build();
```

### 5、创建Schedule实例

创建Schedule实例，start，并绑定jobDetail和trigger:

```java
SchedulerFactory sfact = new StdSchedulerFactory();
Scheduler scheduler = sfact.getScheduler();
scheduler.start();
scheduler.scheduleJob(jobDetail, trigger);
```

每次调度器执行job时，在调用execute之前创建一个job实例，调用结束后回收

## 二、JobDetail

JobDetail: 为Job实例提供了许多设置属性，以及JobDataMap成员变量属性，用来存储特定Job实例的状态信息，调度器需要借助JobDetail对象来添加Job实例

### 1、属性

- name 任务名称
- group 所在组的名称，默认为DEFAULT
- jobClass 任务的实现类
- jobDataMap 参数Map

### 2、创建一个JobDetail

```java
JobDetail jobDetail = JobBuilder
    .newJob(HelloJob.class)
    .withIdentity("myjob", "group1")
    .build();
```

### 3、获得属性

```java
jobDetail.getKey().getName()
jobDetail.getKey().getGroup()
jobDetail.getJobClass().getName()
```

## 三、JobExecutionContext

JobExecutionContext：用于在Job中获取JobDetail和Trigger的参数

### 1、设置参数

```java
// 使用usingJobData(key, value)
JobDetail jobDetail = JobBuilder
        .newJob(HelloJob.class)
        .withIdentity("myjob", "group1")
        .usingJobData("message", "hello myJob1")
        .usingJobData("FloatJobValue", 3.14F)
        .build();
Trigger trigger = TriggerBuilder
        .newTrigger()
        .withIdentity("myTrigger", "group1")
        .usingJobData("message", "hello myTrigger1")
        .usingJobData("DoubleTriggerValue", 2.0D)
        .startNow()
        .withSchedule(
            SimpleScheduleBuilder
            .simpleSchedule()
            .withIntervalInSeconds(2)
            .repeatForever())
        .build();
```

### 2、获取参数

方法一：在job中获得jobDetail和trigger，然后获得其dataMap

JobDataMap:用来装载任何可序列化的数据对象

```java
public void execute(JobExecutionContext context) 
    throws JobExecutionException {
JobDataMap dataMap = context.getJobDetail().getJobDataMap();
String jobMessage = dataMap.getString("message");
Float jobFloatValue = dataMap.getFloat("FloadJobValue");

JobDataMap tdataMap = context.getTrigger().getJobDataMap();
String triMessage = dataMap.getString("message");
Double triggerDoubleValue = tdataMap.getDouble("DoubleTriggerValue");

// 获得合并的DataMap（以trigger中为准)：
JobDataMap mdataMap = context.getMergedJobDataMap();
```

方法二：在Job中加上相应成员变量和getter和setter方法

```java
public class HelloJob implements Job {
    private String message;
    private Float floatJobValue;
    private Doubel doubleJobValue;

    // getter and setter

    @Override
    public void execute(JobExecutionContext context) 
        throws JobExecutionException {
        // 直接使用属性值
    }

}
```

## 四、SimpleTrigger

作用：在一个指定时间段内执行一次作业任务，或是在指定的时间间隔内多次执行作业任务

```java
SimpleTrigger trigger = (SimpleTrigger)TriggerBuilder
    .newTrigger()
    .withIdentity("myTrigger", "group1")
    .startAt(date)
    .withSchedule(SimpleScheduleBuilder
            .simpleSchedule()
            .withIntervalInSeconds(2)
            .withRepeatCount(SimpleTrigger.REPEAT_INDEFINITELY))
    .build();
```

### 1、设置执行开始时间

- startNow()
- startAt()

### 2、设置结束时间

- endAt()

### 3、设置执行间隔

- withIntervalInSeconds()

### 4、设置执行次数

- withRepeatCount()
- repeatForever() 等同于 withRepeatCount(SimpleTrigger.REPEAT_INDEFINITELY)

## 五、CronTrigger

基于日历的作用调度器，使用更多更灵活。

### 1、创建

```java
CronTrigger trigger = (CronTrigger)TriggerBuilder
        .newTrigger()
        .withIdentity("myTrigger", "group1")
        .withSchedule(CronScheduleBuilder.cronSchedule("* * * * * ?"))
        .build();
```

### 2、cron表达式

上述声明中的cronSchedule中指定cron表达式，可以指定某个时刻执行次数等。

- 格式：一个字符串，用空格隔开，依次表示 秒 分 小时 日 月 周 年

|字段名 |  允许的值 | 允许的特殊字符  |
|:--:|:--|:--|
秒  | 0-59 | , - * / |
分  | 0-59 |   , - * / |
小时| 0-23 |  , - * /  |
日  | 1-31 | , - * ? / L W C | 
月  | 1-12 or JAN-DEC | , - * / |
周几 | 1-7 or SUN-SAT | , - * ? / L C # |
年 (可选字段) | empty, 1970-2099 | , - * / |

- 特殊字符：

    - “?”字符：表示不确定的值

    - “,”字符：指定数个值

    - “-”字符：指定一个值的范围

    - “/”字符：指定一个值的增加幅度。n/m表示从n开始，每次增加m

    - “L”字符：用在日表示一个月中的最后一天，用在周表示该月最后一个星期X

    - “W”字符：指定离给定日期最近的工作日(周一到周五)

    - “#”字符：表示该月第几个周X。6#3表示该月第3个周五

## 六、Scheduler

### 1、创建SchedulerFactory

```java
ScheulerFactory sfact = new StdSchedulerFactory()
Scheduler scheduler = sfact.getScheduler();

DirectSchedulerFactory factory = DirectSchedulerFactory.getInstance();
Scheduler scheduler = factory.getScheduler();
```

### 2、StdSchedulerFactory:

- 使用一组参数来创建和初始化quartz调度器
- 配置参数一般存储在quartz.properties
- 调用getScheduler方法就能创建和初始化调度器对象

### 3、相关方法

- Date scheduleJob(JobDetail jobDetail, Trigger trigger) 绑定jobdetail和trigger
- void start() 启用scheduler
- void standby() 暂时挂起scheduler
- void shutdown() 关闭scheduler
- void shutdown(boolean)
true表示等待所有正在执行的job执行完毕之后，再关闭
false是直接关闭

## 七、quartz.properties

声明式编程的设计模式，启动时引用工程下的quartz.properties，不存在引用org.quartz下的quartz.properties

### 1、调度器属性

- org.quartz.scheduler.instanceName: 区分特定的调度器实例
- org.quartz.scheduler.instanceid: 必须在所有调度器实例中是唯一的，尤其是一个集群中，作为集群唯一key。可以设置AUTO

### 2、线程池属性

- org.quartz.threadPool.threadCount: 工作线程的数量
- org.quartz.threadPool.threadPriority: 线程优先级1-10(默认为5)，用在集群中
- org.quartz.threadPool.class: 线程池实现，默认org.quartz.simpl.SimpleThreadPool

### 3、作业存储设置

- job和trigger如何存储
- org.quartz.jobStore.class: org.quartz.simpl.RAMJobStore

### 4、插件配置

## 八、Spring和Quartz集成
