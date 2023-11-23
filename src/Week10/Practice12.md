# DVD Rental Database Queries

## Request 1
- In the film table, the length of the film is shown in the length column. How many films are there with a length greater than the average film length?
### Query
```sql
SELECT COUNT(*)
FROM film
WHERE length > (SELECT AVG(length) FROM film);
```

## Request 2
- How many films are there with the highest rental_rate value in the film table?
### Query
```sql
SELECT COUNT(*)
FROM film
WHERE rental_rate = (SELECT MAX(rental_rate) FROM film);
```

## Request 3
- List the films with the lowest rental_rate and the lowest replacement_cost values in the film table.
### Query
```sql
SELECT *
FROM film
WHERE rental_rate = (SELECT MIN(rental_rate) FROM film)
AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);
```

## Request 4
- List the customers who shop the most in the payment table.
### Query
```sql
SELECT customer_id, COUNT(*) as payment_count
FROM payment
GROUP BY customer_id
ORDER BY payment_count DESC;
```

## Note
These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).