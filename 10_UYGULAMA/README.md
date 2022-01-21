<p>City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.</p>

```sql
SELECT city, country FROM city
LEFT JOIN country ON city.id = country.country_id;
```

<p>Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.</p>

```sql
SELECT first_name, last_name FROM customer
RIGHT JOIN payment ON customer.id = payment.payment_id;
```

<p>Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.</p>

```sql
SELECT first_name, last_name FROM customer 
FULL JOIN rental ON customer.id = rental.rental_id;
```