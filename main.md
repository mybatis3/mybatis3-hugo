+++
title = "MyBatis2"
description = ""
weight = 10
type = ""

draf = true

+++

## 强烈推荐必读文章

- [深入了解 MyBatis 参数](http://blog.csdn.net/isea533/article/details/44002219)
- [深入了解 MyBatis 返回值](http://blog.csdn.net/isea533/article/details/46442067)
- [MyBatis-Spring 配置简单了解](http://blog.csdn.net/isea533/article/details/45640319)
- [MybatisGeneator 详解](http://blog.csdn.net/isea533/article/details/42102297)
- [MyBatis Geneator 中文文档](http://mbg.cndocs.tk/)
- [MyBatis 博客专题](http://blog.csdn.net/column/details/mybatis-sample.html)

## MyBatis官方内容

官方仓库：https://github.com/mybatis/mybatis-3

当前版本：[![Maven central](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis)

官方文档：http://mybatis.github.io/mybatis-3/index.html

MyBatis-Spring 官方文档：https://mybatis.github.io/spring/index.html



## MyBatis 分页插件

源码地址：

- [https://github.com/pagehelper/Mybatis-PageHelper](https://github.com/pagehelper/Mybatis-PageHelper)
- [http://git.oschina.net/free/Mybatis_PageHelper](http://git.oschina.net/free/Mybatis_PageHelper)

当前版本：[![Maven central](https://maven-badges.herokuapp.com/maven-central/com.github.pagehelper/pagehelper/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.pagehelper/pagehelper)

## MyBatis 通用 Mapper

源码地址：

- [https://github.com/abel533/Mapper](https://github.com/abel533/Mapper)
- [http://git.oschina.net/free/Mapper](http://git.oschina.net/free/Mapper)

当前版本：[![Maven central](https://maven-badges.herokuapp.com/maven-central/tk.mybatis/mapper/badge.svg)](https://maven-badges.herokuapp.com/maven-central/tk.mybatis/mapper)

## 关注微信订阅号 - 获取最新相关信息

![wxgzh](images/wxgzh.jpg)

## MyBatis 和 Spring 集成示例

> 只有基础的配置信息，没有任何现成的功能，作为新手入门搭建框架的基础

- [集成Spring4.x](https://github.com/abel533/Mybatis-Spring) - [下载zip](https://github.com/abel533/Mybatis-Spring/archive/master.zip)
- [集成Spring3.x](https://github.com/abel533/Mybatis-Spring/tree/spring3.x) - [下载zip](https://github.com/abel533/Mybatis-Spring/archive/spring3.x.zip)
- [集成Spring4.x(使用Oracle数据库)](https://github.com/abel533/Mybatis-Spring/tree/mybatis-oracle) - [下载zip](https://github.com/abel533/Mybatis-Spring/archive/mybatis-oracle.zip)
- [spring4-simple](https://github.com/abel533/Mybatis-Spring/tree/spring4-simple)  -  [下载zip](https://github.com/abel533/Mybatis-Spring/archive/spring4-simple.zip)

前三个框架集成了 **MyBatis 分页插件**和 **MyBatis 通用 Mapper**，最后一个**spring4-simple** 没有集成任何插件。



## Spring Boot 和 MyBatis 集成示例

### [https://github.com/abel533/MyBatis-Spring-Boot](https://github.com/abel533/MyBatis-Spring-Boot)

上面这个项目集成了**MyBatis 分页插件**和 **MyBatis 通用 Mapper**.

## 其他插件

### JdbcType 自动配置插件 - 运行时自动添加 jdbcType 属性

源码地址：http://git.oschina.net/free/Mybatis_Utils/tree/master/JdbcType

### SqlHelper - 获取sql

gitosc地址：[SqlHelper](http://git.oschina.net/free/Mybatis_Utils/tree/master/SqlHelper)

相关文章： [Mybatis工具SqlHelper - 获取Mybatis方法的Sql](http://blog.csdn.net/isea533/article/details/40044417)

### PerformanceInterceptor

### 性能拦截器，用于输出每条 SQL 语句及其执行时间

源码地址：http://git.oschina.net/free/Mybatis_Utils/tree/master/Performance

#### 简单说明：

性能分析拦截器主要输出Sql以及Sql执行的时间，该拦截器会损失一定的整体性能，所以建议在测试环境使用，正式环境不建议使用。

另外，如果配置了多个拦截器，那么一定要把这个拦截器配置在第一个，否则其他需要修改Sql的拦截器会对该拦截器获取Sql部分产生影响。

建议根据个人需求对该拦截器进行修改。

### CameHumpInterceptor

### 返回值Map结果的Key转为驼峰式

例如返回结果中Map的`{REAL_NAME:liuzh}`会转换为`{realName:liuzh}`

源码地址：http://git.oschina.net/free/Mybatis_Utils/tree/master/CameHumpMap
