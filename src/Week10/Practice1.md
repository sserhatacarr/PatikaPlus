# DVD Rental Database Queries

## Question 1
### Query
```sql
-- Retrieve the data from the title and description columns in the film table.
SELECT title, description FROM film;
```

## Question 2
### Query
```sql
-- Retrieve all data from all columns in the film table with the condition that the length is greater than 60 AND less than 75.
SELECT * FROM film WHERE length > 60 AND length < 75;
```

## Question 3
### Query
```sql
-- Retrieve all data from all columns in the film table with the conditions rental_rate is 0.99 AND replacement_cost is 12.99 OR 28.99.
SELECT * FROM film WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);
```

## Question 4
### Query
```sql
-- Retrieve the last_name value of the customer whose first_name is 'Mary' in the customer table.
SELECT last_name FROM customer WHERE first_name = 'Mary';
```
## Question 5
### Query
```sql
-- Retrieve all data from all columns in the film table where length is not greater than 50 AND rental_rate is not 2.99 or 4.99.
SELECT * FROM film WHERE length <= 50 AND rental_rate != 2.99 AND rental_rate != 4.99;
```