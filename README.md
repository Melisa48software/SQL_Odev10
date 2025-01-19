# SQL_Odev10
lcw bootcamp sql 10.ödev reposudur.

-- 1. City ve Country Tablosunu LEFT JOIN Kullanarak Birleştirmek
SELECT city.city, country.country
FROM city
LEFT JOIN country ON city.country_id = country.country_id;

-- 2. Customer ve Payment Tablosunu RIGHT JOIN Kullanarak Birleştirmek
SELECT payment.payment_id, customer.first_name, customer.last_name
FROM customer
RIGHT JOIN payment ON customer.customer_id = payment.customer_id;

-- 3. Customer ve Rental Tablosunu FULL JOIN Kullanarak Birleştirmek
SELECT rental.rental_id, customer.first_name, customer.last_name
FROM customer
FULL JOIN rental ON customer.customer_id = rental.customer_id;
