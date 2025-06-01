# Примеры SQL-запросов для работы с данными

## Запрос 1
Написать запрос, который выведет сгруппированную по имени пользователя, типу объекта бронирования сумму тотал его бронирований (из таблицы Reservations), у которых рейтинг 4 и более. Результат отсортировать по убыванию суммы тотал бронирования.

```sql
select
    u.u_name,
    r.home_type,
    rev.rating,
    res.total
from reservations res
join users u on u.id = res.user_id
join revews rev on rev.reservation_id = res.id
join rooms r on r.id = res.room_id
where rev.rating >= 4
order by res.total desc

#2
Написать запрос, который выведет тип жилья, его адрес и стоимость за ночь, в адресе которого есть слово 'Avenue'.

select
    r.home_type,
    r.address,
    res.price 
from reservations res
join revews rev on rev.reservation_id = res.id
join rooms r on r.id = res.room_id
where r.address like '%Avenue%'

#3
В таблице 'rooms' изменить суточные цены за ночь в адресах c 80 на 90,а в адресе есть слово 'Avenue'.

update rooms
set price = 90
where address like '%Avenue%'
and price in (80);
commit;
