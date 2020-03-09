spring ,springmvc,mybatis简单整合

1，spring 整合mybatis:
       spring管理mybatis的连接池，sessionFactory
       spring 扫描到dao接口所在包，管理动态代理产生的dao实现类
       使用spring的声明式事务
2,spring 整合spring mvc
      spring容器只管理Repository，Service,Controller由Springmvc容器管理
      注册ServletContext监听，初始化ServletContext时，初始化Springmvc容器，和spring容器



create table account(
id int(11) not null auto_increment,
name varchar(32) not null,
money double  not null,
PRIMARY KEY(id)
)ENGINE=InnoDB DEFAULT CHARSET=utf8;