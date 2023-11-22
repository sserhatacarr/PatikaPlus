
# DVD Rental Database Queries

## Request 1
- Calculate the average of the values in the rental_rate column in the film table.
### Query
```sql
SELECT AVG(rental_rate) FROM film;
```

## Request 2
- Count how many films in the film table start with the character 'C'.
### Query
```sql
SELECT COUNT(*) FROM film WHERE title LIKE 'C%';
```

## Request 3
- Find the length of the longest film in the film table where the rental_rate value is equal to 0.99.
### Query
```sql
SELECT MAX(length) FROM film WHERE rental_rate = 0.99;
```

## Request 4
- Count how many different replacement_cost values there are for films in the film table that are longer than 150 minutes.
### Query
```sql
SELECT COUNT(DISTINCT replacement_cost) FROM film WHERE length > 150;
```

## Note
These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).
