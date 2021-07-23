# warehouse_manager
#### developed by Nikita Kuznetsov

### формулировка тз

* [ ] регистрация/авторизация/выход
* [ ] админка

<br>

* [ ] записью являются товар/предмет, склад
* [ ] Пользователь может “заказывать поставку” (покупать на склад), “списывать” (удалить со склада)
* [ ] Можно оценить стоимости содержимого
* [ ] Можно оценить остатки (колличество товаров на складе)
* [ ] Опционально:
  * [ ] Сроки поставок (задержка между заказом и поступлением на склад)
  * [ ] ❓Оценка будущей необходимости (планирование) 
  * [ ] ❓Напоминания: заказать недостающее, истечение срока годности 


## REST API

* [ ] вход: <br> 
  `POST:http://host/login`
* [ ] выход: <br> 
  `GET:http://host/logout`
* [ ] регистрация: <br> 
  `POST:http://host/register`
  
  
* [ ] список складов: <br>
  `GET:http://host/warehouses`
* [ ] информация о складе по его id: 
  `GET:http://host/warehouses/<warehouse_id>`
  * [ ] стоимость всех его товаров
  * [ ] колличество товаров
* [ ] создать пустой склад: <br>
  `POST:http://host/warehouses`
* [ ] изменить информацию о складе: 
  `PUT:http://host/warehouses/<warehouse_id>`
* [ ] удалить лишний склад:
  `DELETE:http://host/warehouses/<warehouse_id>`
  
  
* [ ] список товаров на складе: 
  `GET:http://host/warehouses/<warehouse_id>/items`
* [ ] информация о товаре по его id: 
  `GET:http://host/warehouses/<warehouse_id>/items/<item_id>`
* [ ] создать товар с заданными характеристиками: 
  `POST:http://host/warehouses/<warehouse_id>/items`
* [ ] изменить характеристики товара: 
  `PUT:http://host/warehouses/<warehouse_id>/items/<item_id>`
* [ ] удалить товар со склада: 
  `DELETE:http://host/warehouses/<warehouse_id>/items/<item_id>`
  