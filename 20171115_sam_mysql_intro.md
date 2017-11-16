# MySQL Intro

## Installation and Research

Official MySQL website 
https://www.mysql.com/

Install WAMP if using Windows
http://www.wampserver.com/en/

If using Ubuntu, you can install MySQL via package manager. However I would recommend installing the lamp stack.
` sudo apt-get install lamp`

## Getting Started

Log into MySQL via the command line
```
mysql -uroot -p
```


Create a database
```
create database test_database;
```

View databases
```
show databases;
```

Delete a database
```
drop database test_database;
```

Start Using a Database
```
use test_datebase;
```

Create a table
```
create table users (
  id INT(6) AUTO_INCREMENT PRIMARY KEY,
  username VARCHAR(25),
  email VARCHAR(25)
);
```

Show Tables
```
show tables;
```

Show Table Info
```
explain users;
```

Delete a table
```
drop table users;
```
