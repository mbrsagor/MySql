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

### How to delete database?
``` DROP DATABASE 'db_name'; ```
 