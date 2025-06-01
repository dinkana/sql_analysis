# Создание таблицы 'rooms'

```sql
-- Optional: Drop the table if it already exists
DROP TABLE IF EXISTS rooms;

-- Create the rooms table
CREATE TABLE rooms(
    id INTEGER NOT NULL PRIMARY KEY,
    home_type VARCHAR(127) NOT NULL,
    address VARCHAR(255) NOT NULL,
    has_tv BOOLEAN NOT NULL,
    has_internet BOOLEAN NOT NULL,
    has_kitchen BOOLEAN NOT NULL,
    has_air_con BOOLEAN NOT NULL,
    price INTEGER,
    owner_id INTEGER,
    latitude NUMERIC,
    longitude NUMERIC
);

-- Insert sample data
INSERT INTO rooms(id,home_type,address,has_tv,has_internet,has_kitchen,has_air_con,price,owner_id,latitude,longitude) VALUES 
(1,'Private room','11218, Friel Place, New York','1','1','1','0',149,1,40.6475,-73.9633),
(2,'Entire home/apt','10018, 6th Avenue, New York','0','1','1','1',225,1,40.7536,-73.9634),
(3,'Private room','10027, West 128th Street, New York','1','0','0','1',150,2,40.809,-73.9635),
(4,'Entire home/apt','11238, Gates Avenue, New York','1','0','0','1',89,2,40.6851,-73.9636),
(5,'Entire home/apt','10029, Park Avenue, New York','0','1','1','1',80,3,40.7985,-73.9637),
(6,'Entire home/apt','10016, East 38th Street, New York','0','1','0','0',200,3,40.7477,-73.9638),
(7,'Private room','11216, Lexington Avenue, New York','0','0','1','1',60,4,40.6869,-73.9639),
(8,'Private room','10019, West 53rd Street, New York','1','0','0','1',79,14,40.7649,-73.9640),
(9,'Private room','10025, West 107th Street, New York','1','0','1','0',79,6,40.8018,-73.9641),
(10,'Entire home/apt','10002, Rutgers Street, New York','1','0','1','0',150,7,40.7134,-73.9642),
(11,'Entire home/apt','10025, West 109th Street, New York','1','1','0','0',135,8,40.8032,-73.9643),
(12,'Private room','10036, West 47th Street, New York','0','0','1','1',85,10,40.7608,-73.9644),
(13,'Private room','11215, 11th Street, New York','0','0','0','0',89,11,40.6683,-73.9645),
(14,'Private room','10025, West 106th Street, New York','0','0','0','1',85,12,40.7983,-73.9646),
(15,'Entire home/apt','10014, Perry Street, New York','1','0','0','1',120,13,40.7353,-73.9647),
(16,'Entire home/apt','11211, South 4th Street, New York','0','0','1','0',140,14,40.7084,-73.9648),
(17,'Entire home/apt','11205, Willoughby Avenue, New York','0','0','1','0',215,15,40.6917,-73.9649),
(18,'Private room','10011, West 21st Street, New York','1','1','0','1',140,16,40.7419,-73.9650),
(19,'Entire home/apt','11216, Bergen Street, New York','1','1','1','1',99,17,40.6759,-73.9651),
(20,'Entire home/apt','10026-2864, Duke Ellington Circle, New York','0','0','0','0',190,18,40.7968,-73.9652),
(21,'Entire home/apt','11249, North 8th Street, New York','1','1','1','1',299,19,40.7184,-73.9653),
(22,'Private room','11217, Saint Marks Avenue, New York','1','0','0','1',130,20,40.6807,-73.9654),
(23,'Private room','11217, 5th Avenue, New York','1','1','1','1',80,21,40.6799,-73.9655),
(24,'Private room','11217, 5th Avenue, New York','1','1','1','0',110,22,40.68,-73.9656),
(25,'Entire home/apt','11221, Hancock Street, New York','1','0','0','0',120,23,40.6837,-73.9657),
(26,'Private room','11218, Terrace Place, New York','1','1','0','0',60,24,40.656,-73.9658),
(27,'Private room','10034, Seaman Avenue, New York','1','1','0','0',80,25,40.8675,-73.9659),
(28,'Entire home/apt','10019, West 56th Street, New York','1','1','1','0',150,26,40.7672,-73.9660),
(29,'Private room','10034, Post Avenue, New York','1','0','0','0',44,27,40.8648,-73.9661),
(30,'Entire home/apt','10003, East 10th Street, New York','0','1','1','0',180,28,40.7292,-73.9854),
(31,'Private room','10031, West 140th Street, New York','0','0','1','1',50,29,40.8224,-73.951),
(32,'Private room','10027, West 126th Street, New York','0','0','1','1',52,30,40.813,-73.9547),
(33,'Private room','11222, Lombardy Street, New York','0','1','0','0',55,31,40.7222,-73.9376),
(34,'Private room','10031, West 138th Street, New York','1','0','1','0',50,32,40.8213,-73.9532),
(35,'Private room','11216, Jefferson Avenue, New York','1','0','0','0',70,32,40.6831,-73.9547),
(36,'Private room','11215, 10th Street, New York','1','0','0','1',89,32,40.6687,-73.9878),
(37,'Private room','11221, Lexington Avenue, New York','0','1','0','0',35,2,40.6888,-73.9431),
(38,'Entire home/apt','11237, Troutman Street, New York','1','0','1','0',85,1,40.7019,-73.9275),
(39,'Private room','11226, Marlborough Road, New York','0','1','0','0',150,25,40.637,-73.9633),
(40,'Shared room','10002, East Broadway, New York','1','1','1','1',40,25,40.714,-73.9892),
(41,'Private room','10009, East 4th Street, New York','0','0','0','0',68,25,40.7229,-73.982),
(42,'Entire home/apt','11215, 13th Street, New York','1','1','1','0',120,25,40.6628,-73.9797),
(43,'Private room','11205, Park Avenue, New York','1','0','1','1',120,12,40.6967,-73.9758),
(44,'Private room','10024, West 87th Street, New York','0','1','1','0',135,21,40.7901,-73.9793),
(45,'Entire home/apt','10027, West 130th Street, New York','0','1','1','0',150,21,40.8117,-73.9448),
(46,'Entire home/apt','11225, Ocean Avenue, New York','0','0','1','1',150,21,40.6594,-73.9624),
(47,'Private room','11101, 21st Street, New York','1','0','0','1',130,26,40.7477,-73.9474),
(48,'Entire home/apt','11207, Fulton Street, New York','1','1','0','0',110,16,40.6811,-73.9559),
(49,'Entire home/apt','11221, Throop Avenue, New York','1','1','0','0',115,15,40.6855,-73.9409),
(50,'Private room','11205, Washington Park, New York','1','0','1','1',80,15,40.6914,-73.9738);
