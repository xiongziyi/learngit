mysql 常用命令 
    对数据库的操作  
            use  dbName;
            drop database  dbName;
            create database dbName;
            show databases;
    对表的操作
            create table  tableName (column_Name column_Type)
               举个栗子
                 create table if  tableName(
                      user_id int  unsigned auto_increment,
                      user_name varchar(100) not null,
                      user_password varchar(100) not null,
                      submit_date date,
                      primary key ( user_id)
                       )default charset = utf8;
                 drop table tableName;
              insert into tableName (field1,field2,fieldN) values (value1,value2,value3)
                举个栗子
                  insert into tableName (user_name,user_password ,submit_date) values ("xzy","123",NOW());//主键自增
              drop  table tableName;
              select column_Name1,column_Name2,column_Namen from tableName  where   if one ..
              delete from tableName  where   if one(例如 id>2)
              update tableName  set  field = "重命名"  where  if one (例如 id =2)

