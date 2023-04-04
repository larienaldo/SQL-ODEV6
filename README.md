# SQL-ODEV6

## Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?

SELECT AVG (rental_rate) <br>
FROM film;

## Film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?

SELECT COUNT (title) <br>
FROM film <br>
WHERE title LIKE 'C%';

## Film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?

SELECT MAX (length) <br>
FROM film <br>
WHERE rental_rate = 0.99 ;

## Film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?

SELECT COUNT (DISTINCT replacement_cost) <br>
FROM film <br>
WHERE length > 150 ;
