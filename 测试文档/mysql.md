#### 登录命令
mysql -hlocalhost -uroot -p<br/>
回车之后，要求输入密码，输入密码<br/>
登录数据库

#### 查看数据库中有哪些数据库
shows databases;

#### 进入其中某个数据库
use database_name;

#### 查看数据库中有哪些表
show tables;

#### 查看表的注解信息
select table_name,table_comment from information_schema.tables where table_schema="数据库名称" and table_name="表名";

#### 查看某个表的结构
desc table_name;<br/>
这个命令只能展示表的结构，表字段类型，主键信息和该属性是否可为空等属性，而不显示外键信息。

#### 查看其他表中字段更多信息
select column_name,column_default,is_nullable,data_type,collation_name,column_type,column_key,column_comment from information_schema.columns where table_schema="数据库名称" and table_name="表名";

#### 直接删除数据库
drop database name;  删除数据库不会进行提醒

#### 
