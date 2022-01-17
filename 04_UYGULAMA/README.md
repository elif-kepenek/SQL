<p>Film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.</p>

```sql
SELECT DISTINCT(replacement_cost) FROM film;
```

<p>Film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?</p>

```sql
SELECT COUNT(DISTINCT(replacement_cost)) FROM film;
```

<p>Film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?</p>

```sql
SELECT COUNT(title) FROM film
WHERE title LIKE 'T%' AND rating = 'G';
```

<p>Country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?</p>

```sql
SELECT COUNT(country) FROM country
WHERE country LIKE '_____';
```

<p>City tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?</p>

```sql
SELECT city FROM city
WHERE city ILIKE '%r';
```