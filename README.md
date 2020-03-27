## MySql tutorial

The tutorial is not for advance user. You may run the command your terminal here all of 'Query' for very basic. I will try to share day by day advance topic and complex query. If have any kind of wrong please forgive me because of I am also learning.

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
    -> first_name varchar(50),
    -> last_name varchar(50),
    -> email varchar(70),
    -> password varchar(50),
    -> address varchar(50),
    -> is_admin TINYINT(1),
    -> register_date DATETIME,
    -> PRIMARY KEY(id)
    -> );
```

### How to `insert` data into table?
``` 
INSERT INTO users(first_name, last_name, email, password, address, is_admin, register_date)
VALUES('mbr', 'sagor', 'mbrsagor@gmail.com', '12345@123', 'Uttara sector#11 road#10/B', 1, date()); 
```

### Show all data
``` SELECT FROM * db_name.users ```

### How to `filter` or query in database?
```
SELECT * FROM WHERE users address='uttara';
```

### How to `filter` or query `multiple` in database?
```
SELECT * FROM WHERE users address='uttara' AND id=1;
```
OR
``` SELECT * FROM WHRE users is_admin >0 ```

### Update table row
```
UDPATE users SET email='brshagor.cse@gmail.com' WHERE ID=1;
```

### How to `Delete` row from the table?
```
DELETE FROM users id=1; 
```

### How to show table column/fields ?
``` SHOW COLUMNS FROM table_name ```

### How to show table?
``` show Tables ```

### How to `alter` table?
```
ALTER TABLE users ADD age varchar(6)
```

### How to modify column?
```
ALTER TABLE users MODIFY COLUMN age INT(6);
```

### Order by ASC
```
SELECT * FROM users ORDER BY email ASC;
```

### Delete table
``` drop table table_name```

### How to delete database?
``` DROP DATABASE 'db_name'; ```

### How to export mysql database?
``` mysqldump -u root -p db_name | gzip > eco.sql.zip ```
 
### How to Import mysql database?
``` mysql -u root -p db_name < ~/Desktop/database/db_name.sql ```
