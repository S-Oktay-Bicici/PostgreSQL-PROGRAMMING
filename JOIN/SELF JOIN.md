``` sql

SELECT sütun_ismi
FROM tablo_1
INNER JOIN tablo_2
ON tablo1.sütun_ismi = tablo_2.sütun_ismi;

SELECT 
	a.name,
	a.surname,
	a.age,
	b.sales,
	b.customer_name,
	b.customer_surname
FROM sales_22015 AS a
INNER JOIN customer_22015 AS b
ON a.customer_id = b.customer_id
ORDER BY customer_id;
	
``` 