<p>City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.</p>

```sql
SELECT city, country FROM city
INNER JOIN country ON city.id = country.country_id;
```

<p>Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.</p>

```sql
SELECT first_name, last_name FROM customer
INNER JOIN payment ON payment.payment_id = customer.id;
```

<p>Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.</p>

```sql
SELECT rental.rental_id, first_name, last_name FROM customer 
INNER JOIN rental ON cutomer.id = rental.rental_id;
```