## Questions and Answers

1) Select the FirstName, LastName, and CompanyName of all Customers whose company name 
contains the word "Bike". Sort the results by LastName, then FirstName, then CompanyName.
<details><summary>Show answer #1</summary>

```sql
    SELECT FirstName
        , LastName
        , CompanyName
    FROM SalesLT.Customer
    WHERE CompanyName LIKE '%Bike%'
```
</details>

2) Select all the customers who do not have a middle name.

3) Select all the customers with a first name of "Mike" whose phone number starts with 454

4) Select all of the Products that are Red and have a ListPrice between $500 and $1500

5) Using your solution from question 4, add another condition to narrow your previous results to only include Products with a weight over 9000.

6) Select all of the Products that have a name containing "Mountain Frame" or "Road Frame" and have a Color of "Red". Sort the results by Color in descending order and then by Name in ascending order


## Story Problem Questions and Answers

The following questions will not specifically point out a table/columns that you need to work with. You will have to look at the data in the database and think about the query you need to code and result set you need to solve a problem.

1) A customer comes in and is asks if you carry medium sports shorts and what colors they come in.

2) A customer asks if anybody at their company "Sharp Bikes" is a customer. If yes, what is their phone number?

3) A customer with a high-end store wants to know what the three most expensive wheels are for any bike.

4) A customer, Gary Vargas from Exercise Center, wants to know what email we have on file for him.

5) Which products don't have a custom thumbnail photo available?

6) Which products did we start selling in 2005?