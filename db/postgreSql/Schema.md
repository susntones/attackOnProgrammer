第一次了解schema的概念。

schema有点类似于命名空间。

默认的schema是public。

schema下有对象如果需要一起删除,需要带上cascade关键字.有点像使用rmdir删除目录一样,文件夹下有东西不然删除.

默认是谁创建的schema,owner就是谁,当然也可以指定
create schema s01 authorization hippo;

postgresql中使用 \dn 显示所有的schema和所有者。

\c - username 切换用户
\d tableName 查看表的字段信息。