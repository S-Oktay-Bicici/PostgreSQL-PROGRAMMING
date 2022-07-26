

``` sql
-- Database oluşturuyoruz

CREATE DATABASE MyData;
```


``` sql
-- Oluşturduğumuz database'e tablo oluşturuyoruz ve sütun ekliyoruz

CREATE TABLE regions( 
	region_id      SERIAL  primary key,       
	region_name    VARCHAR(25) );
```
	
her sütunun veri türünü ve kısıtalamsını tanımlamayoruz. 

### Kısıtlamalar 
- NOT NULL --> Veritabanındaki bir sütunun boş geçilememesini sağlar. 
- DEFAULTS --> bir sütun için varsayılan bir değer sağlar.
- UNIQUE --> •Veritabanı tablosundaki verilerin benzersizliğini garanti etmek için kullanılır.
- CHECK --> •Bir veritabanı tablosu üzerinde gerçekleşen INSERT ve UPDATE işlemlerinde verinin kontrol edilmesi ve şart oluşturulmasını sağlar.
- Primary Key --> Tablonun sorgulanmasında hem kullanıcı hem de sistem tarafından en çok kullanılacak ve gerekli olan sütunu tanımlar.
- Foreign Key --> V•Birden fazla tablonun JOIN ile birleştirilmesi işlemlerinde birincil tablonun ikincil tablolardaki referansına denir.

### AS Kullanımı

``` sql
-- tablo1 ile aynı yapıda tablo adında bir tablo oluşturduk 

>CREATE TABLE tablo AS (SELECT * FROM tablo1) WITH NO DATA;
```
--- 

### SERIAL --> Otomatik artan sütunlu tablo oluşturmak için kullanılır

- SMALLSERIAL --> 2 bytes
- SERIAL            --> 4 bytes
- BIGSERIAL      --> 8 bytes


``` sql
CREATE TABLE tablo_seri(
	ID			SERIAL,
	AD			VARCHAR);
```

### SEQUENCE --> Otomatik artan sütun oluşturmak

``` sql
CREATE SEQUENCE demo_table_seq;
CREATE SEQUENCE demoTable(
	ID 			INTEGER  DEFAULT nextval('demo_table_seq'),
	Name 	TEXT );
```

### TEMP --> Geçici tablo oluşturmak

``` sql
CREATE TEMP TABLE demo_temp_table(
	ID 		INT);
```

> [!Data Types ] 
>Numeric
>Character String
>Date/Datetime


>Numeric 
- smallint --> 2 bytes
- integer --> 4 bytes
- bigint --> 8 bytes 
- decimal --> variable
- SMALLSERIAL --> 2 bytes
- SERIAL            --> 4 bytes
- BIGSERIAL      --> 8 bytes


> Character
- character varying,  varchar(n)
- character(n), char(n)
- text

>Date time
- timestamp --> 8 bytes
- date --> 4 bytes
- time --> 8 bytes
- interval --> 12 bytes


#CREATE
#AS
#SERIAL
#SEQUENCE
#TEMP
