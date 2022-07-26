revoke verilen izinlerin geri alınmasında kullanılır.


``` SQL
-- Kullanıcıya hangi işlemleri hangi tablo üzerinde alacağımızı belirliyoruz
GRANT SELECT,INSERT,UPDATE,DELETE ON 'tablo ismi' TO oktay;

-- tüm işlemleri belirli tablo üzerinden belirli kişiye alabiliryoruz
GRANT ALL ON 'tablo ismi' TO oktay;

-- yada belrili bir işlemi herekese kapalı yapabiliriz
GRANT SELECT ON 'tablo ismi' TO PUBLİC;
``` 
