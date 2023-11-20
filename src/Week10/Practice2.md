# DVD Rental Database Queries

## Request 1
- Retrieve all data from all columns in the film table with the condition that the replacement cost is greater than or equal to 12.99 and less than 16.99 (use BETWEEN - AND).
### Request
```sql
SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.99;
```

## Request 2
### Request
- Retrieve data from the first_name and last_name columns in the actor table with the condition that first_name is 'Penelope', 'Nick', or 'Ed' (use IN operator).
```sql
SELECT first_name, last_name FROM actor WHERE first_name IN ('Penelope', 'Nick', 'Ed');
```

## Request 3
- Retrieve all data from all columns in the film table with the conditions that rental_rate is 0.99, 2.99, 4.99 AND replacement_cost is 12.99, 15.99, 28.99 (use IN operator).
### Request
```sql
SELECT * FROM film WHERE rental_rate IN (0.99, 2.99, 4.99) AND replacement_cost IN (12.99, 15.99, 28.99);
```

## Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).