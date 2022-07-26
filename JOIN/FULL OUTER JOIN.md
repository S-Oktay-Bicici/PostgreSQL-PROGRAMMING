``` sql

SELECT tablo_1.sutun_1, tablo_2.sutun2
FROM tablo_1
FULL JOIN tablo_2
ON tablo_1.sutun = tablo_2.sutun;

SELECT 
	a.name,
	a.surname,
	a.age,
	b.sales,
	b.customer_name,
	b.customer_surname
FROM sales_22015 AS a
FULL JOIN customer_22015 AS b
ON a.customer_id = b.customer_id
ORDER BY customer_id;
	
``` 