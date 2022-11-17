
# api_final_yatube
## Описание
api_final_yatube - это мой учебный проект по курсу Python-разработчик в Яндекс Практикуме.

Данный проект представляет из себя API для блог-платформы Yatube , построенное на основе Django REST Framework.


Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

```
$ git clone https://github.com/pa1nf0rce/api_final_yatube.git
$ cd api_final_yatube
```
Cоздать и активировать виртуальное окружение:
```
python3 -3.7 -m venv venv
source venv/Scripts/activate
```
Установить зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```
Выполнить миграции:
```
$ cd yatube_api
python3 manage.py migrate
```
Запустить проект:
```
python3 manage.py runserver
```
Проект буден доступен по адресу http://127.0.0.1:8000/

Некоторые примеры запросов к API
api/v1/posts/:

GET - получить список постов
POST - добавить свой пост
api/v1/posts/{post_id}/comments/:

GET - получить список комментариев определенного поста
POST - добавить комментарий к посту
Это далеко не весь список эндпоинтов и возможных запросов. В проекте есть документация к API в виде ReDoc - она доступна по адресу http://127.0.0.1:8000/redoc/.
