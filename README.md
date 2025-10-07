# Blog API

REST API для блога.  
Реализовано на FastAPI с использованием Python 3.10.



##  Как запустить проект

1. Клонировать проект или скачать архив.
2. Установить зависимости:
   ```bash
   pip install -r requirements.txt
Запустить сервер:

bash
Copy code
uvicorn main:app --reload
Открыть документацию API:
http://127.0.0.1:8000/docs

Реализованные возможности
Пользователи (User)
GET /users — получить список пользователей

GET /users/{id} — получить пользователя по ID

POST /users — создать пользователя

PUT /users/{id} — обновить пользователя

DELETE /users/{id} — удалить пользователя

Посты (Post)
GET /posts — получить список постов

GET /posts/{id} — получить пост по ID

POST /posts — создать пост

PUT /posts/{id} — обновить пост

DELETE /posts/{id} — удалить пост

Пример запроса (создание пользователя)
POST /users

json
Copy code
{
  "id": 1,
  "email": "masha@example.com",
  "login": "masha",
  "password": "5123"
}


Автор
Кубарова Мария
2025