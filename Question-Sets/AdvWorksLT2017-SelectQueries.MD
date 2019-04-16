# SELECT Queries for Adventure Works Light 2017


## Getting started

Download and run the Create_AdventureWorksLight2017.sql script. This
will create a database named AdvWorksLT2017.

Script location https://github.com/JoeProgrammer88/SQL-Practice/raw/master/Database-Creation-Scripts/Create_AdventureWorksLight2017.sql

Right-click the "Download" button and choose "Save Link As..." to save the file as a .sql file.

Use the AdvWorksLT2017 database for the following questions

## Before you begin
The AdventureWorks database uses a custom schema for most tables instead of the default dbo. Since dbo is the default schema many developers opt not to add it. That means your FROM clause will need to be slightly modified.
```sql
    SELECT *
    FROM Customer -- could also be written as FROM dbo.Customer
```
has to be written as
```sql
    SELECT *
    FROM SalesLT.Customer
```
notice the schema name "SalesLT" in front of the table name?

## Questions

