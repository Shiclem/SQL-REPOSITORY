# SQL-REPOSITORY

# SQL- Structured query language for querying of Data 

SQL provides a number of operations that enable users to read, manipulate, and alter data. SQL is widely used by engineers in software development, This is important for everybody not only data analyst,data developer, data engineering, database adminstrator use sql. it is used for storing, retriving, managing data,in relational database management system (RDMBS).
..........
# TYPE OF RDMBS
- Mysql
- Postgresql
- Msaccess
- SQL Server , use SQL as their database language
- SQL allows users to query the database in a number of ways, using English statements.
- RDBMS is for storing, querying, retrieving and managing data.
.........
  
## How database store data in a structure: 
- create table which are composed of rows and columns, each table represent a specific type of data and each row or record in the table represents a single entry.

The columns or field define the attributes of the data , such as a customer's name, age , or account number. Tables in database have rows and columns just like excel.

Database tables for instance are organized by columns, Each column must have a unique name.

# SQL COMMANDS 

- SQL commands are instruction, it is used to communicate with database.
- It is also used to perform various tasks, functions and queries of data.
- it can perform various tasks like create a table, add data to tablets, drop the table, modify the table set permission for users.

  # TO CREATE TABLE
  
~~~
CREATE TABLE Students (
  StudentID INT PRIMARY KEY,
  FirstName VARCHAR(50) NOT NULL,
  LastName VARCHAR(50) NOT NULL,
  Email VARCHAR(100) UNIQUE,
  DateOfBirth DATE,
  Gender VARCHAR(10),
  Course VARCHAR(50),
  Department VARCHAR(50),
  CreatedAt TIMESTAMP DEFAULT CURRENT_TIMESTAMP);
~~~
..........

### Explanation 

- `StudentID`: Unique identifier for each student (Primary Key).
- `FirstName` and `LastName`: Student's name.
- `Email`: Student's email address (Unique constraint).
- `DateOfBirth`: Student's date of birth.
- `Gender`: Student's gender.
- `Course` and `Department`: Student's course and department.
- `CreatedAt`: Timestamp for when the record was created.

 # TYPES OF COMMANDS

### Five type of SQL commnads

- DDL;Data definition language_ is use to change the structure of the table.
- DML:Data manipulation language_ use yo modify database 
- DCL: Data control language_ command are use to grant and take back authority from any database users.
- TCL: Transaction control language _used to manage transactions in the database
- DQL: Data query language_ is used to fetch the data from the database ( select) to retrieve

~~~
  SELECT * FROM TABLE1
  WHERE CONDITION = TRUE
~~~
........

# SQL Data types
- Binary _ yes or no
- Numeric _ is most widely used datatype in sql ; numeric value only.
- Date or daytime _ are used to be stored in date.
..........
# SQL keys
In sql keys are special field in a table that helps
- create relationship between tables
- mountain uniqueness
- ensure data is consistent and valid
............
  
# Databases keys

- foreign key
- primary key
- super key
- candidate key
- surogate key.

  primary key must be declare before execute ( syntax word is identity)
  Identity - Auto create increasing the primary key.
  decimal - is to store exact numerical value.
...........
  
  # GROUP BY`
  is a clause used to:
- Divide data into groups based on one or more columns.
-  Aggregate data within each group.

## Purpose

- Summarize data
- Perform calculations on groups
- Identify trends and patterns

### Syntax

`SELECT column1, column2, ...`
`FROM tablename`
`GROUP BY column1, column2, ...;`

### How it works

- SQL selects data from the table.
- Groups data based on specified columns.
- Applies aggregate functions (e.g., SUM, COUNT, AVG) to each group.

### Common aggregate functions

- SUM
- COUNT
- AVG (average)
- MAX
- MIN
- GROUPING SETS

### Example

`SELECT Department, AVG(Salary) AS AverageSalary`
`FROM Employees`
`GROUP BY Department;`

### Result

| Department | AverageSalary |
| --- | --- |
| Sales | 50000 |
| Marketing | 60000 |
| IT | 70000 |
........

### Having 

HAVING is a clause used to:

- Filter groups based on aggregate conditions.
- Apply conditions to grouped data.

### Syntax

`SELECT column1, column2, ...`
`FROM tablename`
`GROUP BY column1, column2, ...`
`HAVING condition;`

### purpose

- Filter groups based on aggregate values (e.g., SUM, COUNT, AVG).
- Narrow down results to specific groups.

### Examples

- Filter groups with average salary > 50000:

`SELECT Department, AVG(Salary) AS AverageSalary`
`FROM Employees`
`GROUP BY Department`
`HAVING AVG(Salary) > 50000;`

Find departments with > 5 employees:

`SELECT Department, COUNT(*) AS EmployeeCount`
`FROM Employees`
`GROUP BY Department`
`HAVING COUNT(*) > 5;
.........

### order by 
Ascending and descending order. 

### union 
remove duplicate 

### union all 
execute all with duplicate 

### comparison relation operator
<= less than 

>= greater than

<> not equal
...........

### To join table 
Inner join 
Left join 
Right join 
Full join 
This has to do with joining multiple tables to return in a single columns. 
...........

# SQL view 

virtual table, that is created based on the result set of a sql query. 

### Creating a View

`CREATE VIEW view_name AS`
`SELECT column1, column2, ...`
`FROM tablename;`

### Example

`CREATE VIEW EmployeeInfo AS`
`SELECT FirstName, LastName, Department`
`FROM Employees;`
..........

### CASE WHEN STATEMENT 

Conditional expression that allow to create different output based on certain condition. 

### Syntax

`CASE`
`WHEN condition1 THEN result1`
`WHEN condition2 THEN result2`
`...`
`ELSE default_result`
`END`

### Formula Logic

- Evaluate conditions from top to bottom.
- Return result for first true condition.
- If no conditions are true, return default_result (ELSE clause).

### Key points 
- Flexibility
- Readability
- Efficiency 




  
