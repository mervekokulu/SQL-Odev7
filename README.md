# SQL-Odev7

1. film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.

`SELECT rating, COUNT (*) FROM film`<br>
`GROUP BY rating;`

2. film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

`SELECT replacement_cost, COUNT (*) from film`<br>
`GROUP BY replacement_cost`<br>
`HAVING COUNT (*) > 50;`

3. customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir? 

`SELECT store_id, COUNT (*) FROM customer`<br>
`GROUP BY store_id;`

4. city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

`SELECT country_id, COUNT (*) FROM city`<br>
`GROUP BY country_id`<br>
`ORDER BY COUNT (*) DESC`<br>
`LIMIT 1;`
