# Данный проект позволяет получать данные о работодателях и их вакансиях с сайта HH.ru

Для это необходимо использовать публичный API hh.ru и библиотеку запросов.

Данные о вакансиях и работодателях добавляются в таблицы базы данных PostgreSQL. Для работы с базой данных используется библеотека - psycopg2.
Для работы с базой данной используется класс DBManager. 

# Благодаря классу DBManager в консоль выводится:
- список всех компаний и количество вакансий у каждой компании
- список всех вакансий с указанием названия компании, названия вакансии, зарплата и ссылка на вакансию 
- среднюю зарплату по вакансиям
- список всех вакансий, у которых зарплата выше средней по всем вакансиям
- список всех вакансий, в названии которых содержаться переданные в метод слова "Phyton"

Файл database_.ini говорит о том, что необходимо ввести свой пароль для подключения БД, через конфигурационный файл (если конфигур. файл не срабатывает, переименовать файл в database.ini).

Фаил .env_simple необходим для ввода своего пароля и дальнейшей работы создания и добавления данных в таблицы.