# DVD Rental Database Queries

## Request 1
- Retrieve the data from the title and description columns in the film table.
### Query
```sql
SELECT title, description FROM film;
```

## Request 2
- Retrieve all data from all columns in the film table with the condition that the length is greater than 60 AND less than 75.
### Query
```sql
SELECT * FROM film WHERE length > 60 AND length < 75;
```

## Request 3
- Retrieve all data from all columns in the film table with the conditions rental_rate is 0.99 AND replacement_cost is 12.99 OR 28.99.
### Query
```sql
SELECT * FROM film WHERE rental_rate = 0.99 AND (replacement_cost = 12.99 OR replacement_cost = 28.99);
```

## Request 4
- Retrieve the last_name value of the customer whose first_name is 'Mary' in the customer table.
### Query
```sql
SELECT last_name FROM customer WHERE first_name = 'Mary';
```
## Request 5
- Retrieve all data from all columns in the film table where length is not greater than 50 AND rental_rate is not 2.99 or 4.99.
### Query
```sql
SELECT * FROM film WHERE length <= 50 AND rental_rate != 2.99 AND rental_rate != 4.99;
```
## Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).