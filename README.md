## RSS reader

### Используемые технологии, библиотеки

Клиентская сторона | Серверная сторона
-------------------|-------------------
HTML               | PHP
CSS                | IDNA convert
JavaScript         | PDO
JQuery             | Cron
AJAX               | MySQL

Для ускорения разработки применялиcь

Инструмент         |
-------------------|
SCSS               |
Composer       |

### Особенности функционирования

* Копия структуры базы данных находится в файле `db_dump.sql`, находящемся в корневой дирректории
* Для подключения к БД в файле `config/web.php` необходимо присвоить правильные значения свойствам параметра 'db'
* Для парсинга фидов, cron должен выполнять скрипт по следующему пути: `yourdomain.ru/feed/parse`
* Для удаления прочитанных новостей, cron должен выполнять скрипт по следующему пути: `yourdomain.ru/news/delete`
