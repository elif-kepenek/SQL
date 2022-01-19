<p>Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.</p>

```sql
CREATE DATABASE test;
```

```sql
CREATE TABLE employee (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    birthday DATE,
    email VARCHAR(100)
)
```

<p>Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.</p>

```sql
insert into employee (name, birthday, email) values ('Robbin Dammarell', '2007-08-18', 'rdammarell0@angelfire.com');
insert into employee (name, birthday, email) values ('Yves Siddons', '1952-04-20', 'ysiddons1@wiley.com');
insert into employee (name, birthday, email) values ('Noelani Faragan', '2018-11-29', 'nfaragan2@java.com');
insert into employee (name, birthday, email) values ('Suzanna Stanney', '1954-04-08', 'sstanney3@51.la');
insert into employee (name, birthday, email) values ('Dulsea Spiaggia', '2006-03-29', 'dspiaggia4@cnbc.com');
insert into employee (name, birthday, email) values ('Annecorinne Leuchars', '1964-11-03', null);
insert into employee (name, birthday, email) values ('Rosaleen Thow', '1998-11-12', 'rthow6@berkeley.edu');
insert into employee (name, birthday, email) values ('Desi Phinn', '1969-06-13', 'dphinn7@jalbum.net');
insert into employee (name, birthday, email) values ('Ignace Moncrefe', '1958-12-10', 'imoncrefe8@tripadvisor.com');
insert into employee (name, birthday, email) values ('Catlaina Jervis', '1989-05-25', 'cjervis9@printfriendly.com');
insert into employee (name, birthday, email) values ('Cathrin Aizikovich', '1986-07-08', null);
insert into employee (name, birthday, email) values ('Eirena Stutard', '1971-02-19', 'estutardb@ehow.com');
insert into employee (name, birthday, email) values ('Kellie Grummitt', '1989-12-05', 'kgrummittc@printfriendly.com');
insert into employee (name, birthday, email) values ('Jackelyn Champkins', '1981-02-17', null);
insert into employee (name, birthday, email) values ('Walker Dollard', '1974-09-20', null);
insert into employee (name, birthday, email) values ('Linell Lindsley', '2008-07-22', 'llindsleyf@narod.ru');
insert into employee (name, birthday, email) values ('Abramo Phillip', '1969-04-28', null);
insert into employee (name, birthday, email) values ('Lucretia Stannas', '1982-07-31', null);
insert into employee (name, birthday, email) values ('Vally McGhee', '1977-06-08', 'vmcgheei@so-net.ne.jp');
insert into employee (name, birthday, email) values ('Livy Millimoe', '2001-10-14', null);
insert into employee (name, birthday, email) values ('Inesita Barnaby', '1989-05-26', 'ibarnabyk@wikia.com');
insert into employee (name, birthday, email) values ('Duky Dorber', '1959-03-05', null);
insert into employee (name, birthday, email) values ('Cally Doring', '2002-05-28', 'cdoringm@bizjournals.com');
insert into employee (name, birthday, email) values ('Gianni Hansen', null, 'ghansenn@npr.org');
insert into employee (name, birthday, email) values ('Ranna Verna', '1958-08-11', 'rvernao@house.gov');
insert into employee (name, birthday, email) values ('Art Blakeley', '1989-11-18', 'ablakeleyp@tiny.cc');
insert into employee (name, birthday, email) values ('Walden Peris', '2019-04-04', 'wperisq@nhs.uk');
insert into employee (name, birthday, email) values ('Binnie Ghidini', '1966-08-25', 'bghidinir@amazon.co.uk');
insert into employee (name, birthday, email) values ('Chrissie Surphliss', '1951-06-26', 'csurphlisss@sbwire.com');
insert into employee (name, birthday, email) values ('Timothea Hinchshaw', '2002-07-16', 'thinchshawt@google.com');
insert into employee (name, birthday, email) values ('Willi Pickerill', '2011-12-21', null);
insert into employee (name, birthday, email) values ('Aylmar Rennie', '2021-07-27', 'arenniev@cargocollective.com');
insert into employee (name, birthday, email) values ('Ashbey Landrieu', null, 'alandrieuw@state.gov');
insert into employee (name, birthday, email) values ('Daffi Ludford', '1963-10-28', 'dludfordx@blogtalkradio.com');
insert into employee (name, birthday, email) values ('Aimee Funcheon', '1971-08-25', 'afuncheony@google.com.au');
insert into employee (name, birthday, email) values ('Kenn Buxey', '1988-03-24', 'kbuxeyz@fastcompany.com');
insert into employee (name, birthday, email) values ('Frazer Happer', '1975-06-15', 'fhapper10@homestead.com');
insert into employee (name, birthday, email) values ('Dosi Lilly', '2000-10-20', 'dlilly11@purevolume.com');
insert into employee (name, birthday, email) values ('Ezmeralda Woolland', '2005-07-01', 'ewoolland12@economist.com');
insert into employee (name, birthday, email) values ('Brock Vevers', '1967-05-23', 'bvevers13@shop-pro.jp');
insert into employee (name, birthday, email) values ('Prisca Inch', '2014-03-04', 'pinch14@w3.org');
insert into employee (name, birthday, email) values ('Mimi Ronisch', '1988-07-16', 'mronisch15@sfgate.com');
insert into employee (name, birthday, email) values ('Fonz Masurel', '2014-06-30', 'fmasurel16@youtu.be');
insert into employee (name, birthday, email) values ('Sherman Rule', '2018-03-22', null);
insert into employee (name, birthday, email) values ('Jodie Hurley', '2004-08-04', 'jhurley18@themeforest.net');
insert into employee (name, birthday, email) values ('Willey McCahill', '1996-06-06', 'wmccahill19@artisteer.com');
insert into employee (name, birthday, email) values ('Nehemiah Stubbe', '2005-11-23', null);
insert into employee (name, birthday, email) values ('Mord Moryson', '1979-07-10', 'mmoryson1b@uol.com.br');
insert into employee (name, birthday, email) values ('Any Varga', '1980-11-09', 'avarga1c@taobao.com');
insert into employee (name, birthday, email) values ('Orren Bahlmann', '1988-05-16', null);
```

<p>Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.</p>

```sql
UPDATE employee
SET name = 'Thom Yorke'
WHERE id = 1;
```

```sql
UPDATE employee
SET email = 'thom@yorke.com'
WHERE id = 1;
```

```sql
UPDATE employee
SET birthday = '1968-10-07'
WHERE id = 1;
```

```sql
UPDATE employee
SET email = null
WHERE id < 5;
```

```sql
UPDATE employee
SET birthday = null
WHERE id > 45;
```

<p>Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.</p>

```sql
DELETE FROM employee
WHERE id = 15;
```

```sql
DELETE FROM employee
WHERE name = 'Thom Yorke';
```

```sql
DELETE FROM employee
WHERE birthday = '2019-04-04';
```

```sql
DELETE FROM employee
WHERE email LIKE '%ğ%';
```

```sql
DELETE FROM employee
WHERE id > 48;
```