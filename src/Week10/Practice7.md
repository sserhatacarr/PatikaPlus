
# DVD Rental Database Queries

## Request 1
- Group the films in the film table according to their rating values.
### Query
```sql
SELECT rating, COUNT(*)
FROM film
GROUP BY rating;
```

## Request 2
- When we group the films in the film table according to the replacement_cost column, list the replacement_cost value and the corresponding number of films where the number of films is more than 50.
### Query
```sql
SELECT replacement_cost, COUNT(*)
FROM film
GROUP BY replacement_cost
HAVING COUNT(*) > 50;
```

## Request 3
- What are the numbers of customers corresponding to the store_id values in the customer table?
### Query
```sql
SELECT store_id, COUNT(*)
FROM customer
GROUP BY store_id;
```

## Request 4
- After grouping the city data in the city table according to the country_id column, share the country_id information and the number of cities that contain the most cities.
### Query
```sql
SELECT country_id, COUNT(*)
FROM city
GROUP BY country_id
ORDER BY COUNT(*) DESC
LIMIT 1;
```

## Note
These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).

