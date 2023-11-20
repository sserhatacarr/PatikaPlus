# DVD Rental Database Queries

## Request 1
- Retrieve unique values from the replacement_cost column in the film table.
### Query
```sql
SELECT DISTINCT replacement_cost FROM film;
```

## Request 2
- Count the number of distinct values in the replacement_cost column in the film table.
### Query
```sql
SELECT COUNT(DISTINCT replacement_cost) FROM film;
```

## Request 3
- Count the number of films in the film table where the title starts with the character 'T' and has a rating of 'G'.
### Query
```sql
SELECT COUNT(*) FROM film WHERE title LIKE 'T%' AND rating = 'G';
```

## Request 4
- Count the number of countries in the country table where the country name has exactly 5 characters.
### Query
```sql
SELECT COUNT(*) FROM country WHERE LENGTH(country) = 5;
```
## Request 5
- Count the number of cities in the city table where the city name ends with the character 'R' or 'r'.
### Query
```sql
SELECT COUNT(*) FROM city WHERE city ILIKE '%r';
```

## Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).