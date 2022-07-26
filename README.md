# SQL Sorguları 

## 1- DDL - Data Definition Language ( Veri Tanımlama Dili )
[[CREATE]] --> Veritabanında nesne oluşturmak için kullanılır.
[[ALTER]] --> Mevcut bir nesenenin yapısını değiştirmek için kullanılır.
[[DROP]] --> Bir nesneyi silmek için kullanılır.
	
## 2- DML - Data Manipulation Language ( Veri İşleme Dili )
[[INSERT]] --> Veri ekleme amacıyla kullanılır
[[UPDATE]] --> Veri güncelleme amacıyla kullanılır
[[DELETE]] --> Veri silme amacıyla kullanılır

## 3- DQL - Data Query Language ( Veri Sorgu Dili )
[[SELECT]]
[[ORDER BY]]
[[GROUP BY]]
	
## 4- DCL - Data Control Language ( Veri Kontrol Dili )
[[GRANT]]
[[REVOKE]]
	
## 5- TCC - Transactional Control Commands ( İşlemsel Kontrol Komutları )
[[COMMIT]]
[[ROLLBACK]]
	
	
Örnek kodlar [[hr-sql-sorguları.sql]]


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
