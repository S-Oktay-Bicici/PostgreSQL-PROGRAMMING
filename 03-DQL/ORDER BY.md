``` sql

-- birşey yazılmadığı durumda ASC olarak alır
--ASC alfabetik ve nümerik sıraya göre sıralar 
SELECT * FROM sütun_ismi
FROM tablo_ismi
ORDER BY sütun_ismi ASC;

-- DESC tersine sıralam yapar  
SELECT * FROM sütun_ismi
FROM tablo_ismi
ORDER BY sütun_ismi DESC;

-- farklı sütünları farklı srılama işlemi
SELECT * FROM sütun_ismi
FROM tablo_ismi
ORDER BY sütun_ismi ASC, sütun_ismi2 DESC;

-- verilen sütuna göre sılama işlemi yapıyor 
-- aynı değerleri çıkararak
SELECT DISTINCT sütun_ismi
FROM tablo_ismi
ORDER BY sütun_ismi ASC;
```

#ORDER BY
#ASC
#DESC
