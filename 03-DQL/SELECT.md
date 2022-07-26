``` sql

-- tablo içindeki tüm sütunları çeker
SELECT * FROM tablo_ismi;

SELECT tablo_1, tablo_2 FROM tablo_ismi;

-- String birleştirme ve Takma isim kullanımı
SELECT sutun1, sutun2 AS yeni_isim FROM tablo_ismi

SELECT * FROM tablo_ismi WHERE sutun1 < 100;

SELECT * FROM tablo_ismi WHERE sutun1 <= 100;

SELECT * FROM tablo_ismi WHERE sutun1 <> 100;

SELECT * FROM tablo_ismi WHERE sutun1 = 'king';

SELECT * FROM tablo_ismi WHERE sutun1 != 100;

SELECT 2 + 3;
SELECT 2 * 3;
SELECT 10 / 5;
SELECT 14 % 4 AS sonuc;


SELECT 'SADIK' || 'OKTAY' || 'BİÇİCİ' AS full_name;
SELECT 'ABC' || 2 AS result; --> eror
SELECT 'ABC' || NULL AS result; --> null

SELECT CONCAT('SADIK','OKTAY','BİÇİCİ');
SELECT CONCAT('ABC', NULL); --> ABC
SELECT CONCAT('ABC', 5); --> ABC5

SELECT first_name
CONCAT('ADINIZ', LENGTH(first_name), 'karakter uzunluğundadır') AS uzunluk
FROM tablo_ismi;

-- belirlenen karakteri birleştirilen değerler arasına katarak işlemi yapıyor
SELECT 
CONCAT_WS(',',last_name,first_name) AS full_name
FROM tablo_ismi
ORDER BY last_name;

SELECT * FROM tablo_ismi
WHERE ID = 10 AND MAAS >= 6000;

SELECT * FROM tablo_ismi
WHERE ID = 10 OR MAAS >= 6000;

-- belirlenen değerler arasındaki veriyi döndürür
SELECT * FROM tablo_ismi
WHERE MAAS BETWEEN 4500 AND 6000;

-- belirlenen kayıtlarlar dışındaki veriyi döndürür
SELECT * FROM tablo_ismi
WHERE MAAS NOT BETWEEN 4500 AND 6000;

-- ismi ok ile başlayan uzunluğu belirlisz her ismi döndürür
SELECT first_name, last_name
FROM tablo_ismi
WHERE first_name LIKE 'OK%'

-- ismin son iki karakterine bakarak var olan tüm veriyi döndürür
SELECT first_name, last_name
FROM tablo_ismi
WHERE first_name LIKE '%AY'

-- ikinci karakteri k olan isimleri döndürür
SELECT first_name, last_name
FROM tablo_ismi
WHERE first_name LIKE '_K%'

-- toplam 5 karakterli sonu y ile biten isismleri döndürür
SELECT first_name, last_name
FROM tablo_ismi
WHERE first_name LIKE '____y'

-- ilk 4 kaydı getirir
SELECT first_name, last_name
FROM tablo_ismi LIMIT 4;

-- ilk 2 kaydı atlayıp 4 kaydı getirir
SELECT first_name, last_name
FROM tablo_ismi LIMIT 4 OFFSET 2;

SELECT * FROM sütun_ismi
FROM tablo_ismi
ORDER BY sütun_ismi DESC
LIMIT 5 OFFSET 1;

-- tablo1 ve tablo2 de aynı sütünları birleştirerek getirir(tekrarları atar)
SELECT sütun_ismi FROM tablo_1
UNION
SELECT sütun_ismi FROM tablo_2;

-- tekralı olanlarla birlikte birleştirip getirir
SELECT sütun_ismi FROM tablo_1
UNION ALL
SELECT sütun_ismi FROM tablo_2;

-- 2 tabloda kesişen değerleri getirir
SELECT sütun_ismi FROM tablo_1
INTERSECT
SELECT sütun_ismi FROM tablo_2;

-- sutunun ortalamasını bulur
SELECT AVG(sutun_ismi) FROM tablo;

-- sutun içerisindeki veri sayısını döndürür
SELECT COUNT(sutun_ismi) FROM tablo;
SELECT COUNT(DISTINCT sutun_ismi) FROM tablo;

-- sutundaki en yüksek değeri döndürür
SELECT MAX(sutun_ismi) FROM tablo;

-- sutundaki en düşük değeri döndürür
SELECT MIN(sutun_ismi) FROM tablo;

-- sütundaki değerlerin toplamını döndürür
SELECT SUM(sutun_ismi) FROM tablo;
SELECT SUM(DISTINCT sutun_ismi) FROM tablo;

-- customer id'si 1 ve 2 olan değerleri döndürür
SELECT customer_id
FROM tablo_1
WHERE customer_id IN(1,2);

-- 1 ve 2 değerlieri hariç hepsini getirir
SELECT customer_id
FROM tablo_1
WHERE customer_id NOT IN(1,2);

-- string fonksiyonları
SELECT CHAR_LENGHT('POSTGRESQL'); --> UZUNLUK VERİR
SELECT LENGHT('POSTGRESQL'); --> UZUNLUK VERİR

SELECT LOWER('PostgreSql'); --> karakterleri küçültür

SELECT UPPER('PostgreSql'); --> karakterleri büyültür

SELECT SUBSTR('soktaybicici.com',2,5); -->oktay

SELECT POSITION('ha' IN 'Merhaba'); --> 4

SELECT ASCII('A'); --> 97

SELECT INITCAP ('hi hello'); --> Hi Hello

SELECT REPEAT ('Hİ', 3); --> HİHİHİ

SELECT REVERSE ('OLLEH'); --> HELLO
``` 

#SELECT
#WHERE
#CONCAT
#CONCAT_WS
#AND
#OR 
#NOT 
#BETWEEN
#LIKE
#LIMIT
#OFFSET
#UNION
#UNIONALL
#AVG
#IN 
#NOT IN
[[INNER JOIN]]
[[LEFT JOIN]]
[[RIGHT JOIN]]
[[FULL OUTER JOIN]]
[[CROSS JOIN]]
[[SELF JOIN]]