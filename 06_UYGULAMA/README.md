<p>Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?</p>

```sql
SELECT AVG(rental_rate) FROM film;
```

<p>Film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?</p>

```sql
SELECT COUNT(title) FROM film
WHERE title LIKE 'C%';
```

<p>Film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?</p>

```sql
SELECT MAX(length) FROM film
WHERE rental_rate = 0.99;
```

<p>Film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?</p>

```sql
SELECT COUNT(DISTINCT(replacement_cost)) FROM film
WHERE length > 150;
```