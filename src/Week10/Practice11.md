# DVD Rental Database Queries

## Request 1
- List all data for the first_name columns in the actor and customer tables.
### Query
```sql
(SELECT first_name FROM actor)
UNION
(SELECT first_name FROM customer);
```

## Request 2
- List intersecting data for the first_name columns in the actor and customer tables.
### Query
```sql
(SELECT first_name FROM actor)
INTERSECT
(SELECT first_name FROM customer);
```

## Request 3
- List data found in the first table but not in the second for the first_name columns in the actor and customer tables.
### Query
```sql
(SELECT first_name FROM actor)
EXCEPT
(SELECT first_name FROM customer);
```

## Request 4
- Repeat the first 3 queries for duplicate data as well.
### Query
```sql
(SELECT first_name FROM actor)
UNION ALL
(SELECT first_name FROM customer);

(SELECT first_name FROM actor)
INTERSECT ALL
(SELECT first_name FROM customer);

(SELECT first_name FROM actor)
EXCEPT ALL
(SELECT first_name FROM customer);
```

## Note
These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).