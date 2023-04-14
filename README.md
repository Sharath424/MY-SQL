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

## Data Manipulation Lanaguage(DML)

## Transaction Control Lanaguage(TCL)

## Data Query/Retrieval Language (DQL/DRL)

## MySQL Functions

## MySQL Sub Query

## MySQL Views

## MySQL Stored Procedure 