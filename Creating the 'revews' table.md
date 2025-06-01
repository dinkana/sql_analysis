# Создание таблицы 'revews'

```sql
-- Optional: Drop the table if it already exists
-- Опционально: Удаляем таблицу, если она уже существует
DROP TABLE IF EXISTS revews;

-- Create the 'revews' table
-- Создаем таблицу 'revews'
CREATE TABLE revews(
    id INTEGER NOT NULL PRIMARY KEY,
    reservation_id INTEGER,
    rating INTEGER
);

-- Insert data into the 'revews' table
-- Вставляем данные в таблицу 'revews'
INSERT INTO revews(id,reservation_id,rating) VALUES (1,1,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (2,3,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (3,4,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (4,5,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (5,8,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (6,9,3);
INSERT INTO revews(id,reservation_id,rating) VALUES (7,10,2);
INSERT INTO revews(id,reservation_id,rating) VALUES (8,12,2);
INSERT INTO revews(id,reservation_id,rating) VALUES (9,13,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (10,14,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (11,15,3);
INSERT INTO revews(id,reservation_id,rating) VALUES (12,16,2);
INSERT INTO revews(id,reservation_id,rating) VALUES (13,17,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (14,18,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (15,19,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (16,20,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (17,21,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (18,25,5);
INSERT INTO revews(id,reservation_id,rating) VALUES (19,26,4);
INSERT INTO revews(id,reservation_id,rating) VALUES (20,28,1);
INSERT INTO revews(id,reservation_id,rating) VALUES (21,29,2);
INSERT INTO revews(id,reservation_id,rating) VALUES (22,30,3);
