# MeowHub

MeowHub — это веб-приложение для любителей кошек, где пользователи могут делиться фотографиями своих питомцев, просматривать анкеты других котиков и оставлять комментарии. Проект реализован с использованием Python (Django), JavaScript, CSS, HTML и Docker.

## Возможности

- Регистрация и авторизация пользователей
- Добавление профиля котика с фотографией и описанием
- Просмотр списка всех котиков
- Комментирование анкет котиков
- Адаптивный дизайн интерфейса
- Docker-контейнеризация приложения

## Стек технологий

- Python (Django)
- JavaScript
- HTML5, CSS3
- Docker
- Gunicorn, Nginx

## Быстрый старт

### Клонирование репозитория

```bash
git clone https://github.com/Vladimir-Samoilov/kittygram_final.git
cd kittygram_final
```

*(Если переименуете репозиторий — обновите ссылку!)*

### Запуск с помощью Docker

1. Постройте и запустите контейнеры:

```bash
docker-compose up --build
```

2. Приложение будет доступно по адресу: http://localhost/

### Без Docker (локально)

1. Установите зависимости:

```bash
pip install -r requirements.txt
```

2. Примените миграции и создайте суперпользователя:

```bash
python manage.py migrate
python manage.py createsuperuser
```

3. Запустите сервер:

```bash
python manage.py runserver
```

## Переменные окружения

Для работы с базой данных и другими сервисами используйте переменные окружения. Пример `.env` файла:

```
SECRET_KEY=your_secret_key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
DB_NAME=meowhub
DB_USER=meowhub_user
DB_PASSWORD=meowhub_password
DB_HOST=db
DB_PORT=5432
```

## Контакты

Автор: Владимир Самойлов  
GitHub: [Vladimir-Samoilov](https://github.com/Vladimir-Samoilov)

---

Проект выполнен в рамках учебной программы Яндекс Практикум.
