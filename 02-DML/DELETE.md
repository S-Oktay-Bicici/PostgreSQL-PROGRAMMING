``` sql

-- delete veri silmek için kullanılırken 
-- drop nesne silmek için kullanılır

CREATE TABLE users(
	ID 		INT,
	NAME 	VARCHAR(20)
	);

INSERT INTO users(ID,NAME) VALUES(5, 'OKTAY');

INSERT INTO users(ID, NAME)
VALUES(10, 'SADIK'),
	   (5,'BİÇİCİİ'),
	   (57,'SAMET');

--tüm veriyi siler 
DELETE FROM users;

-- id 5 e eşit olan verileri siler
DELETE FROM users 
WHERE ID = 5;

DELETE FROM users 
WHERE ID > 5;

-- delete silinen verinin diğer tablolardaki ilişkisine bakar

-- TRUNCATE ilişkilere bakmadan direkt siler 
TRUNCATE TABLE users;		  
```
#DELETE
#TRUNCATE