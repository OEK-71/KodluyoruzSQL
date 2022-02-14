# Homework 8  
1- test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

- CREATE TABLE employee (id SERIAL PRIMARY KEY, name varchar(70), birthday date, email varchar(100));

2- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

- insert info employee(name,birthday,email) values ('Tom','1997-06-06','tom97@squidoo.com');
- insert info employee(name,birthday,email) values ('Bard','1987-03-01','drab@discovery.com');
- insert info employee(name,birthday,email) values ('Matt','1968-11-01','mat681101@about.com');
- insert info employee(name,birthday,email) values ('Tom','1972-01-22','tom220172@outlook.com');

3- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

- Update employeee set name = 'Onur',birthday = '1997-06-03', email = 'onur@gmail.com' WHERE id BETWEEN 3 AND 8 returning *;

4- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

DELETE from employee WHERE id BETWEEN 3 and 8 returning *;
