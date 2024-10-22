# SQL-REPOSITORY

# SQL- Structured query language for querying of Data 
SQL provides a number of operations that enable users to read, manipulate, and alter data. SQL is widely used by engineers in software development, This is important for everybody not only data analyst,data developer, data engineering, database adminstrator use sql. it is used for storing, retriving, managing data,in relational database management system (RDMBS).

## TYPE OF RDMBS
- Mysql
- Postgresql
- Msaccess
- SQL Server , use SQL as their database language
- SQL allows users to query the database in a number of ways, using English statements.
- RDBMS is for storing, querying, retrieving and managing data.

# How database store data in a structure: 
- create table which are composed of rows and columns, each table represent a specific type of data and each row or record in the table represents a single entry.

The columns or field define the attributes of the data , such as a customer's name, age , or account number. Tables in database have rows and columns just like excel.

Database tables for instance are organized by columns, Each column must have a unique name.

# SQL COMMANDS 

- SQL commands are instruction, it is used to communicate with database.
- It is also used to perform various tasks, functions and queries of data.
- it can perform various tasks like create a table, add data to tablets, drop the table, modify the table set permission for users.

  # TO CREATE TABLE
  ```
CREATE TABLE Students (
  StudentID INT PRIMARY KEY,
  FirstName VARCHAR(50) NOT NULL,
  LastName VARCHAR(50) NOT NULL,
  Email VARCHAR(100) UNIQUE,
  DateOfBirth DATE,
  Gender VARCHAR(10),
  Course VARCHAR(50),
  Department VARCHAR(50),
  CreatedAt TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

# Explanation 

- `StudentID`: Unique identifier for each student (Primary Key).
- `FirstName` and `LastName`: Student's name.
- `Email`: Student's email address (Unique constraint).
- `DateOfBirth`: Student's date of birth.
- `Gender`: Student's gender.
- `Course` and `Department`: Student's course and department.
- `CreatedAt`: Timestamp for when the record was created.

 # TYPES OF COMMANDS

## Five type of SQL commnads

- DDL;Data definition language_ is use to change the structure of the table.
- DML:Data manipulation language_ use yo modify database 
- DCL: Data control language_ command are use to grant and take back authority from any database users.
- TCL: Transaction control language _used to manage transactions in the database
- DQL: Data query language_ is used to fetch the data from the database ( select) to retrieve

~~~SQL
  SELECT * FROM TABLE1
  WHERE CONDITION = TRUE
  ~~~
  
SQL Data types
- Binary _ yes or no
- Numeric _ is most widely used datatype in sql ; numeric value only.
- Date or daytime _ are used to be stored in date.

# SQL keys
In sql keys are special field in a table that helps
- create relationship between tables
- mountain uniqueness
- ensure data is consistent and valid

# Databases keys

- foreign key
- primary key
- super key
- candidate key
- surogate key. 


- GITHub for portfolio building

 

  
  ''' SQL'''

  
