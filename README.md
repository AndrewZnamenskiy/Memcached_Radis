# Домашнее задание к занятию «Кеширование Redis/memcached»

---

### Задание 1. Кеширование 

Приведите примеры проблем, которые может решить кеширование. 

*Приведите ответ в свободной форме.*

### Решение 2

#### Команды запуска  Python Web серверов

* Повышение производительности достигается за счет складывания в кэш данных, к которым чаще всего происходит обращение;
* Увеличение скорости ответа;
* Экономия ресурсов базы данных, например, применяя кэширование тяжелых запросов;
* Сглаживание бустов трафика. Например, во время черной пятницы онлайн-магазины используют кэш, чтобы переживать резкое увеличение трафика.

Например, применение кэширования веб страниц интернет магазинов позволяет сохранять в
кэш наиболее часто запрашиваемые продукты их описания и картинки. Поскольку кэширующие 
базы размещены в оперативной памяти, отклик на запросы очень быстрый, в тоже время 
нагрузка на основную БД существенно снижается.

Другим примером может служить кэширующий DNS сервер, выдающий разрешнение часто запрашиваемых доменных имён 
из локальной базы. 

---

### Задание 2. Memcached

Установите и запустите memcached.

*Приведите скриншот systemctl status memcached, где будет видно, что memcached запущен.*


### Решение 2

#### Команда установки Memcache

**sudo apt update && apt install memcached**


*Скриншот systemctl status memcache*

![Commit Task2](https://github.com/AndrewZnamenskiy/Memcached_Radis/blob/main/img/task2p1.png)


---

### Задание 3. Удаление по TTL в Memcached

Запишите в memcached несколько ключей с любыми именами и значениями, для которых выставлен TTL 5. 

*Приведите скриншот, на котором видно, что спустя 5 секунд ключи удалились из базы.*


### Решение 3


*Скриншот удаления данных по TTL*

![Commit Task3](https://github.com/AndrewZnamenskiy/Memcached_Radis/blob/main/img/task3p1.png)


---

### Задание 4. Запись данных в Redis

Запишите в Redis несколько ключей с любыми именами и значениями. 

*Через redis-cli достаньте все записанные ключи и значения из базы, приведите скриншот этой операции.*


### Решение 4


*Скриншот добавления и вывода ключей в Redis*

![Commit Task4](https://github.com/AndrewZnamenskiy/Memcached_Radis/blob/main/img/task4p1.png)


## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже разобраться в материале.

### Задание 5*. Работа с числами 

Запишите в Redis ключ key5 со значением типа "int" равным числу 5. Увеличьте его на 5, чтобы в итоге в значении лежало число 10.  

*Приведите скриншот, где будут проделаны все операции и будет видно, что значение key5 стало равно 10.*


### Решение 5


*Скриншот процедуры инкрементирования ключа на заданноую величину*

![Commit Task5](https://github.com/AndrewZnamenskiy/Memcached_Radis/blob/main/img/task5p1.png)






