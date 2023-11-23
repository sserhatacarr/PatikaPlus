
# Employee Table Queries

## Request 1
- Let's create a table named 'employee' in your test database with the column information id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100).
### Query
```sql
create table employee ( 
id SERIAL PRIMARY KEY, 
first_name VARCHAR (50) NOT NULL, 
birth_date DATE NOT NULL, 
email VARCHAR (100) NOT NULL 
);
```

## Request 2
- When we group the films in the film table according to the replacement_cost column, list the replacement_cost value and the corresponding number of films where the number of films is more than 50.
### Query
```sql
insert into author (first_name, last_name, email, birthday) values ('Shaine', 'Purchall', 'spurchall0@cdc.gov', null);
insert into author (first_name, last_name, email, birthday) values ('Geordie', 'Hallums', 'ghallums1@netvibes.com', '1905-09-21');
insert into author (first_name, last_name, email, birthday) values ('Pearle', 'Golthorpp', 'pgolthorpp2@elpais.com', null);
insert into author (first_name, last_name, email, birthday) values ('Luci', 'Robjents', 'lrobjents3@gov.uk', '1906-09-21');
insert into author (first_name, last_name, email, birthday) values ('Kandy', 'Slucock', 'kslucock4@hhs.gov', '1996-11-13');
-------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------------------
```

## Request 3
- Let's perform 5 UPDATE operations that will update the other columns for each column.
### Query
```sql
UPDATE employee SET first_name = 'Updated Name' WHERE id = 1;
UPDATE employee SET birth_date = '2000-01-01' WHERE first_name = 'Erina';
UPDATE employee SET email = 'updatedemail@example.com' WHERE birth_date = '1920-09-20';
UPDATE employee SET first_name = 'Another Name', birth_date = '1990-01-01' WHERE email = 'bmorales3@symantec.com';
UPDATE employee SET first_name = 'New Name', birth_date = '1990-01-01', email = 'newemail@example.com' WHERE id = 5;
```

## Request 4
- Let's perform 5 DELETE operations that will delete the relevant row for each column.
### Query
```sql
DELETE FROM employee WHERE id = 10;
DELETE FROM employee WHERE first_name = 'Taylor';
DELETE FROM employee WHERE birth_date = '1999-12-17';
DELETE FROM employee WHERE email = 'ltunnadinea@macromedia.com';
DELETE FROM employee WHERE first_name = 'Mozelle' AND birth_date = '1908-07-06';
```

