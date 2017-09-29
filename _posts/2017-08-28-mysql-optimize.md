---
layout: post
title: "mysql优化"
categories: Mysql
tags:  mysql optimize
author: Edward
---

* content
{:toc}

今天公司组织了关于mysql性能的优化，实习一个多月来也见识了不同场景下的sql的应用，这里整理一下。

--------------------

## 一、使用join而不是子查询

in和not in虽然写起来简单易懂，但会导致全表查询，不建议使用，而是用join来代替

in的替换（内连接）：

```sql
# SELECT * FROM customer WHERE ID in (SELECT customer_id FROM sales) 
SELECT * FROM customer JOIN sales ON customer.ID = salesin.customer_id
```

not in的替换（左外连接）:

```sql
# SELECT * FROM customer WHERE ID NOT in (SELECT customer_id FROM sales) 
SELECT * FROM customer LEFT JOIN sales ON customer.ID = salesin.customer_id WHERE sales.customer_id IS NULL
```

注意在使用join时，只把连接条件写在on后面，而把其他的过滤条件写在where后面

根据业务场景，使用join还是left join，一般为了符合正常思维逻辑，不会使用right join和full join

使用join还能使逻辑更加清晰，因为连接条件紧跟在连接表的后面

## 二、批量更新和插入

频繁访问数据库的一个很糟糕的做法，不建议使用，而是在sql中写好批量插入和更新的语句，在Java中调用一次就好：

错误写法：

```sql
<insert id="">
    INSERT INTO 
        customer (ID, name)
    VALUES 
        (id, name)
</insert>
```

```java
for (Customer customer : customerList) {
    Mapper.insert(customer);
}
```

正确写法：

```sql
<insert id="" parameterType="java.util.List">
    INSERT INTO 
        customer (ID, name)
    VALUES 
        <foreach collection="list" item="item" index="index" separator=",">  
            (#{item.id}, #{item.name})  
        </foreach>  
</insert>
```

```java
Mapper.insert(customerList);
```

## 三、约束的使用

工作中大量的bug都是由于不严谨的代码造成的，而在sql中使用约束是一个很好的减少bug的方式。

## 四、不使用distinct

在数据量很大的情况下，使用排序操作会影响性能，group by、order by和distinct都会造成排序，所以使用distinct的效率很低。可以使用exists来代替distinct：

```sql
# SELECT DISTINCT id, name FROM customer, customerinfo WHERE customer.ID = customerinfo.customer_id 

SELECT id, name FROM customer WHERE EXISTS (SELECT 'T' FROM customerinfo WHERE customerinfo.customer_id = customer.id)
```

原因是exists在子查询满足条件时，立即返回，这里使用一个常量作为子查询的返回结果，因为exists并不考虑查询的结果，而常量显然比查询一个字段更快

## 五、使用索引

索引适用于那些经常查询（一般是多表），但是很少插入的语句

在mysql中，使用explain + 查询语句可以来优化查询

常用参数：

- type：显示连接使用了何种类型。从最好到最差的连接类型为const、eq_reg、ref、range、indexhe和all

- possible_keys：显示可能应用在这张表中的索引。如果为空，没有可能的索引。可以为相关的域从where语句中选择一个合适的语句

- key： 实际使用的索引。如果为null，则没有使用索引。很少的情况下，mysql会选择优化不足的索引。这种情况下，可以在select语句中使用use index（indexname）来强制使用一个索引或者用ignore index（indexname）来强制mysql忽略索引

- key_len：使用的索引的长度。在不损失精确性的情况下，长度越短越好

- ref：显示索引的哪一列被使用了，如果可能的话，是一个常数

- rows：mysql认为必须检查的用来返回请求数据的行数,数值越大越不好，说明没有用好索引

- extra：关于mysql如何解析查询的额外信息。using temporary和using filesort是最差的情况，意思mysql根本不能使用索引，结果是检索会很慢

这里详细可参考这篇博客：[mysql explain的使用（优化查询）](http://www.cnblogs.com/0201zcr/p/5742382.html)

## 六、对数据二次加工

我曾经在mybatis中码过如下的代码，被表哥训了一顿：

```sql
<select id="" resultMap="java.util.HashMap" >
    select
    <foreach collection="dimList" item="dim">
        ${dim}, 
    </foreach>
        ... 
    from 
        ...
    where 
        ...
        and pay_order_split.ID in
            <foreach collection="orderList" item="order" index="index"
                open="(" close=")" separator="," >
                #{id}
            </foreach>
    group by
        <foreach collection="dimList" item="dim"
            open="" close="" separator=",">
            ${dim}
        </foreach>
</select>
```

这段代码在sql中执行好几个循环list的语句，其实这些完全可以在外层的Java中加工：

```sql
<select id="" resultType="java.util.HashMap" >
    select
        ${dimList},
        ...
    from 
        ...
    where 
        ...
        and t_pay_order_split.id in (${orderList})
    group by
        ${dimList}
</select>
```
