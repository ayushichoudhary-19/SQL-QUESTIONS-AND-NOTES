# SQL Basics and Prerequisites

Before diving into SQL problem-solving on platforms like LeetCode and HackerRank, it's essential to have a good grasp of the basics. This guide provides a quick overview of some fundamental SQL concepts and common query functions.

## Table of Contents
1. [Introduction to SQL](#introduction-to-sql)
2. [Creating a Table](#creating-a-table)
3. [SELECT Statement](#select-statement)
4. [Using Wildcards (*)](#using-wildcards)
5. [Aggregate Functions](#aggregate-functions)
   - [MIN()](#min)
   - [MAX()](#max)
   - [COUNT()](#count)
6. [ORDER BY](#order-by)
   - [ASC (Ascending)](#asc-ascending)
   - [DESC (Descending)](#desc-descending)

## Introduction to SQL
SQL (Structured Query Language) is a domain-specific language used for managing and querying relational databases. It allows you to interact with databases, retrieve data, modify data, and perform various operations.

## Creating a Table
To store data in a relational database, you need to define tables. Here's a basic syntax for creating a table:

```sql
CREATE TABLE table_name (
    column1 datatype,
    column2 datatype,
    ...
);
```

Example:
```sql
CREATE TABLE Students (
    StudentID INT,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    Age INT
);
```

## SELECT Statement
The `SELECT` statement is used to retrieve data from one or more tables. The basic syntax is:

```sql
SELECT column1, column2, ...
FROM table_name;
```

Example:
```sql
SELECT FirstName, LastName
FROM Students;
```

## Using Wildcards (*)
You can use the `*` wildcard to select all columns from a table.

Example:
```sql
SELECT * FROM Students;
```

## Aggregate Functions
Aggregate functions perform a calculation on a set of values and return a single value.

### MIN()
The `MIN()` function returns the minimum value in a set.

Example:
```sql
SELECT MIN(Age) FROM Students;
```

### MAX()
The `MAX()` function returns the maximum value in a set.

Example:
```sql
SELECT MAX(Age) FROM Students;
```

### COUNT()
The `COUNT()` function returns the number of rows in a set.

Example:
```sql
SELECT COUNT(*) FROM Students;
```

## ORDER BY
The `ORDER BY` clause is used to sort the result set in ascending or descending order based on one or more columns.

### ASC (Ascending)
To sort in ascending order (default behavior):

```sql
SELECT * FROM Students
ORDER BY Age ASC;
```

### DESC (Descending)
To sort in descending order:

```sql
SELECT * FROM Students
ORDER BY Age DESC;
```

These are some fundamental SQL concepts and functions that will be useful as you start solving SQL problems on platforms like LeetCode and HackerRank. Feel free to explore more SQL topics as you progress in your learning journey.

