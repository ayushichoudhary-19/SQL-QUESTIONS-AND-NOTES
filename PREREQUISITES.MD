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
