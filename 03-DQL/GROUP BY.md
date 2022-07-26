
``` sql

-- DISTINCT görevi görerek aynı olan veriden tek alarak gruplar ve dönüdrür
SELECT * FROM sütun_ismi
FROM tablo_ismi
GROUP BY sütun_ismi;

SELECT sütun_ismi,
COUNT(customer_id) AS customer_count
FROM customer
GROUP BY region;

SELECT product_id,
SUM(quantity) AS quantity_sold
FROM sales
GROUP BY product_id
ORDER BY quantity_sold DESC;


SELECT customer_id,
MIN(sales) AS min_sales,
MAX(sales) AS max_sales,,
AVG(sales) AS Average_sales,
SUM(sales) AS Total_sales
FROM sales
GROUP BY customer_id
ORDER BY total_sales DESC
LIMIT 5;


SELECT customer_id, SUM(amount)
FROM payment
GROUP BY customer_id
HAVING SUM(amount) > 200;

```

#GROUP BY
#HAVING