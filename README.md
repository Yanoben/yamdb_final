# yamdb_final
[![CI](https://github.com/Yanoben/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?branch=master)](https://github.com/Yanoben/yamdb_final/actions/workflows/yamdb_workflow.yml)

# API for social media 'Yatube'

### Автор
- @Yanoben

### Ссылке на проект
- http://51.250.29.6/

###  Redoc
- http://51.250.29.6/redoc

### Технологии в проекте
- Python 3.7
- Django 2.2.19
- Django REST framework 3.12.4

### Запуск проекта в dev-режиме
- Сначала клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yanoben/api_yamdb.git
```

- Установите и активируйте виртуальное окружение
```
python -m venv venv

. venv/bin/activate
```

- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 

- В папке с файлом manage.py выполните команду:
```
python3 manage.py runserver
```

## Примеры запроса

### GET

`GET /reviews/`

    curl -i -H 'Accept: application/json' http://51.250.29.6/reviews/

### Response

    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:30 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 2

    [

    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    },
    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    },
    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    }

    ]

### GET ID

`GET /reviews/<int:review_id>/`

    curl -i -H 'Accept: application/json' http://51.250.29.6/reviews/<int:reviews_id>/

### Response

    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:30 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 2

    [
        {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
        }
    ]

### GET

`GET /reviews/<int:review_id>/comments`

    curl -i -H 'Accept: application/json' http://51.250.29.6/reviews/<int:review_id>/comments

### Response

    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:30 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 2

    [

    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    },
    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    },
    {
        "id": 0,
        "author": "string",
        "text": "string",
        "pub_date": "2021-08-24T14:15:22Z",
        "image": "string",
        "group": 0
    }

    ]