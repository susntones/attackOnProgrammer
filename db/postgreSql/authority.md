postgres 权限管理
=============

#### 概述

在PostgreSQL 里没有区分用户和角色的概念，"CREATE USER" 为 "CREATE ROLE" 的别名，这两个命令几乎是完全相同的，唯一的区别是"CREATE USER" 命令创建的用户默认带有LOGIN属性，而"CREATE ROLE"
命令创建的用户默认不带LOGIN属性(CREATE USER is equivalent to CREATE ROLE except that CREATE USER assumes LOGIN by default, while CREATE ROLE does not)。


[参考文章](http://www.cnblogs.com/mchina/archive/2013/04/26/3040440.html)