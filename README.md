# SQL Sorguları 

## 1- DDL - Data Definition Language ( Veri Tanımlama Dili )
CREATE --> Veritabanında nesne oluşturmak için kullanılır.<br>
ALTER --> Mevcut bir nesenenin yapısını değiştirmek için kullanılır.<br>
DROP --> Bir nesneyi silmek için kullanılır.<br>
	
## 2- DML - Data Manipulation Language ( Veri İşleme Dili )
INSERT --> Veri ekleme amacıyla kullanılır<br>
UPDATE --> Veri güncelleme amacıyla kullanılır<br>
DELETE --> Veri silme amacıyla kullanılır<br>

## 3- DQL - Data Query Language ( Veri Sorgu Dili )
SELECT<br>
ORDER BY<br>
GROUP BY<br>
	
## 4- DCL - Data Control Language ( Veri Kontrol Dili )
GRANT<br>
REVOKE<br>
	
## 5- TCC - Transactional Control Commands ( İşlemsel Kontrol Komutları )
COMMIT<br>
ROLLBACK<br>
	
	
Örnek kodlar
* hr-sql-sorguları.sql
* Adventureworks - OLTP database for a fictitious, multinational manufacturing company called Adventure Works Cycles
* Chinook - digital media store
* French Towns - all French towns and regions
* ISO-3166 - All countries and subcountries in the world
* Pagila - Movie rental database with actors, ratings, payments, etc.
* Role Based Access Control - authentication solution
* USDA - food database
* World - Cities, Countries, and what language they speak


> [!NOTE] 
>Veri --> ham(işlenmemiş) gerçek enformasyon parçacığına verilen isimdir. Veriler ölçüm, sayım, deney, gözlem ya da araştırma yolu ile elde edilmektedir.
	

> [!NOTE] 
> Bilgi -->Toplanan verilerin işlenmesi sonucunda ortaya çıkan anlamlandırılmış veri bütünüdür.	

> [!NOTE]
> Veritabanı 
> - Birbiriyle ilişkili ya da ilişkisiz verilerin belirli bir düzen içerisinde depolandığı özel yazılımlardır.
> - Ticari bir veritabanı yazılımı en temel seviyede ANSI-SQL standardını desteklemek zorundadır.
> - Veritabanlarındaki veriler sorgulanabilir, değiştirilebilir ve silinebilirlerdir.
> - Veritabanı veriyi disk üzerinde tutar. Yani veriler bilgisayara kayıtlıdır. Ancak bunlar normal dosya formatında olmadığı için kullanıcılar tarafından bu verilere erişilemez. Bu verilere sadece ilgili veritabanı yazılımının SQL motoru tarafından erişilebilir.
> - Bir veritabanı sistemi kendi SQL sorgu betiğiyle sorgulanabileceği gibi, dış sistemlere entegre amacıyla geliştirilen erişim araçlarıyla(driver) da sorgulanabilir.
> - Bir veritabanı programlarken en temel nesnelerden birisi connection’dır. Bu bağlantı nesnesi sayesinde veritabanı motoruna erişim iznine sahip oluruz. Bu bir sorgu editörü de olabilir, harici ve kendi geliştirdiğiniz bir uygulama da olabilir. Hepsi veritabanı motoru üzerinde bir bağlantı açar ve tüm işlemler bu bağlantı üzerinden yönetilir.
	
> [!NOTE]
> SQL Türleri 
> - SQL Server  : Transact-SQL (T-SQL)
> - Oracle  : Procedurel SQL (PL/SQL)
> - PostgreSQL  : PL/pgSQL
