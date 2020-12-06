# GoMySQL

## Prerequisites
To Install Go, <a href="https://golang.org/doc/install">click here</a>.<br/><br/>
Add go-mysql dependency, using 
```
go get -u github.com/go-sql-driver/mysql
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

## Build
To build this project, run following command in the project directory (where main file exists).<br/>

`go build .`<br/>

A binary file by the project name would be generated.
 
 ## Testing
 
If there are any test cases in the project, following command can be used to run those test cases.<br/>

`go test ./...`<br/>

## Execution

Once the binary is generated, execute the binary to run the program.<br/>

`./GoMySQL`<br/>

