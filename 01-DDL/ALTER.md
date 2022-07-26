ALTER TABLE tablo_ismi [aksiyon]

- Columns --> Add,Delete(Drop),Modify, Rename
- Constraints --> Add,Drop
- Index --> Add,Drop


``` SQL
CREATE TABLE users(
	ID		INT
);

-- tabloya ekleme yapıyrouz
ALTER TABLE users ADD gender CHAR(1);
	
-- tablodan silme yapıyoruz	
ALTER TABLE users DROP gender;

-- var olan ismi değiştiriyrouz
ALTER TABLE users RENAME TO People;

-- tabloaya ekleme yapıyoruz
ALTER TABLE users ADD COLUMN "isActive" BIT(1);

--sütun ismini değiştiriyroz
ALTER TABLE users RENAME COLUMN gender TO gender_title;

-- tablodaki sütunun kısıtlamasını değiştiriyoruz
ALTER TABLE tablo_ismi ALTER COLUMN sütun_ismi SET NOT NULL;

-- sütuna primary key atıyrouz
ALTER TABLE tablo_ismi ADD PRIMARY KEY sütun_ismi;

-- sütunun kısıtlamasını değiştiriyoruz
ALTER TABLE tablo_ismi ADD CONSTRAINT sütun_ismi CHECK (sütun_ismi>=100);
``` 
