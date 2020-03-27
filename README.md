## MySql tutorial

### How to create mysql user?
 ```CREATE USER 'Sagor'@'localhost' IDENTIFIED BY '12345';```

 ### List of all users
 ``` 'SELECT user, host FROM mysql.user'; ```

 ### How to exit from `MySql' ?
 Run ``` exit ``` command

### How to create database?

``` CREATE DATABASE 'db_name'; ```

### List of databases
``` show databases; ```

### List of table in the dataase
First select database ```use database_name``` Then ```show tables```

### How to create table?
```CREATE TABLE users (
    -> id INT AUTO_INCREMENT,
    -> fast_name varchar(50),
    -> last_name varchar(50),
    -> email varchar(70),
    -> password varchar(50),
    -> address varchar(50),
    -> is_admin TINYINT(1),
    -> register_date DATETIME,
    -> PRIMARY KEY(id)
    -> );
```

### How to show table?
``` show Tables ```

### Delete table
``` drop table table_name```

### How to delete database?
``` DROP DATABASE 'db_name'; ```
 