# DVD Rental Database Queries

## Question 1
### Query
```sql
-- Retrieve country names from the country column in the country table that start with the character 'A' and end with the character 'a'.
SELECT country FROM country WHERE country ILIKE 'A%a';
```
## Question 2
### Query
```sql
-- Retrieve country names from the country column in the country table that have at least 6 characters and end with the character 'n'.
SELECT country FROM country WHERE LENGTH(country) >= 6 AND country LIKE '%n';

```
## Question 3
### Query
```sql
-- Retrieve film names from the title column in the film table that contain the character 'T' (case-insensitive) at least 4 times, regardless of case.
SELECT * FROM film WHERE LOWER(title) LIKE '%t%' OR UPPER(title) LIKE '%T%' LIMIT 4;
```
## Question 4
### Query
```sql
-- Retrieve all data from all columns in the film table where the title starts with the character 'C', length is greater than 90, and rental_rate is 2.99.
SELECT * FROM film WHERE title LIKE 'C%' AND length > 90 AND rental_rate = 2.99;
```

## Note

- Note
  These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).