# GoMySQL

## Prerequisites
To Install Go, <a href="https://golang.org/doc/install">click here</a>.<br/><br/>
Add go-mysql dependency, using 
```
go get -u github.com/go-sql-driver/mysql
```
Add error package , using 
```
go get -u github.com/pkg/errors
```
Create required schema.<br/>
```
CREATE DATABASE student;
USE student;
CREATE TABLE IF NOT EXISTS student(
    id INT(11) NOT NULL AUTO_INCREMENT, 
    name VARCHAR(50) DEFAULT NULL,
    age INT(11) DEFAULT 0,
    UNIQUE KEY(id),
    PRIMARY KEY(id)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```


