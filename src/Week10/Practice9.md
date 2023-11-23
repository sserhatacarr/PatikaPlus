# DVD Rental Database Queries

## Request 1
- Write an INNER JOIN query to see the city (city) and country (country) names together in the city and country tables.
### Query
```sql
SELECT city.city, country.country
FROM city
INNER JOIN country ON city.country_id = country.country_id;
```

## Request 2
- Write an INNER JOIN query to see the payment_id in the payment table and the first_name and last_name names in the customer table together.
### Query
```sql
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM payment
INNER JOIN customer ON payment.customer_id = customer.customer_id;
```

## Request 3
- Write an INNER JOIN query to see the rental_id in the rental table and the first_name and last_name names in the customer table together.
### Query
```sql
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM rental
INNER JOIN customer ON rental.customer_id = customer.customer_id;
```

## Note
These queries are based on the DVD Rental database. You can download the database from [here](https://sp.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip).