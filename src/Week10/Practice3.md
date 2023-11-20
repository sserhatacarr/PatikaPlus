# DVD Rental Database Queries

## Request 1
- Retrieve country names from the country column in the country table that start with the character 'A' and end with the character 'a'.
### Query
```sql
SELECT country FROM country WHERE country ILIKE 'A%a';
```

## Request 2
- Retrieve country names from the country column in the country table that have at least 6 characters and end with the character 'n'.
### Query
```sql
SELECT country FROM country WHERE LENGTH(country) >= 6 AND country LIKE '%n';
```

## Request 3
- Retrieve film names from the title column in the film table that contain the character 'T' (case-insensitive) at least 4 times, regardless of case.
### Query
```sql
SELECT * FROM film WHERE LOWER(title) LIKE '%t%' OR UPPER(title) LIKE '%T%' LIMIT 4;
```

## Request 4
- Retrieve all data from all columns in the film table where the title starts with the character 'C', length is greater than 90, and rental_rate is 2.99.
### Query
```sql
SELECT * FROM film WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;
```

## Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).