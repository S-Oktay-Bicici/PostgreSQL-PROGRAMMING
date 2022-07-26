``` sql
CREATE TABLE users(
	ID 		INT,
	NAME 	VARCHAR(20)
	);

INSERT INTO users(ID,NAME) VALUES(5, 'OKTAY');

INSERT INTO users(ID, NAME)
VALUES(10, 'SADIK'),
			  (5,'BİÇİCİİ'),
			  (57,'SAMET');

-- Single UPDATE
			  
UPDATE users
SET NAME = 'SADIK'
WHERE ID = 10;

-- Multiple UPDATE
-- tüm isim değerlerini x olarak değiştirir
UPDATE users
SET NAME = 'x'
			  
```
#UPDATE