# MYSQL
<br>

![image My-Sql](images/My-sql.png)

## Introduction to MySQL
<br>

![Introduction](images/Introduction.png)
<br>


<div style="font-size:20px; text-align:justify;"> 

{{1}} [What is Database](#what-is-database)

{{2}} [What is MySQL](#what-is-mysql)

{{3}} [What is MySQL RDMS](#mysql-rdbms)

{{4}} [MySQL SQL](#mysql-sql)

{{5}} [WorkBench Installation](#installation-of-mysql-workbench)

</div>

### What is Database 
<br>

* A database is an organized collection of structured information, or data, typically stored electronically in a computer system. 

* Databases make data management easy

* A database is usually controlled by a database management system (DBMS).
<br>

![image data-base](images/Database.png)
<br>


### What is MySQL  
<br>

* MySQL is a relational database management system

* MySQL is free and open-source.

* MySQL is ideal for both small and large applications

* MySQL is very fast, reliable, scalable, and easy to use

* MySQL is cross-platform

* MySQL is compliant with the ANSI SQL standard
<br>

**Who Uses MySQL**

<br>

* Huge websites like Facebook, Twitter, Airbnb, Booking.com, Uber, GitHub, YouTube, etc.

* Content Management Systems like WordPress, Drupal, Joomla!, Contao, etc.

* A very large number of web developers around the world

### MySQL RDBMS
<br>

**What is RDBMS**

* RDBMS stands for Relational Database Management System.

* RDBMS is a program used to create, update, and manage relational databases.

* Some of the most well-known RDBMSs include MySQL, PostgreSQL, MariaDB, Microsoft SQL Server, and Oracle Database.

* RDBMS uses SQL queries to access the data in the database.
<br>

![image RDBMS-data-base](images/RDBMS.png)"A relational database defines database relationships in the form of tables. The tables are related to each other - based on data common to each. Look at the following two tables "Customers" and "Orders",The relationship between the "Customers" table and the "Orders" table is the CustomerID column"
<br>

### MySQL SQL
<br>

**What is SQL**

* SQL is used to communicate with a database.

* According to ANSI (American National Standards Institute), it is the standard language for relational database management systems.

* SQL statements are used to perform tasks such as update data on a database or retrieving data from a database.

<br>
**Some of The Most Important SQL Commands** :

* SELECT - extracts data from a database
* UPDATE - updates data in a database
* DELETE - deletes data from a database
* INSERT INTO - inserts new data into a database
* CREATE DATABASE - creates a new database
* ALTER DATABASE - modifies a database
* CREATE TABLE - creates a new table
* ALTER TABLE - modifies a table
* DROP TABLE - deletes a table
* CREATE INDEX - creates an index (search key)
* DROP INDEX - deletes an index

### Installation of MySQL WorkBench

**Steps to install MySQL**:

{{1-7}} 
> **Step 1**: Click on the link : (https://dev.mysql.com/downloads/)

{{2-7}} 
> **Step 2**: Select MySQL Installer for Windows 
>![image MySQL Installer for Windows](/images/mySQL-Installer.png)

{{3-7}} 
> **Step 3**: Download MySQL Installer web community 2.4 M 
>![image MySQL Installer for Windows ](/images/mySQL-Installer-version.png)

{{4-7}} 
> **Step 4**: click on No thanks, just start my download.
>![image MySQL Installer for Windows ](/images/mySQL-Installer-version-nothanks.png)

{{5-7}} 
> **Step 5**: click on the downloaded file.

{{6-7}}
> **Step 6**: setting up the Workbench
>(https://www.youtube.com/watch?v=YSOY_NyOg40)




## Data Types
<br>
An SQL developer must decide what type of data will be stored inside each column when creating a table. The data type is a guideline for SQL to understand what type of data is expected inside of each column, and it also identifies how SQL will interact with the stored data.

<br>
In MySQL there are three main data types: text, number, and date and time.

* [Text data types](#text-data-types)

* [Number data Types](#number-data-types)

* [Date data types](#date-data-types)

<br>

![image MySQL datatypes ](/images/datatypes.png)
<br>

###	Text data types

<br>

| **_Data Type_** | **_Description_**                          |
|-----------------|--------------------------------------------|
|CHAR(size)       |Holds a fixed length string (can contain letters, numbers, and special characters). The fixed size is specified in parenthesis.Can store up to 255 characters|
|VARCHAR(size)    |Holds a variable length string (can contain letters, numbers, and special characters). The maximum size is specified in parenthesis.Can store up to 255 characters. Note: If you put a greater value than 255 it will be converted to a TEXT type|
|TINYTEXT         |Holds a string with a maximum length of 255 characters|
|TEXT             |Holds a string with a maximum length of 65,535 characters|
|BLOB             |For BLOBs (Binary Large OBjects). Holds up to 65,535 bytes of data|
|MEDIUMTEXT       |Holds a string with a maximum length of 16,777,215 characters|
|MEDIUMBLOB       |For BLOBs (Binary Large OBjects). Holds up to 16,777,215 bytes of data|
|LONGTEXT         |Holds a string with a maximum length of 4,294,967,295 characters|
|LONGBLOB         |For BLOBs (Binary Large OBjects). Holds up to 4,294,967,295 bytes of data|



###	Number data Types
<br>

<!-- data-transpose data-type="none" -->
| **_Data Type_** | **_Description_**                          | **_Lower limit_**                   | **_Upper limit_**                    | **_Memory_**       |
|-----------------|--------------------------------------------|-------------------------------------|--------------------------------------|--------------------|
| bigint          | It stores whole numbers in the range given | −2^63 (−9,223,372, 036,854,775,808) | 2^63−1 (9,223,372, 036,854,775,807)  | 8 bytes            |
| int             | It stores whole numbers in the range given | −2^31 (−2,147, 483,648)             | 2^31−1 (2,147, 483,647)              | 4 bytes            |
| smallint        | It stores whole numbers in the range given | −2^15 (−32,767)                     | 2^15 (32,768)                        | 2 bytes            |
| tinyint         | It stores whole numbers in the range given | 0                                   | 255                                  | 1 byte             |
| decimal         | Used for scale and fixed precision numbers | −10^38+1                            | 10^381−1                             | 5 to 17 bytes      |
| float           | Used for a floating precision number       | −1.79E+308                          | 1.79E+308                            | 7 bytes            |
| double          | A large number with a floating decimal point| −3.40E+38                          | −3.40E+38                            | 15 bytes           |
| meduimint       | It stores whole numbers in the range given  | −8,388,608                           | +8,388,608                         | 3 bytes            |

###	Date data types


| **_Data Type_** | **_Description_**                          |
|-----------------|--------------------------------------------|
|DATE()           |A date. Format: YYYY-MM-DD **Note**: The supported range is from '1000-01-01' to '9999-12-31'|
|DATETIME()       |A date and time combination. Format: YYYY-MM-DD HH:MI:SS **Note**: The supported range is from '1000-01-01 00:00:00' to '9999-12-31 23:59:59'|
|TIMESTAMP()      |A timestamp. TIMESTAMP values are stored as the number of seconds since the Unix epoch ('1970-01-01 00:00:00' UTC). Format: YYYY-MM-DD HH:MI:SS **Note**: The supported range is from '1970-01-01 00:00:01' UTC to '2038-01-09 03:14:07' UTC|
|TIME()           |A time. Format: HH:MI:SS **Note**: The supported range is from '-838:59:59' to '838:59:59'|
|YEAR()           |A year in two-digit or four-digit format.**Note**: Values allowed in four-digit format: 1901 to 2155. Values allowed in two-digit format: 70 to 69, representing years from 1970 to 2069|


## Constraints

* MySQL CONSTRAINT is used to define rules to allow or restrict what values can be stored in columns. The purpose of inducing constraints is to enforce the integrity of a database.

* MySQL CONSTRAINTS are used to limit the type of data that can be inserted into a table.

* MySQL CONSTRAINTS can be classified into two types - column level and table level.

* The column-level constraints can apply only to one column where as table-level constraints are applied to the entire table.

* MySQL CONSTRAINT is declared at the time of creating a table.

**MySQL CONSTRAINTs are** : 

* [NOT NULL](#not-null)

* [UNIQUE](#unique)

* [PRIMARY KEY](#primary-key)

* [FOREIGN KEY](#foreign-key)

* [DEFAULT](#default)

### NOT NULL

* The NOT NULL constraint enforces a column to NOT accept NULL values.

* This enforces a field to always contain a value, which means that you cannot insert a new record, or update a record without adding a value to this field.

**Not NULL on Creating a Table**:-

```markdown

CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int
);
```
**Output**:

![image not null ](images/Not-Null.png)
### UNIQUE

* The UNIQUE constraint ensures that all values in a column are different.

* Both the UNIQUE and PRIMARY KEY constraints provide a guarantee for uniqueness for a column or set of columns.

* A PRIMARY KEY constraint automatically has a UNIQUE constraint.

* However, you can have many UNIQUE constraints per table, but only one PRIMARY KEY constraint per table.

```markdown

CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
    UNIQUE (ID)
);

```

**Output**:

![image- Unique-id ](images/Unique-id.png)

#### Multiple Unique Constraints

* To name a UNIQUE constraint, and to define a UNIQUE constraint on multiple columns, use the following SQL syntax

```markdown

CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
    CONSTRAINT UC_Employee UNIQUE (ID,LastName)
);
```

**Output**:

![image multiple unique  ](images/mulitiple-unique.png)




#### Unique Constraints on Alter Table

* To create a UNIQUE constraint on the "ID" & "LastName" column when the table is already created, use the following SQL

```markdown

ALTER TABLE Employee
ADD CONSTRAINT UC_Employee UNIQUE (ID,LastName);


```

**Output**:

![image Alter multiple unique  ](images/Alter-uniqueKey.png)


#### Drop a Unique  Constraint

To drop a UNIQUE constraint, use the following MySQL:

```markdown

ALTER TABLE Employee
DROP INDEX UC_Employee;

```

**Output**:

![image drop ](images/drop-unique.png)


### PRIMARY KEY

* The PRIMARY KEY constraint uniquely identifies each record in a table.

* Primary keys must contain UNIQUE values, and cannot contain NULL values.

* A table can have only ONE primary key; and in the table, this primary key can consist of single or multiple columns (fields).

```markdown

CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
    PRIMARY KEY (ID)
);

```
**Output**:

![image primary-key ](images/primary-key.png)

#### Multiple Primary Constraints

To allow naming of a PRIMARY KEY constraint, and for defining a PRIMARY KEY constraint on multiple columns, use the following SQL syntax:

```markdown
CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
   CONSTRAINT PK_Employee PRIMARY KEY (ID,LastName)
);

```
**Output**:

![image multiple-primary-key ](images/mulitiple-primary.png)

#### primary Constraints on Alter Table

To create a PRIMARY KEY constraint on the "ID" column when the table is already created, use the following SQL:

```markdown
ALTER TABLE Employee
ADD PRIMARY KEY (ID);

```


**Output**:

![image alter-primary-key ](images/alter-pk.png)

#### Drop a primary  Constraint

To drop a PRIMARY KEY constraint, use the following MySQL:

```markdown
ALTER TABLE Employee
DROP PRIMARY KEY;

```
**Output**:

![image drop-primary-key ](images/drop-pk.png)


### FOREIGN KEY

* The FOREIGN KEY constraint is used to prevent actions that would destroy links between tables.

* A FOREIGN KEY is a field (or collection of fields) in one table, that refers to the PRIMARY KEY in another table.

* The table with the foreign key is called the child table, and the table with the primary key is called the referenced or parent table.

**Employee Table**:-

| **_EmployeeID_** | **_FirstName_**|**_LastName_**   | **_Age_** |
|------------------|----------------|-----------------|-----------|
| 1                | texas          | John            | 26        |
| 2                | Phoenix        | justin          | 25        |
| 3                | SpaceX         | elon            | 28        |


**Salary**:

| **_SalaryID_** | **_Salary_** | **_EmployeeID_** |
|----------------|--------------|------------------|
| 1              | 65000$       | 1                |
| 2              | 45000$       | 2                |
| 3              | 50000$       | 3                |

* Notice that the "EmployeeID" column in the "Salary" table points to the "EmployeeID" column in the "Employee" table.

* The "EmployeeID" column in the "Employee" table is the PRIMARY KEY in the "Employee" table.

* The "EmployeeID" column in the "Salary" table is a FOREIGN KEY in the "Salary" table.

* The FOREIGN KEY constraint prevents invalid data from being inserted into the foreign key column, because it has to be one of the values contained in the parent table.

#### Create Foreign key

```markdown
CREATE TABLE Salary (
    SalaryID int NOT NULL,
    Salary int NOT NULL,
    EmployeeID int,
    PRIMARY KEY (SalaryID),
    FOREIGN KEY (EmployeeID) REFERENCES Employee(ID)
);
```


**Output**:

![image foreign-key ](images/foreign-key.png)

#### foreign Constraints on Alter Table

```markdown
ALTER TABLE Salary
ADD FOREIGN KEY (EmployeeID) REFERENCES Employee(ID);

```
**Output**:

![image alter-foreign-key ](images/alter-fk.png)


#### Drop a foreign  Constraint

```
ALTER TABLE Salary
DROP FOREIGN KEY FK_EmployeeSalary;

```

**Output**:

![image drop-foreign-key ](images/drop-fk.png)


### DEFAULT

The following SQL sets a DEFAULT value for the "City" column when the "Persons" table is created:

```markdown

CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
    City varchar(255) DEFAULT 'US'
);

```

**Output**:

![image default ](images/default.png)




## Data Definition Language(DDL)

A data definition language (DDL) is a computer language used to create and modify the structure of database objects in a database. These database objects include views, schemas, tables, indexes, etc.

**Data Definition Laungauge Commands are as follows**

1. [CREATE](#create-command) 

2. [ALTER](#alter-command)

3. [DROP](#drop-command)

4. [TRUNCATE](#truncate-command)

### Create Command

create is a DDL SQL command used to create a table in a relational database management system.
The table creation command requires the following details −

*	Name of the table

*	Name of the fields(Column) 

*	Definitions for each field(Datatype)

Syntax:

```
/* to create database */
    CREATE DATABASE database_name;

    /* to create schema */
    CREATE SCHEMA schema_name;

    /* to create table */
CREATE TABLE <TABLE_NAME> 
	( 
		column_name1 datatype1, 
		column_name2 datatype2, 
		column_name3 datatype3, 
		column_name4 datatype4 
	);

```
Create Command Example

```
/* to create database */
CREATE DATABASE EmployeeManagement;

/* to create schema */
CREATE SCHEMA Employees;

/* to create table */
CREATE TABLE Employee (
    ID int NOT NULL,
    FirstName varchar(255) NOT NULL,
    LastName varchar(255) NOT NULL,
    Age int ,
   CONSTRAINT PK_Employee PRIMARY KEY (ID,LastName)
);
```
Output:

![image create ](images/create.png)

### Alter Command

Alter statement is used to add, delete or modify columns in an exisiting table

*	Add column

The basic syntax of an ALTER TABLE command to add a New Column in an existing table is as follows

Syntax:

```
    ALTER  TABLE table_name
	ADD column_name datatype;
```

Example:

```
ALTER TABLE Employee
ADD Email varchar(255);
```

Output:
![image Alter-table ](images/Alter-table.png)

#### Modify column

The basic syntax of an ALTER TABLE command to change the DATA TYPE of a column in a table is as follows.

Syntax:

```
ALTER  TABLE  table_name 
ALTER  COLUMN column_name  datatype;

```

Example:

```
ALTER TABLE Employee
ADD DateOfBirth date;

ALTER TABLE Employee
MODIFY COLUMN DateOfBirth year;

```

Output:
![image Alter-modify ](images/Alter-modify.png)

#### Delete column

The basic syntax of an ALTER TABLE command to DROP COLUMN in an existing table is as follows.

Syntax:

```
ALTER  TABLE table_name 
DROP  COLUMN column_name;

```

Example:

```
ALTER TABLE Employee
DROP COLUMN DateOfBirth;

```

Output:
![image Drop-column ](images/drop-column.png)


### Drop Command

It is very easy to drop an existing MySQL table, but you need to be very careful while deleting any existing table because the data lost will not be recovered after deleting a table. 

Syntax:

```
DROP  TABLE  table_name;

```

Example:

```
DROP TABLE Employee


```

Output:

![image Drop-table ](images/drop-table.png)

### Truncate Command

TRUNCATE command removes all the records from a table. But this command will not destroy the table's structure.

Syntax:

```
TRUNCATE TABLE table_name ;
```

Example:

```

TRUNCATE TABLE Employee ;

```
Output:

![image truncate ](images/truncate-table.png)


## Data Manipulation Lanaguage(DML)

The DML commands in Structured Query Language change the data present in the SQL database. We can easily access, store, modify, update and delete the existing records from the database using DML commands.

DML Commands are :

* [Insert Command](#insert-command)

* [Update Command](#update-command)

* [Delete Command](#delete-command)

### Insert Command

* The SQL INSERT INTO Statement is used to add new rows of data to a table in the database.

* Only one row is inserted with this syntax.

* Insert a new row containing values for each column.

* List values in the default order of the columns in the table.

* Optionally, list the columns in the insert clause.

* Enclose character and data values within single quotation marks.

It is possible to write the INSERT INTO statement in two ways:

1. Specify both the column names and the values to be inserted:

Syntax:

```
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);

```

2. If you are adding values for all the columns of the table, you do not need to specify the column names in the SQL query. However, make sure the order of the values is in the same order as the columns in the table. Here, the INSERT INTO syntax would be as follows:

```
INSERT INTO table_name VALUES (value1, value2, value3, ...);
```

Example:

```
INSERT INTO Employee (ID,FirstName, LastName, Age)
VALUES (1,'Cardinal', 'Tom B. Erichsen', 21);

```

Output:

![image insert ](images/insert.png)

### Update Command

* The UPDATE Query is used to modify the existing records in a table.

* You can use the WHERE clause with the UPDATE query to update the selected rows, otherwise, all the rows would be affected.


Syntax:

```
UPDATE table_name 
SET column1 = value1, column2 = value2...., columnN = valueN 
WHERE [condition];

```
Example:

```
UPDATE Employee
SET FirstName = 'Alfred', LastName = 'Schmidt'
WHERE ID = 1;

```
Output:

![image update ](images/update.png)



### Delete Command

* The SQL DELETE Query is used to delete the existing records from a table.
* You can use the WHERE clause with a DELETE query to delete the selected rows, otherwise all the records would be deleted. 

Syntax:

```
DELETE FROM table_name 
WHERE [condition];

```
Example:

```
DELETE FROM Employee WHERE  ID = 1;

```

Output:

![image delete ](images/delete.png)


## Data Control Language

It is used to control privileges in Database. To perform any operation in the database, such as for creating tables, sequences or views, a user needs privileges.

The DCL statements are

1. [GRANT](#grant-command)

2. [REVOKE](#revoke-command)

### Grant Command

* It is used to provide any user access privileges or other privileges for the database

Syntax:

```
/* Grant read only to a User */
GRANT SELECT ON table_name TO user_name;

/* Grant insert,update,delete & select function to a user */
GRANT INSERT, UPDATE, DELETE, SELECT ON table_name TO user_name;

```

Example:

```

CREATE USER john@localhost IDENTIFIED BY 'jtp12345';

GRANT ALL ON employee.* TO john@localhost;

```


Output:

![image grant ](images/grant.png)


### Revoke Command

* It is used to take back the privileges from any user, use the REVOKE command.

Syntax:

```
REVOKE privilege_name(s)   
ON object   
FROM user_account_name;  

```
Example:

```
REVOKE ALL, GRANT OPTION FROM john@localhost;  

```

Output:

![image revoke ](images/revoke.png)


## Transaction Control Lanaguage(TCL)

Database Transactions:

A transaction begins with the first statement is encounterd and ends when one of the following occurs.This command is used to manage changes to DML statements.

* A commit or rollback statement is issued.

* A DDL statement, such as create is issued.

* A DCL statement is issued.

* The system crashes.

* After one transaction ends, the next executable SQL statement automatically starts the next transaction.

* A DDL statement or a DCL statement is automatically committed and therefore implicitly ends a transaction.

You can control the logic of transactions by using the

1. [Commit](#commit)

2. [Savepoint](#savepoint)

3. [Rollback](#rollback)

### Commit

* COMMIT command is used to permanently save any transaction into the database.

* When we use any DML command like INSERT, UPDATE or DELETE, the changes made by these commands are not permanent, until the current session is closed, the changes made by these commands can be rolled back.

* To avoid that, we use the COMMIT command to mark the changes as permanent.

Syntax:

```
COMMIT;

```

Example:

```
COMMIT;
```

Output:

![image commit ](images/commit.png)


### Savepoint

*	SAVEPOINT command is used to temporarily save a transaction so that you can rollback to that point whenever required.

Syntax:

```
	SAVEPOINT savepoint_name;

```

Example:

```

	SAVEPOINT transactionA;


```
Output:

![image savepoint ](images/savepoint.png)



### Rollback

* This command restores the database to last commited state. It is also used with SAVEPOINT command to jump to a savepoint in an ongoing transaction.
* If we have used the UPDATE command to make some changes into the database, and realise that those changes were not required, then we can use the ROLLBACK command to rollback those changes, if they were not commited using the COMMIT command.

Syntax:

```
ROLLBACK savepoint_name;
```

Example:

```
ROLLBACK to transactionA;

```
Output:

![image rollback ](images/rollback.png)


### Example for Commit, Savepoint and RollBack

```
create table student(id INT,name VARCHAR(20));
start transaction;
select * from student;
insert into student values(10,'Dravid');
savepoint transactionInsert;
insert into student values(20,'Sachin');
insert into student values(30,'Dhoni');
insert into student values(40,'kohli');
select * from student;
savepoint transactionDelete;
delete from student where id=10;
delete from student where id=20;
select * from student;
rollback to transactionDelete;
select * from student;
rollback to transactionDelete;
select * from student;
rollback;
select * from student;

```
Output:

![image com-sav-rol ](images/com-sav-rol.png)



## Data Query/Retrieval Language (DQL/DRL)

SELECT statement is used to retrieve the information from database using select statement you can do the following

* Projection: It is used to choose columns in a table that you want returned by the query.

* Selection: It is used to choose rows in a table that you want returned by your query.

* Joining: You can choose the join capability in SQL to bring together data that is stored in different tables by creating a link between them.

Syntax:

```
SELECT column1, column2, ...FROM table_name;

/* select all the fields available in the table */
SELECT * FROM table_name;

```

Example:

```
SELECT * FROM employee;

SELECT Id,first_name,last_name FROM employee.employees;

```

output:

![image select ](images/Select.png)

### Arithmetic Expressions

* Create expressions with number and date data by using arithematic operators

* Operator Precedence : * , / , + , -

* If the operators within an expression are of same priority then evaluation is done from left to right.

Example:

```
SELECT ID,FirstName,LastName,salary,(20*salary-100)/2 FROM employee;

```

output:

![image Arithmetic ](images/Arithmetic.png)

### column aliases

* Renames column heading

* It is useful for calculations

* Immediately followed by the column name, there can also be optional keyword AS keyword betweeen the column name and alias.

* Enclose alias name in double quotations if it contains a special characters such as # or $ or is case sensitive.

* Column aliases can be used in both select clause and the order by clause you cannot use column aliases in where clause.

Syntax:

```
SELECT column_name AS alias_name
FROM table_name;

```
Example:

```
SELECT ID AS EmployeeID, FirstName  AS EmployeeName
FROM employee;
```

Output:

![image Aliases ](images/alias.png)

### Clause

1. [DISTINCT](#distinct)

2. [WHERE](#where)

3. [ORDER BY](#order-by)

4. [GROUP BY](#group-by)

5. [HAVING](#having)

#### DISTINCT

* The SQL DISTINCT keyword is used in conjunction with the SELECT statement to eliminate all the duplicate records and fetching only unique records.

* There may be a situation when you have multiple duplicate records in a table. While fetching such records, it makes more sense to fetch only those unique records instead of fetching duplicate records and can be used for more than one column

* Distinct keyword should be used immediately after the select keyword.

* Distinct can also be used with multiple columns and it affects all the columns selected

Syntax

```
SELECT DISTINCT column1, column2,.....columnN 
FROM table_name  WHERE [condition]
```

Example:

```
SELECT DISTINCT FirstName  
FROM employee; 

```

Output:

![image distinct ](images/distinct.png)

#### WHERE

* We restrict the rows returned by using the WHERE clause.

* Where restricts the query to rows that meets the condition

* Condition is composed of column names ,expressions constants ,and a comparison operator.

* Where consists of three elements.

1. column name 

2. comparison condition 

3. column name, constant or list of values

* Character strings and date values are enclosed in single quotation marks.

* The WHERE clause is not only used in the SELECT statement, but it is also used in the UPDATE, DELETE statement, etc.,


Syntax:

```	
	SELECT column1, column2,.....columnN 
FROM table_name 
WHERE [condition]

```

Example:

```
SELECT * FROM employee
WHERE ID = 1;

```


Output:

![image where ](images/where.png)


#### ORDER BY

* We sort rows by using order by clause .

1. ASC: ascending order , default

2. DSC: descending order.

* The order by clause comes last in the select statement.

* Order by clause is executed last in the query execution .it is placed last unless the for update clause is used.

* Default sorting is ascending

* Numeric values are displayed with lowest values first ex: 1-999

* Date values are displayed with earliest value first ex: 01-jan-92 before 01-jan-95.

* Character values are displayed in alphabetic order ex: A-Z.

* Null values are displayed last for ascending sequences and first for descending sequences.

* We can also sort by a column number in the select list.

Syntax:

```
SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;

```

Example:

```
SELECT * FROM employee
ORDER BY salary;

```

Output:

![image order by ](images/order-by.png)


##### ORDER BY DESC


Syntax:

```
SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;

```

Example:

```

SELECT * FROM employee
ORDER BY salary DESC;

```

Output:

![image order by Desc ](images/Desc.png)


#### GROUP BY

* We use GROUP BY clause to divide the rows in a table into groups.

* If you include a group function in a select statement, you cannot select individual results as well ,unless the individual column appears in the GROUP BY clause.

* Using WHERE clause you can include rows before dividing them into groups.

* You must include the columns in the GROUP BY clause.

* You cannot use a column alias in the GROUP BY clause.

* By default, rows are sorted by ascending order of the columns included in the group by list. You can override this by using ORDER BY clause.

* You cannot use WHERE clause to restrict groups

Syntax:

```
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
ORDER BY column_name(s);

```

Example:

```
SELECT COUNT(ID), FirstName
FROM employee
GROUP BY FirstName
ORDER BY COUNT(ID) DESC;

```
Output:

![image Group by Desc ](images/group-by.png)


#### HAVING

* The HAVING Clause enables you to specify conditions that filter which group results appear in the results.

* The WHERE clause places conditions on the selected columns, whereas the HAVING clause places conditions on groups created by the GROUP BY clause.

* The HAVING clause must follow the GROUP BY clause in a query and must also precede the ORDER BY clause if used.

Syntax:

```
SELECT column_name(s)
FROM table_name
WHERE condition
GROUP BY column_name(s)
HAVING condition
ORDER BY column_name(s);

```

Example:

```
SELECT COUNT(ID), salary
FROM employee
GROUP BY salary
HAVING COUNT(ID) > 1
ORDER BY COUNT(ID) DESC;

```
Output:

![image having ](images/Having.png)

### Logical conditions

<br>

| **_Operator_**        | **_Meaning_**                                                 |
|-----------------------|---------------------------------------------------------------|
|     AND               |     Returns true if both component conditions   are true      |
|     OR                |     Returns true if either component conditions   are true    |
|     NOT               |     Returns true if false, Returns false if   true            |

<br>

1. AND

Example:

```

SELECT * FROM employee
WHERE FirstName = "nick" AND salary = 2500;

```

Output:

![image and ](images/and.png)

2. OR

Example:

```
SELECT * FROM employee
WHERE FirstName = "nick" OR salary = 2500;

```

Output:

![image OR ](images/OR.png)

3. NOT

Example:

```
SELECT * FROM employee
WHERE FirstName NOT LIKE 's%';

```

Output:

![image Not ](images/NOT.png)

### Comparision conditions


| **_Operator_**  | **_Meaning_**                   |
|-----------------|---------------------------------|
|     =           |     Equal to                    |
|      >          |     Greater than                |
|     >=          |     Greater than or Equal to    |
|     <           |     Less than                   |
|     <=          |     Less than or Equal to       |
|     <>,!=,^=    |     Not equal to                |

Example:

```
SELECT * FROM employee
WHERE salary > 2500;

```

Output:

![image greater-then ](images/greater-than.png)

### Other Comparision operator

* [**BETWEEN AND**](#between-and)
* [**IN**](#in)
* [**LIKE**](#like)
* [**IS NULL**](#is-null)

#### BETWEEN AND

* BETWEEN and AND are actually translated by the sql server server to a pair of AND conditions (a>=lower limit) AND (a⇐ higher limit).

* Using BETWEEN AND has no performance benefits, and it is used logical simplicity.

Example:

```
SELECT * FROM employee
WHERE salary BETWEEN 2000 AND 25000;

```

Output:

![image between ](images/between.png)


#### IN

* It is used to test the values in a list. IN condition is also known as member ship condition

* If characters or dates are used in a list they must be enclosed in a single quotation marks .

* IN is actually translated by a sql server to a set of OR conditions a=value1 or a= value2 or a=value3.

* Using IN has no performance benefits ,and is used for logical simplicity.

Example:

```
SELECT * FROM employee
WHERE City IN ('Paris','London');

```

Output:

![image IN ](images/IN.png)


#### LIKE

* It is used for performing wildcard searches of valid search string values.

* Search conditions can contain either literal characters or numbers .

* % denotes zero or many characters .

* _ denotes one character or any single character.


Example:

```
SELECT * FROM employee
WHERE FirstName LIKE 'e%';

```

Output:

![image like ](images/like.png)


#### IS NULL

Example

```
SELECT FirstName,LastName,salary,City FROM employee WHERE salary IS NULL;

SELECT FirstName,LastName,salary,City FROM employee WHERE salary IS  NOT NULL;

```

Output:

![image not-null ](images/not-nu.png)

## Joins

SQL Server (Transact-SQL) JOINS are used to retrieve data from multiple tables. A SQL Server JOIN is performed whenever two or more tables are joined in a SQL statement.

There are 2 different types of SQL Server joins:

1. [INNER JOIN](#inner-join)

2. [OUTER JOIN](#outer-join)

* Left Join

* Right Join

3. [CROSS JOIN](#cross-join)

### INNER JOIN

The INNER JOIN keyword selects records that have matching values in both tables.

Syntax:

```
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name = table2.column_name;

```

Table:

```
CREATE TABLE EmployeeDetails (
    EmployeeDetailsID int NOT NULL,
    ID int NOT NULL,
    Address varchar(255) NOT NULL,
    City varchar(255) NOT NULL , 
    PRIMARY KEY (EmployeeDetailsID),
    FOREIGN KEY (ID) REFERENCES Employee(ID)
);

```

Example:

```
SELECT EmployeeDetails.EmployeeDetailsID, employee.FirstName
FROM EmployeeDetails
INNER JOIN employee ON EmployeeDetails.ID = employee.ID;

```

Output:

![image inner-join ](images/Inner-join.png)



### OUTER JOIN 

**LEFT JOIN**

The LEFT JOIN keyword returns all records from the left table (table1), and the matching records from the right table (table2). The result is 0 records from the right side, if there is no match

Syntax:

```
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name = table2.column_name;

```

Example:

```
SELECT employee.FirstName, EmployeeDetails.EmployeeDetailsID
FROM employee
LEFT JOIN EmployeeDetails ON employee.ID = EmployeeDetails.ID
ORDER BY employee.FirstName;

```


Output:

![image left-join ](images/Left-join.png)


#### RIGHT JOIN

The RIGHT JOIN keyword returns all records from the right table (table2), and the matching records from the left table (table1). The result is 0 records from the left side, if there is no match.

Syntax:

```
SELECT column_name(s)
FROM table1
RIGHT JOIN table2
ON table1.column_name = table2.column_name;
```
Example:

```
SELECT EmployeeDetails.EmployeeDetailsID, employee.LastName, employee.FirstName
FROM EmployeeDetails
RIGHT JOIN employee ON EmployeeDetails.ID = employee.ID
ORDER BY EmployeeDetails.EmployeeDetailsID;

```


Output:

![image right-join ](images/right-join.png)

### CROSS JOIN

The CROSS JOIN keyword returns all matching records from both tables whether the other table matches or not. So, if there are rows in "employee" that do not have matches in "EmployeeDetails", or if there are rows in "EmployeeDetails" that do not have matches in "employee", those rows will be listed as well.

Syntax:

```
SELECT column_name(s)
FROM table1
CROSS JOIN table2;
```

Example:

```
SELECT employee.FirstName, EmployeeDetails.EmployeeDetailsID
FROM employee
CROSS JOIN EmployeeDetails;

```

Output:

![image cross-join ](images/cross-join.png)

## MySQL Functions

Functions in SQL Server are the database objects that contains a set of SQL statements to perform a specific task. A function accepts input parameters, perform actions, and then return the result.

Different types of sql server functions are as follows

1. String Functions

2. Number Funtions

3. Date Functions


### String Functions

SQL string functions are used primarily for string manipulation.

The following table listed each of the functions with a brief description:


| Function         | Description                                                                                       |
|------------------|---------------------------------------------------------------------------------------------------|
| ASCII            | Returns the ASCII value for the specific character                                                |
| CHAR_LENGTH      | Returns the length of a string (in characters)                                                    |
| CHARACTER_LENGTH | Returns the length of a string (in characters)                                                    |
| CONCAT           | Adds two or more expressions together                                                             |
| CONCAT_WS        | Adds two or more expressions together with a separator                                            |
| FIELD            | Returns the index position of a value in a list of values                                         |
| FIND_IN_SET      | Returns the position of a string within a list of strings                                         |
| FORMAT           | Formats a number to a format like "#,###,###.##", rounded to a specified number of decimal places |
| INSERT           | Inserts a string within a string at the specified position and for a certain number of characters |
| INSTR            | Returns the position of the first occurrence of a string in another string                        |
| LCASE            | Converts a string to lower-case                                                                   |
| LEFT             | Extracts a number of characters from a string (starting from left)                                |
| LENGTH           | Returns the length of a string (in bytes)                                                         |
| LOCATE           | Returns the position of the first occurrence of a substring in a string                           |
| LOWER            | Converts a string to lower-case                                                                   |
| LPAD             | Left-pads a string with another string, to a certain length                                       |
| LTRIM            | Removes leading spaces from a string                                                              |
| MID              | Extracts a substring from a string (starting at any position)                                     |
| POSITION         | Returns the position of the first occurrence of a substring in a string                           |
| REPEAT           | Repeats a string as many times as specified                                                       |
| REPLACE          | Replaces all occurrences of a substring within a string, with a new substring                     |
| REVERSE          | Reverses a string and returns the result                                                          |
| RIGHT            | Extracts a number of characters from a string (starting from right)                               |
| RPAD             | Right-pads a string with another string, to a certain length                                      |
| RTRIM            | Removes trailing spaces from a string                                                             |
| SPACE            | Returns a string of the specified number of space characters                                      |
| STRCMP           | Compares two strings                                                                              |
| SUBSTR           | Extracts a substring from a string (starting at any position)                                     |
| SUBSTRING        | Extracts a substring from a string (starting at any position)                                     |
| SUBSTRING_INDEX  | Returns a substring of a string before a specified number of delimiter occurs                     |
| TRIM             | Removes leading and trailing spaces from a string                                                 |
| UCASE            | Converts a string to upper-case                                                                   |
| UPPER            | Converts a string to upper-case                                                                   |

#### ASCII

* The ASCII() function returns the ASCII value for the specific character.

Syntax:

```
ASCII(character)
```

Example:

```
SELECT FirstName, ASCII(FirstName) AS NumCodeOfFirstChar
FROM employee;

```

Output:

![image AscII ](images/Ascii.png)

#### CHAR_LENGTH

* The CHAR_LENGTH() function return the length of a string

Syntax:

```
CHAR_LENGTH(string)

```

Example:

```
SELECT FirstName,CHAR_LENGTH(FirstName) AS LengthOfName
FROM employee;

```

Output:

![image charleng ](images/carlen.png)



#### CHARACTER_LENGTH

* The CHARACTER_LENGTH() function return the length of a string

Syntax:

```
CHARACTER_LENGTH(string)

```

Example:

```

SELECT LastName, CHARACTER_LENGTH(LastName) AS LengthOfName
FROM employee;

```

Output:

![image charlength ](images/Charater-length.png)



#### CONCAT

* The CONCAT() function adds two or more expressions together.

Syntax:

```

CONCAT(expression1, expression2, expression3,...)
```

Example:

```
SELECT FirstName,LastName, CONCAT(FirstName, " ", LastName) AS FullName
FROM employee;

```

Output:

![image CONCAT ](images/concat.png)


#### CONCAT_WS

* The CONCAT_WS() function adds two or more expressions together with a separator.

Syntax:

```
CONCAT_WS(separator, expression1, expression2, expression3,...)
```

Example:

```

SELECT FirstName,LastName, CONCAT_WS(" ", FirstName, LastName) AS Address
FROM employee;
```

Output:

![image concatws ](images/concatws.png)


#### FIELD

* The FIELD() function returns the index position of a value in a list of values.

* This function performs a case-insensitive search.

Syntax:

```
FIELD(value, val1, val2, val3, ...)

```

Example:

```
SELECT FIELD("Q", "s", "q", "l");
```

Output:

![image FIELD ](images/field.png)


#### FIND_IN_SET

* The FIND_IN_SET() function returns the position of a string within a list of strings.

Syntax:

```
FIND_IN_SET(string, string_list)

```

Example:

```
SELECT FIND_IN_SET("q", "s,q,l");

```

Output:

![image FIELD ](images/field_ser.png)


#### FORMAT

* The FORMAT() function formats a number to a format like "#,###,###.##", rounded to a specified number of decimal places, then it returns the result as a string.

Syntax:

```
FORMAT(number, decimal_places)
```
Example:

```
SELECT FORMAT(25045500.5634, 0);

```

Output:

![image FORMAT ](images/format.png)


#### INSERT

* The INSERT() function inserts a string within a string at the specified position and for a certain number of characters.

Syntax:

```
INSERT(string, position, number, string2)

```
Example:

```
SELECT INSERT("google.com", 8, 3, "no");
```

Output:

![image INSERT ](images/insert-goo.png)


#### INSTR

* The INSTR() function returns the position of the first occurrence of a string in another string.

* This function performs a case-insensitive search.

Syntax:

```
INSTR(string1, string2)

```

Example:

```
SELECT FirstName, INSTR(FirstName, "a")
FROM employee;

```

Output:

![image INSTR ](images/Inter.png)


#### LCASE

* The LCASE() function converts a string to lower-case.

Syntax:

```
LCASE(text)

```
Example:

```
SELECT LCASE(FirstName) AS LowercaseFirstName
FROM employee;
```

Output:

![image LCASE ](images/Lcase.png)

#### LEFT

* The LEFT() function extracts a number of characters from a string (starting from left).

Syntax:

```
LEFT(string, number_of_chars)
```

Example:

```
SELECT FirstName,LEFT(FirstName, 5) AS ExtractString
FROM employee;
```

Output:

![image LEFT ](images/left.png)


#### LENGTH

* The LENGTH() function returns the length of a string (in bytes).

Syntax:

```
LENGTH(string)

```
Example:

```
SELECT FirstName,LENGTH(FirstName) AS LengthOfName
FROM employee;
```

Output:

![image length ](images/length.png)


#### LOCATE

* The LOCATE() function returns the position of the first occurrence of a substring in a string.

* If the substring is not found within the original string, this function returns 0.

* This function performs a case-insensitive search.

Syntax:

```
LOCATE(substring, string, start)

```
Example:

```
SELECT FirstName,LOCATE("a", FirstName)
FROM employee;
```

Output:

![image locate ](images/locate.png)


#### LPAD

* The LPAD() function left-pads a string with another string, to a certain length.

Syntax:

```
LPAD(string, length, lpad_string)
```

Example:

```
SELECT LPAD(FirstName, 30, "ABC") AS LeftPadFirstName
FROM employee;
```

Output:

![image LPAD ](images/LPad.png)

#### LTRIM

* The LTRIM() function removes leading spaces from a string.

Syntax:

```
LTRIM(string)
```
Example:

```
SELECT LTRIM("FirstName") AS LeftTrimmedString;
```

Output:

![image LTRIM ](images/ltrim.png)


#### MID

* The MID() function extracts a substring from a string (starting at any position).

Syntax:

```
MID(string, start, length)

```

Example:

```
SELECT FirstName,MID(FirstName, 2, 5) AS ExtractString
FROM employee;
```

Output:

![image MID ](images/mid.png)

#### POSITION

* The POSITION() function returns the position of the first occurrence of a substring in a string.

* If the substring is not found within the original string, this function returns 0.

Syntax:

```
POSITION(substring IN string)

```

Example:

```
SELECT FirstName,POSITION("a" IN FirstName)
FROM employee;
```

Output:

![image POSITION ](images/position.png)

#### REPEAT

* The REPEAT() function repeats a string as many times as specified.

Syntax:

```
REPEAT(string, number)
```

Example:

```
SELECT FirstName,REPEAT(FirstName, 2)
FROM employee;
```

Output:

![image REPEAT ](images/repeat.png)

#### REPLACE

* The REPLACE() function replaces all occurrences of a substring within a string, with a new substring.

Syntax:

```
REPLACE(string, substring, new_string)
```

Example:

```
SELECT FirstName,REPLACE(FirstName, "a", "m") from employee;
```

Output:

![image REPLACE ](images/Replace.png)


#### REVERSE

* The REVERSE() function reverses a string and returns the result

Syntax:

```
REVERSE(string)
```

Example:

```
SELECT FirstName,REVERSE(FirstName) from employee;
```

Output:

![image REVERSE ](images/reverse.png)


#### RIGHT

* The RIGHT() function extracts a number of characters from a string (starting from right).

Syntax:

```
RIGHT(string, number_of_chars)
```

Example:

```
SELECT FirstName, RIGHT(FirstName, 5) AS ExtractString
FROM employee;
```

Output:

![image RIGHT ](images/right.png)


#### RPAD

* The RPAD() function right-pads a string with another string, to a certain length.

Syntax:

```
RPAD(string, length, rpad_string)
```

Example:

```
SELECT FirstName,RPAD(FirstName, 30, "ABC") AS RightPadFirstName
FROM employee;
```

Output:

![image RPAD ](images/Rpad.png)

#### RTRIM

* The RTRIM() function removes trailing spaces from a string

Syntax:

```
RTRIM(string)

```

Example:

```

SELECT firstname,RTRIM(firstname) AS RightTrimmedString from employee;
```

Output:

![image RTRIM ](images/rtrim.png)


#### SPACE

* The SPACE() function returns a string of the specified number of space characters.

Syntax:

```
SPACE(number)
```

Example:

```
SELECT SPACE(10);
```

Output:

![image SPACE ](images/space.png)


#### STRCMP

* The STRCMP() function compares two strings.

Syntax:

```
STRCMP(string1, string2)
```

Example:

```
SELECT FirstName,LastName,STRCMP(FirstName, LastName) from employee;

```

Output:

![image STRCMP ](images/strcom.png)


#### SUBSTR

* The SUBSTR() function extracts a substring from a string (starting at any position).

Syntax:

```
SUBSTR(string, start, length)

or

SUBSTR(string FROM start FOR length)

```

Example:

```
SELECT FirstName,SUBSTR(FirstName, 2, 5) AS ExtractString
FROM employee;
```

Output:

![image SUBSTR ](images/substr.png)


#### SUBSTRING_INDEX

* The SUBSTRING_INDEX() function returns a substring of a string before a specified number of delimiter occurs.

Syntax:

```
SUBSTRING_INDEX(string, delimiter, number)
```

Example:

```
SELECT LastName,SUBSTRING_INDEX(LastName, ".", 1) AS ExtractString
FROM employee;
```

Output:

![image SUBSTRING_INDEX ](images/sub-index.png)

#### UCASE

* The UCASE() function converts a string to upper-case.

Syntax:

```
UCASE(text)
```

Example:

```
SELECT FirstName,UCASE(FirstName) AS UppercaseFirstName
FROM employee;
```

Output:

![image UCASE ](images/ucase.png)

## MySQL Views

## MySQL Stored Procedure 