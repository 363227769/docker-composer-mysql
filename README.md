# docker-composer-mysql

~~~
# 首先创建一个数据库(zqw)
create database zqw;
# 授权zhiqw用户拥有zqw数据库的所有权限，但只能在本地访问。
grant all privileges on zqw.* to 'zhiqw'@localhost identified by '123456';
# 用户可以远程访问zqw数据库 
grant all privileges on zqw.* to 'zhiqw'@'%' identified by '123456'; 
# 刷新系统权限表 
flush privileges;
~~~
