# MySQL Intro
Front End <--> Back End <--> Database

## DBMS: database management system
- Relational DB: MySQL, Oracle, SqlServer, DB2, SQLite
    - 通过表和表之间，行和列之间的关系进行数据库的存储
- Non relational DB: MongoDB
    - 对象存储，通过对象的自身属性来决定
- DBMS(数据库的管理软件,维护和获取数据)
    - **MySQL: 数据库管理系统** (开源)

## MySQL Intro
- DDL (数据库**定义**语言)
- DML (数据库**操作**语言)
- DQL (数据库**查询**语言)
- DCL (数据库**控制 controller**语言)

- mysql关键字不区分大小写。在java中，一般都小写
## 连接数据库

## 操作数据库

操作数据库 -> 操作数据库中的**表格** ->操作数据库中的**表的数据**

- 操作数据库 (create，delete，use)
```
CREATE DATABASE IF NOT EXISTS school
CREATE DATABASE school

DROP DATABASE IF EXISTS school
DROP DATABASE school

USE `school`
SELECT `user` from student

SHOW DATABASE school -- 查看数据库
```

- 操作表: 
```
ALTER TABLE teacher RENAME AS teacher1

ALTER TABLE teacher1 ADD age INT(11)

ALTER TABLE teacher1 MODIFY age VARCHAR(11) -- modify data type
ALTER TABLE teacher1 CHANGE age age1 INT(11) -- change name

ALTER TABLE teacher1 DROP age1

-- delete 表
DROP TABLE IF EXIST teacher1
```

## JDBC. Java操作数据库的规范
![01_jdbc]()


