CREATE USER kullanici_adi
[WITH PASSWORD 'şifre bu kısıma' | VALID UNTIL ' TARİH']

CREATE USER oktay
WITH PASSWORD 'oktayoktay';

CREATE USER sadık
WITH PASSWORD 'oktayoktay'
VALID UNTIL 'Jan 1, 2020';

CREATE USER sadık
WITH PASSWORD 'oktayoktay'
VALID UNTIL 'infinity';


grant ile oluşturudğumuz kullanıcıya izin veriyoruz 

-- Kullanıcıya hangi işlemleri hangi tablo üzerinde vereceğimizi belirliyoruz
GRANT SELECT,INSERT,UPDATE,DELETE ON 'tablo ismi' TO oktay;

-- tüm işlemleri belirli tablo üzerinden belirli kişiye verebiliryoruz
GRANT ALL ON 'tablo ismi' TO oktay;

-- yada belrili bir işlemi herekese açık yapabiliriz
GRANT SELECT ON 'tablo ismi' TO PUBLİC;
