<p>Country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.</p>

```sql
SELECT country FROM country
WHERE country LIKE 'A%a';
```

<p>Country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.</p>

```sql
SELECT country FROM country
WHERE country LIKE '______%n';
```

<p>Film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.</p>

```sql
SELECT title FROM film
WHERE title ILIKE '%t%t%t%t%';
```

<p>Film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.</p>

```sql
SELECT * FROM film
WHERE title LIKE 'C%'
WHERE length > 90 AND rental_rate = 2.99;
```