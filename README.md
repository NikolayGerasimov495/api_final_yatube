# api_yatube

## Описание

CRUD для проекта социальной сети Yatube.

## СТЭК

-Python
-Django 
-DRF 
-Djoser 

## Установка и запуск

1. Клонируйте репозиторий:
   ```
   git clone git@github.com:NikolayGerasimov495/homework_bot.git
   ```

2. Установить виртуальное окружение для проекта:
    ```
    python -m venv venv
    ```

3. Установите зависимости:
   ```
   pip install -r requirements.txt
   ```

## Примеры запросов

### Создание публикации
**POST** .../api/v1/posts/
```json
{
  "text": "string",
  "image": "string",
  "group": 0
}
```
### Получение публикации
**GET** .../api/v1/posts/{id}/
```json
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
### Обновление публикации
**PUT** .../api/v1/posts/{id}/
```json
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
### Получение комментариев
**GET** .../api/v1/posts/{id}/comments/
```json
{
  "id": 0,
  "author": "string",
  "text": "string",
  "pub_date": "2019-08-24T14:15:22Z",
  "image": "string",
  "group": 0
}
```
### Подписки
**GET** .../api/v1/follow/
```json
[
  {
    "user": "string",
    "following": "string"
  }
]
```
### Подписка
**POST** .../api/v1/follow/
```json
{
  "following": "string"
}
```
