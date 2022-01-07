# 使用Mycat+springBoot完成分库分表。
`sql目录`:存放的是建表语句
`config`:存放的是scheme.xml和rule.xml配置文件

# mycat 插入数据后的效果
```
mysql> use db2;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> select * from user;
+----+------+
| id | name |
+----+------+
|  1 | tom  |
+----+------+
1 row in set (0.00 sec)

mysql> use db3;
Reading table information for completion of table and column names
You can turn off this feature to get a quicker startup with -A

Database changed
mysql> select * from user;
+----+------+
| id | name |
+----+------+
|  2 | jack |
+----+------+
1 row in set (0.00 sec)

```