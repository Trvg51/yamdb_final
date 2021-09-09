# api_yamdb
![example workflow](https://github.com/Trvg51/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)
### Описание

Данный проект позволяет реализовать API - сервис с базой данных различных произведений (фильмы\музыка\книги и тд.)
Реализована возможность оставлять ревью и комментарии.
Дополнительно имеется возможность запустить проект в контейнере (Docker)

### Технологии

Python 3.8.5
Django 3.0.5
Docker 20.10.8

### Запуск проекта в dev-режиме

- Открыть файл и прочитать ".env.template"

- В командной строке в папке с файлом manage.py выполнить команды:
- docker-compose up
- docker-compose exec web python manage.py migrate
- docker-compose exec web python manage.py createsuperuser (создаем админа, заполняем все запрошеные поля)
- docker-compose exec web python manage.py collectstatic --no-input

### Автор

Якушенков Евгений
http://trvgserver.co.vu/