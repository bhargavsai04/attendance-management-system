The first step is to create a project in the name you wish. Create a package named “Attendance“. We are creating java classes in this package.

Make sure MySQL is installed on your system.

Download the MySQL connector from https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-j-8.2.0.zip

Open the properties of the project from the dropdown list which appears on right-click on the project. Navigate to the libraries tab and click on the classpath. Select “Add External JARs…”. Select the file you downloaded. This step will differ on IDE you are using.

Mysql Commands:

create database attendance;

use attendance;

CREATE TABLE user(id int primary key, username varchar(25), name varchar(25), password varchar(25), prio int);

CREATE TABLE class(id int primary key, name varchar(25));

CREATE TABLE students(id int primary key, name varchar(25), class varchar(10));

CREATE TABLE teachers(id int primary key, name varchar(25));

CREATE TABLE attend(stid int, dt date, status varchar(15), class varchar(15));

INSERT INTO user VALUES(1, 'admin', 'Admin', 'admin', 1);
