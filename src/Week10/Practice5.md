# DVD Rental Database Queries

## Request 1
- Retrieve the 5 longest films in the film table that end with the character 'n'.
### Query
```sql
SELECT * FROM film WHERE title LIKE '%n' ORDER BY length DESC LIMIT 5;
```

## Request 2
### Query
- Retrieve the second 5 (lengths 6, 7, 8, 9, 10) the shortest films in the film table that end with the character 'n'.
```sql
SELECT * FROM film WHERE title LIKE '%n' ORDER BY length ASC OFFSET 5 LIMIT 5;
```

## Request 3
- Retrieve the first 4 records from the customer table, sorted in descending order by last_name, where store_id is 1.
### Query
```sql
SELECT * FROM customer WHERE store_id = 1 ORDER BY last_name DESC LIMIT 4;
```

## Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).