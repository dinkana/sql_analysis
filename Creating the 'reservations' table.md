# Создание таблицы 'reservations'

```sql
DROP TABLE IF EXISTS reservations;

CREATE TABLE reservations(
    id INTEGER NOT NULL PRIMARY KEY,
    user_id INTEGER NOT NULL,
    room_id INTEGER NOT NULL,
    start_date DATE NOT NULL,
    end_date DATE NOT NULL,
    price INTEGER NOT NULL,
    total INTEGER NOT NULL
);

INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (1,1,1,'2018-11-13','2018-11-15',140,980);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (2,2,1,'2018-10-09','2018-10-12',120,360);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (3,12,1,'2018-12-29','2019-01-07',180,2520);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (4,13,1,'2019-02-01','2019-02-02',145,420);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (5,17,1,'2019-02-02','2019-02-04',149,777);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (6,14,2,'2020-03-21','2020-03-23',225,719);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (7,19,13,'2020-03-21','2020-04-21',89,3511);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (8,29,16,'2019-06-14','2019-06-24',140,1005);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (9,32,21,'2019-05-11','2019-05-14',270,708);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (10,13,21,'2019-11-04','2019-11-06',280,1485);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (11,9,21,'2020-02-28','2020-02-29',290,504);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (12,7,19,'2020-05-01','2020-05-02',99,581);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (13,15,8,'2020-01-19','2020-01-21',78,354);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (14,13,7,'2019-09-13','2019-09-17',60,1874);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (15,12,5,'2020-05-14','2020-05-15',80,375);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (16,10,5,'2020-03-26','2020-03-27',80,870);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (17,11,50,'2019-11-18','2019-11-25',80,450);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (18,27,49,'2019-09-18','2019-09-20',110,230);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (19,28,49,'2020-04-01','2020-04-02',115,600);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (20,1,49,'2020-06-01','2020-06-11',115,2578);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (21,2,48,'2019-11-07','2019-11-10',110,872);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (22,12,32,'2020-01-14','2020-01-18',52,878);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (23,12,32,'2019-09-17','2019-09-18',52,752);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (24,7,19,'2020-01-08','2020-01-11',99,1457);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (25,18,19,'2019-11-01','2019-11-16',99,240);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (26,21,17,'2019-11-03','2019-11-05',215,340);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (27,31,25,'2020-04-20','2020-04-22',120,2150);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (28,21,14,'2020-02-08','2020-02-12',85,555);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (29,21,39,'2019-12-08','2019-12-09',150,800);
INSERT INTO reservations(id,user_id,room_id,start_date,end_date,price,total) VALUES (30,3,38,'2020-03-20','2020-03-23',185,1500);
