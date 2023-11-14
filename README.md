# Домашнее задание к занятию "SQL. Часть 1" - `Хамов Олег`

### Задание 1

SELECT DISTINCT district

FROM sakila.address

WHERE district like 'K%a'

    and POSITION(' ' IN district) = 0;

### Задание 2

SELECT *

FROM sakila.payment

WHERE Date(payment_date) between '2005-06-15' and '2005-06-18'

    and amount > 10.0;

### Задание 3

SELECT *

FROM sakila.rental

ORDER BY rental_date DESC

LIMIT 5;

### Задание 4

SELECT REPLACE(LOWER(first_name), 'll', 'pp'), LOWER(last_name), active

FROM sakila.customer

WHERE first_name IN ('Kelly', 'Willie')
 
    and active = 1;










