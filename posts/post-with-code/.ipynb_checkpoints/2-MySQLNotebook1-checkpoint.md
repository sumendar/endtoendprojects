# MySQL Check (Sample Notebook for preview md)

> A tutorial of SQL Basic Scripting.

-   toc: true
-   badges: true
-   comments: true
-   categories: \[SQL\]

# **Resources:**

-   https://www.educba.com/data-science/data-science-tutorials/mysql-tutorial/\
-   https://www.w3schools.com/mysql/default.asp

```python
USE world;
SELECT * from city limit 5;
```

Commands completed successfully

(5 row(s) affected)

Total execution time: 00:00:00.016

| ID  | Name           | CountryCode | District      | Population |
|-----|----------------|-------------|---------------|------------|
| 1   | Kabul          | AFG         | Kabol         | 1780000    |
| 2   | Qandahar       | AFG         | Qandahar      | 237500     |
| 3   | Herat          | AFG         | Herat         | 186800     |
| 4   | Mazar-e-Sharif | AFG         | Balkh         | 127800     |
| 5   | Amsterdam      | NLD         | Noord-Holland | 731200     |

```python
# LECTURE: Creating a Database - Part I

CREATE DATABASE IF NOT EXISTS Sales;

CREATE SCHEMA IF NOT EXISTS Sales;
```

Commands completed successfully

Commands completed successfully

Total execution time: 00:00:00.019

```python
USE Sales;
```

Commands completed successfully

Total execution time: 00:00:00.007

```python
CREATE TABLE sales
(
    purchase_number INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    date_of_purchase DATE NOT NULL,
    customer_id INT,
    item_code VARCHAR(10) NOT NULL

);
```

Total execution time: 00:00:00.012

```python
MYSQL:
•   Data base concepts(Database, DBMS, RDMS)
•   Installing MYSQL server and Workbench
•   Select Command
•   Distinct Keyword
•   SQL is not Case Sensitive
•   Where Clause
•   Using Relational operators in where clause condition
•   Using logical operators(AND, OR, NOT)
•   Between Operator
•   Order by Clause(ASC, DESC)
•   Using Between operator with Text
•   In operator
•   Like operator and wildcard characters
•   Aliases for table column names
•   Limit keyword
•   Breaking the lengthy SQL statement into Multiple lines
•   My SQL Built in functions
•   Arithmetic Operators
•   Creating, viewing, describing, deleting and using databases
•   Creating tables and inserting records into the table
•   Data Types
•   Null values, is null and is not null 
•   Delete statement
•   Update statement and set keyword
•   Rename statement and To keyword
•   Alter statement ,Add ,Modify column ,rename and drop column
•   Set auto commit
•   Commit statement
•   Rollback statement
•   Truncate statement
•   Single line and multiline comments
•   Group by clause
•   Having Clause
•   Set operators(union, union all, intersect and minus operator)
•   Joins(inner join, left join, right join, full join, self join)
•   Sub Query(Types of sub query)
•   Integrity Constraints(Not null, unique, primary and foreign key, check, default)
•   Auto increment
•   Insert into 
•   Case, when ,then and end keyword
•   Delimiter
•   Views
•   Indexes
•   Proceedures
•   Any Doubts and Practice assignments on my SQL
ca you please explain definition and query for each step i have entered in the above points one by one till end point in MYSQL language for a novice person with simple queries and easy to understandable definition and small explanation to all above without excluding any?
Sure, I'd be happy to help! Here are the definitions and queries for each of the topics you've listed:
Database Concepts:
A database is an organized collection of data, while a DBMS (Database Management System) is software that manages the database. An RDBMS (Relational Database Management System) is a type of DBMS that stores data in tables that are related to each other by primary and foreign keys.
Installing MYSQL server and Workbench:
To install MYSQL server, you can download it from the official MYSQL website and follow the installation wizard. MYSQL Workbench is a graphical user interface for managing databases and can also be downloaded from the official MYSQL website.
Select Command:
The SELECT statement is used to retrieve data from a database. For example, to select all columns from a table called "users", you would use the following query:
sql
Copy code
SELECT * FROM users;
Distinct Keyword:
The DISTINCT keyword is used to select unique values from a column. For example, to select unique values from a column called "city" in a table called "customers", you would use the following query:
sql
Copy code
SELECT DISTINCT city FROM customers;
SQL is not Case Sensitive:
SQL is not case sensitive, which means that keywords such as SELECT and select are equivalent.
Where Clause:
The WHERE clause is used to filter the results of a SELECT statement based on a specified condition. For example, to select all records from a table called "orders" where the "status" column is equal to "shipped", you would use the following query:
sql
Copy code
SELECT * FROM orders WHERE status = 'shipped';
Using Relational Operators in Where Clause Condition:
Relational operators such as =, <, >, <=, >=, and <> can be used in the WHERE clause to compare values. For example, to select all records from a table called "products" where the "price" column is greater than 10, you would use the following query:
sql
Copy code
SELECT * FROM products WHERE price > 10;
Using Logical Operators (AND, OR, NOT):
Logical operators such as AND, OR, and NOT can be used in the WHERE clause to combine conditions. For example, to select all records from a table called "orders" where the "status" column is equal to "shipped" and the "total" column is greater than 100, you would use the following query:
sql
Copy code
SELECT * FROM orders WHERE status = 'shipped' AND total > 100;
Between Operator:
The BETWEEN operator is used in the WHERE clause to select values within a range. For example, to select all records from a table called "sales" where the "date" column is between January 1, 2022 and March 31, 2022, you would use the following query:
sql
Copy code
SELECT * FROM sales WHERE date BETWEEN '2022-01-01' AND '2022-03-31';
Order by Clause (ASC, DESC):
The ORDER BY clause is used to sort the results of a SELECT statement in ascending (ASC) or descending (DESC) order. For example, to select all records from a table called "customers" and order them by last name in descending order, you would use the following query:
sql
Copy code
SELECT * FROM customers ORDER BY last_name DESC;
Using Between Operator with Text:
The BETWEEN operator can also be used with text values. For example, to select all records from a table called "employees" where the "name" column is between "Alice" and "Bob", you would use the following query:
sql
Copy code
SELECT * FROM employees WHERE name
Sumendar
you ended at 11th point, could you please continue with remaining steps from below for the same MySQL for a beginner to understand definition and queries of each below:
In operator
•   Like operator and wildcard characters
•   Aliases for table column names
•   Limit keyword
•   Breaking the lengthy SQL statement into Multiple lines
•   My SQL Built in functions
•   Arithmetic Operators
•   Creating, viewing, describing, deleting and using databases
•   Creating tables and inserting records into the table
•   Data Types
•   Null values, is null and is not null 
•   Delete statement
•   Update statement and set keyword
•   Rename statement and To keyword
•   Alter statement ,Add ,Modify column ,rename and drop column
•   Set auto commit
•   Commit statement
•   Rollback statement
•   Truncate statement
•   Single line and multiline comments
•   Group by clause
•   Having Clause
•   Set operators(union, union all, intersect and minus operator)
•   Joins(inner join, left join, right join, full join, self join)
•   Sub Query(Types of sub query)
•   Integrity Constraints(Not null, unique, primary and foreign key, check, default)
•   Auto increment
•   Insert into 
•   Case, when ,then and end keyword
•   Delimiter
•   Views
•   Indexes
•   Proceedures
•   Any Doubts and Practice assignments on my SQL
Sure, I apologize for missing that. Here are explanations and examples for the remaining points:
In operator:
The IN operator allows you to specify multiple values in a WHERE clause. It is used to check whether a value is included in a list of values or not.
Example: To retrieve the details of all employees whose department is either 'HR' or 'IT', we can use the following query:
sql
Copy code
SELECT * FROM employees WHERE department IN ('HR', 'IT');
Like operator and wildcard characters:
The LIKE operator is used to search for patterns in columns. It is often used with wildcard characters '%' and ''. The '%' character matches zero or more characters, while '' matches exactly one character.
Example: To retrieve the details of all employees whose name starts with 'J', we can use the following query:
sql
Copy code
SELECT * FROM employees WHERE name LIKE 'J%';
Aliases for table column names:
An alias is a temporary name assigned to a table or column. It can make queries more readable and understandable.
Example: To retrieve the details of all employees along with their salaries, we can use the following query with aliases:
vbnet
Copy code
SELECT name AS EmployeeName, salary AS EmployeeSalary FROM employees;
Limit keyword:
The LIMIT keyword is used to limit the number of records returned in a query result.
Example: To retrieve the details of the first five employees, we can use the following query:
sql
Copy code
SELECT * FROM employees LIMIT 5;
Breaking the lengthy SQL statement into Multiple lines:
A lengthy SQL statement can be broken into multiple lines to improve its readability.
Example: To retrieve the details of all employees whose age is greater than or equal to 25 and salary is greater than or equal to 50000, we can use the following query with line breaks:
sql
Copy code
SELECT * 
FROM employees 
WHERE age >= 25 
AND salary >= 50000;
My SQL Built-in functions:
MySQL provides a number of built-in functions to manipulate data. Some common ones include COUNT(), SUM(), AVG(), MAX(), MIN(), etc.
Example: To retrieve the total number of employees in the employees table, we can use the COUNT() function:
sql
Copy code
SELECT COUNT(*) FROM employees;
Arithmetic Operators:
MySQL supports arithmetic operators such as +, -, *, /, %.
Example: To retrieve the details of all employees whose salary is more than twice their age, we can use the following query:
sql
Copy code
SELECT * FROM employees WHERE salary > 2 * age;
Creating, viewing, describing, deleting and using databases:
A database is a collection of tables and other objects that are used to store and manage data. MySQL provides various commands to create, view, describe, delete and use databases.
Example: To create a new database named 'mydatabase', we can use the following query:
sql
Copy code
CREATE DATABASE mydatabase;
Creating tables and inserting records into the table:
A table is a collection of data that is organized in a specific format. MySQL provides commands to create tables and insert records into the tables.
Example: To create a new table named 'employees' with columns 'name', 'age', 'department' and 'salary', we can use the following query:
sql
Copy code
CREATE TABLE employees (
    name VARCHAR(50),
    age INT,
    department VARCHAR(50),
    salary DECIMAL(10,2)
);
To insert a record into the employees table, we can use the following query:
sql
Copy code
INSERT INTO employees (name, age, department, salary) VALUES ('John Doe', 30, 'IT', 60000);
Data Types:
Data types specify the type of data
Sumendar
you have been missed remaining can you explain below steps till last point in same mysql with easy definition and queries 
Null values, is null and is not null 
•   Delete statement
•   Update statement and set keyword
•   Rename statement and To keyword
•   Alter statement ,Add ,Modify column ,rename and drop column
•   Set auto commit
•   Commit statement
•   Rollback statement
•   Truncate statement
•   Single line and multiline comments
•   Group by clause
•   Having Clause
•   Set operators(union, union all, intersect and minus operator)
•   Joins(inner join, left join, right join, full join, self join)
•   Sub Query(Types of sub query)
•   Integrity Constraints(Not null, unique, primary and foreign key, check, default)
•   Auto increment
•   Insert into 
•   Case, when ,then and end keyword
•   Delimiter
•   Views
•   Indexes
•   Proceedures
•   Any Doubts and Practice assignments on my SQL
Sure, I apologize for the mistake earlier. I will continue from where I left off:
Null values, is null and is not null:
In SQL, a null value represents a missing or unknown value. The IS NULL and IS NOT NULL operators are used to check for null values in a column.
To select all rows where a column is null, you can use the IS NULL operator like this:
sql
Copy code
SELECT * FROM my_table WHERE my_column IS NULL;
To select all rows where a column is not null, you can use the IS NOT NULL operator like this:
sql
Copy code
SELECT * FROM my_table WHERE my_column IS NOT NULL;
Delete statement:
The DELETE statement is used to delete one or more rows from a table. The basic syntax for the DELETE statement is as follows:
sql
Copy code
DELETE FROM table_name WHERE condition;
For example, to delete all rows from a table where the age column is greater than 30, you would use the following statement:
sql
Copy code
DELETE FROM my_table WHERE age > 30;
Update statement and set keyword:
The UPDATE statement is used to modify one or more columns in one or more rows in a table. The basic syntax for the UPDATE statement is as follows:
sql
Copy code
UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition;
For example, to update the age column to 30 for all rows where the name column is 'John', you would use the following statement:
sql
Copy code
UPDATE my_table SET age = 30 WHERE name = 'John';
Rename statement and To keyword:
The RENAME statement is used to rename a table or a column in a table. The basic syntax for the RENAME statement is as follows:
css
Copy code
ALTER TABLE table_name RENAME TO new_table_name;
For example, to rename a table called old_table to new_table, you would use the following statement:
css
Copy code
ALTER TABLE old_table RENAME TO new_table;
To rename a column in a table, you would use the following statement:
sql
Copy code
ALTER TABLE my_table RENAME COLUMN old_column_name TO new_column_name;
Alter statement, Add, Modify column, rename and drop column:
The ALTER statement is used to modify the structure of a table, such as adding or modifying columns, renaming columns, or dropping columns.
To add a new column to a table, you would use the following statement:
sql
Copy code
ALTER TABLE my_table ADD new_column_name data_type;
To modify the data type of an existing column, you would use the following statement:
sql
Copy code
ALTER TABLE my_table MODIFY column_name new_data_type;
To rename a column in a table, you would use the following statement:
sql
Copy code
ALTER TABLE my_table RENAME COLUMN old_column_name TO new_column_name;
To drop a column from a table, you would use the following statement:
sql
Copy code
ALTER TABLE my_table DROP column_name;
Set auto commit:
Auto-commit is a feature in MySQL that automatically commits the current transaction after each SQL statement. To enable auto-commit, you can use the following statement:
java
Copy code
SET autocommit = 1;
To disable auto-commit, you can use the following statement:
java
Copy code
SET autocommit = 0;
Commit statement:
The COMMIT statement is used to permanently save the changes made to a database.
sql
Copy code
COMMIT;
Rollback statement:
The ROLLBACK statement is used to undo changes made to a database in the current transaction.
sql
Copy code
ROLLBACK;
Truncate statement:
The TRUNCATE statement is used to remove all
Sumendar
can you complete remaining till end of all points below?
•   Single line and multiline comments
•   Group by clause
•   Having Clause
•   Set operators(union, union all, intersect and minus operator)
•   Joins(inner join, left join, right join, full join, self join)
•   Sub Query(Types of sub query)
•   Integrity Constraints(Not null, unique, primary and foreign key, check, default)
•   Auto increment
•   Insert into 
•   Case, when ,then and end keyword
•   Delimiter
•   Views
•   Indexes
•   Proceedures
Sure, I can continue with the remaining points. Here are the explanations and examples for each:
Single Line and Multiline Comments:
Comments in SQL are used to write a description or explanation of the code, which makes it easier for others to understand the code. There are two types of comments in SQL: single-line comments and multiline comments.
Single-line comments start with two hyphens (--). Anything that follows after the double hyphen is ignored by the SQL engine. For example:
sql
Copy code
-- This is a single-line comment
SELECT * FROM mytable;
Multiline comments start with a forward-slash and an asterisk (/) and end with an asterisk and a forward-slash (/). Anything that is enclosed between these two characters is ignored by the SQL engine. For example:
sql
Copy code
/*
This is a multiline comment.
It can span multiple lines.
*/
SELECT * FROM mytable;
Group By Clause:
The GROUP BY clause is used with aggregate functions like SUM, COUNT, MAX, MIN, and AVG to group the result-set by one or more columns. This clause is used in a SELECT statement and is typically used to summarize data by grouping related records together. For example:
sql
Copy code
SELECT department, SUM(salary) FROM employees GROUP BY department;
In this example, we are selecting the department and the total salary of all employees in each department. The GROUP BY clause groups the result by department.
Having Clause:
The HAVING clause is used to filter the results of a GROUP BY clause. It allows you to specify a condition that must be met for a group of records to be included in the result. For example:
sql
Copy code
SELECT department, SUM(salary) FROM employees GROUP BY department HAVING SUM(salary) > 100000;
In this example, we are selecting the department and the total salary of all employees in each department. The HAVING clause filters the results to only show departments with a total salary greater than 100000.
Set Operators (UNION, UNION ALL, INTERSECT, and MINUS):
Set operators are used to combine the results of two or more SELECT statements. There are four set operators in SQL: UNION, UNION ALL, INTERSECT, and MINUS.
UNION: combines the results of two SELECT statements and removes duplicate rows.
UNION ALL: combines the results of two SELECT statements and includes all rows, including duplicates.
INTERSECT: returns only the rows that are common to the results of two SELECT statements.
MINUS: returns the rows from the first SELECT statement that are not in the second SELECT statement.
For example:
sql
Copy code
SELECT column1 FROM table1 UNION SELECT column1 FROM table2;
This example combines the results of two SELECT statements that both select column1 from two different tables.
Joins (INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, SELF JOIN):
Joins are used to combine rows from two or more tables based on a related column between them. There are different types of joins in SQL, including:
INNER JOIN: returns only the matching rows from both tables.
LEFT JOIN: returns all the rows from the left table and matching rows from the right table.
RIGHT JOIN: returns all the rows from the right table and matching rows from the left table.
FULL JOIN: returns all the rows from both tables, including any non-matching rows.
SELF JOIN: a join in which a table is joined with itself.
For example:
sql
Copy code
SELECT orders.order_id, customers.customer_name FROM orders INNER JOIN customers ON orders.customer_id = customers.customer_id;
This example selects the order ID and customer name from the orders and customers tables, where the customer ID in the
Sumendar
can you please conclude remaining below as too till end in the same way?
Sub Query(Types of sub query)
•   Integrity Constraints(Not null, unique, primary and foreign key, check, default)
•   Auto increment
•   Insert into 
•   Case, when ,then and end keyword
•   Delimiter
•   Views
•   Indexes
•   Proceedures
Sub Query(Types of subquery):
A subquery, also known as an inner query, is a query that is nested inside another query. It is used to retrieve data that will be used as part of the criteria in the main query. There are two types of subqueries:
Single-row subquery: This type of subquery is used to retrieve a single value, which is used as part of the criteria in the main query.
Example:
SELECT *
FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
In this example, the subquery retrieves the average salary of all employees, which is then used as part of the criteria in the main query to retrieve all employees with a salary greater than the average.
Multiple-row subquery: This type of subquery is used to retrieve multiple rows, which are then used as part of the criteria in the main query.
Example:
SELECT *
FROM employees
WHERE department_id IN (SELECT department_id FROM departments WHERE location_id = 1700);
In this example, the subquery retrieves all department IDs from the departments table that have a location ID of 1700, which is then used as part of the criteria in the main query to retrieve all employees who work in those departments.
Integrity Constraints(Not null, unique, primary and foreign key, check, default):
Integrity constraints are used to ensure data accuracy and consistency in the database. They are rules that must be followed by the data in the database.
NOT NULL: This constraint ensures that a column cannot have a null value.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
name VARCHAR(50) NOT NULL,
age INT NOT NULL
);
UNIQUE: This constraint ensures that each value in a column is unique.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
email VARCHAR(50) UNIQUE
);
PRIMARY KEY: This constraint ensures that each row in a table is uniquely identified by a specific column or columns.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
name VARCHAR(50),
age INT
);
FOREIGN KEY: This constraint ensures that the values in a column of one table match the values in a column of another table.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
name VARCHAR(50),
department_id INT,
FOREIGN KEY (department_id) REFERENCES departments(id)
);
CHECK: This constraint ensures that the values in a column meet a specific condition.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
name VARCHAR(50),
age INT,
CONSTRAINT age_check CHECK (age >= 18)
);
DEFAULT: This constraint sets a default value for a column if no value is specified.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY,
name VARCHAR(50),
age INT DEFAULT 18
);
Auto Increment:
Auto increment is a feature that automatically increments the value of a column by 1 each time a new row is inserted into a table. It is commonly used for primary key columns to ensure that each row has a unique identifier.
Example:
CREATE TABLE employees (
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(50),
age INT
);
Insert into:
The INSERT INTO statement is used to insert new rows into a table.
Example:
INSERT INTO employees (name, age) VALUES ('John', 25);
This statement inserts a new row into the employees table with the values 'John' and 25 in the name and age columns, respectively.
Case, When, Then, and End Keyword:
The CASE statement is used to conditionally execute a set of statements based on a specific condition. It has the following syntax:
CASE
WHEN condition1 THEN
```
