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

1) Select the FirstName, LastName, and CompanyName of all Customers whose company name contains the word "Bike". Sort the results by LastName, then FirstName, then CompanyName.

2) Select all the customers who do not have a middle name.

3) Select all the customers with a first name of "Mike" whose phone number starts with 454

4) Select all of the Products that are Red and have a ListPrice between $500 and $1500

5) Using your solution from question 4, add another condition to narrow your previous results to only include Products with a weight over 9000.

6) Select all of the Products that have a name containing "Mountain Frame" or "Road Frame" and have a Color of "Red". Sort the results by Color in descending order and then by Name in ascending order


## Story Problems
The following questions will not specifically point out a table/columns that you need to work with. You will have to look at the data in the database and think about the query you need to code and result set you need to solve a problem.

1) A customer comes in and is asks if you carry medium sports shorts and what colors they come in.

2) A customer asks if anybody at their company "Sharp Bikes" is a customer. If yes, what is their phone number?

3) A customer with a high-end store wants to know what the three most expensive wheels are for any bike.

4) A customer, Gary Vargas from Exercise Center, wants to know what email we have on file for him.

5) Which products don't have a custom thumbnail photo available?

6) Which products did we start selling in 2005?