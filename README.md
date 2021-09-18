# SQL_ODEV10
**Patika SQL eğitimi kapsamında yaptığım ödev10.**
----------------
1._city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız._
```sql
SELECT city, country FROM city 
LEFT JOIN country ON city.country_id=country.country_id;
```
2._customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız._
```sql
SELECT  payment_id, first_name, last_name FROM customer
RIGHT JOIN payment ON payment.customer_id = customer.customer_id ;
```
3._customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız._
```sql
SELECT  rental_id, first_name, last_name FROM customer
FULL JOIN rental ON rental.customer_id = customer.customer_id ;
```
----------------------
**Sorgu senaryolarını [dvdrental.tar](https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip) isimli dosyayı indirerek gerçekleştirebilirsiniz.**
