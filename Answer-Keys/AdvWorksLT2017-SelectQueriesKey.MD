*ANSWERS SHOWN ARE JUST POSSIBLE SOLUTIONS AND MAY NOT BE THE ONLY SOLUTION*

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
    ORDER BY LastName, FirstName, CompanyName
```
</details>

2) Select all the customers who do not have a middle name.
<details><summary>Show answer #2</summary>

```sql
    SELECT *
    FROM SalesLT.Customer
    WHERE MiddleName IS NULL
```

</details>

3) Select all the customers with a first name of "Mike" whose phone number starts with 454
<details><summary>Show answer #3</summary>

```sql
    SELECT *
    FROM SalesLT.Customer
    --WHERE FirstName = 'Mike' AND LEFT(Phone, 3) = 454
    WHERE FirstName = 'Mike' AND Phone LIKE '454%'
```

</details>


4) Select all of the Products that are Red and have a ListPrice between $500 and $1500
<details><summary>Show answer #4</summary>

```sql
    SELECT *
    FROM SalesLT.Product
    WHERE Color = 'Red' AND ListPrice BETWEEN 500 and 1500
```

</details>

5) Using your solution from question 4, add another condition to narrow your previous results to only include Products with a weight over 9000.
<details><summary>Show answer #5</summary>

```sql
    SELECT *
    FROM SalesLT.Product
    WHERE Color = 'Red' AND ListPrice BETWEEN 500 and 1500
        AND Weight > 9000
```

</details>

6) Select all of the Products that have a name containing "Mountain Frame" or "Road Frame" and have a Color of "Red". Sort the results by Color in descending order and then by Name in ascending order
<details><summary>Show answer #6</summary>

```sql
    -- Parenthesis around the OR conditions make sure we select
    -- mountain frames that are red, or road frames that are red
    -- Since all bikes are Red, we don't actually need to sort by color
    -- but the question does ask
    SELECT *
    FROM SalesLT.Product
    WHERE (Name LIKE '%Mountain Frame%' OR
        Name LIKE '%Road Frame%') AND
        Color = 'Red'
    ORDER BY Color DESC, Name
```

</details>


## Story Problem Questions and Answers

The following questions will not specifically point out a table/columns that you need to work with. You will have to look at the data in the database and think about the query you need to code and result set you need to solve a problem.

1) A customer comes in and is asks if you carry medium sports shorts and what colors they come in.

2) A customer asks if anybody at their company "Sharp Bikes" is a customer. If yes, what is their phone number?

3) A customer with a high-end store wants to know what the three most expensive wheels are for any bike.

4) A customer, Gary Vargas from Exercise Center, wants to know what email we have on file for him.

5) Which products don't have a custom thumbnail photo available?

6) Which products did we start selling in 2005?