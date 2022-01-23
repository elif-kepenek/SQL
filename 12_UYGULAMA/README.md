<p>Film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?</p>

```sql
SELECT COUNT(*) FROM film
WHERE length > 
(
    SELECT AVG(lemgth) FROM film
);
```

<p>Film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?</p>

```sql
SELECT * FROM film
WHERE rental_rate = 
(
    SELECT AVG(length) FROM film
);
```

<p>Film tablosunda en düşük rental_rate ve en düşük replacement_cost değerlerine sahip filmleri sıralayınız.</p>

```sql
SELECT * FROM film
WHERE rental_rate = ANY 
(
    SELECT MIN(rental_rate) FROM film
)
AND replacement_cost = ANY 
(
    SELECT MIN(replacement_cost) FROM film
);
```

<p>Payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.</p>

```sql
SELECT customer.first_name, customer.last_name FROM payment
INNER JOIN customer ON payment.customer_id = customer.id
WHERE payment.amount =
(
    SELECT MAX(amount) FROM payment
);
```