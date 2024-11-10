# Домашнее задание 1

## Описание сервисов

- **nginx**: Веб-сервер, доступный на порту 80.
- **postgresql**: База данных PostgreSQL, доступная на порту 5432.

## Использование

1. Склонируйте репозиторий:


2. Создайте файл `.env` в корневой директории и добавьте в него следующие переменные окружения:
    ```env
    POSTGRES_USER=your_postgres_user
    POSTGRES_PASSWORD=your_postgres_password
    CUSTOM_DB_USER=your_custom_db_user
    CUSTOM_DB_PASSWORD=your_custom_db_password
    CUSTOM_DB_NAME=your_custom_db_name
    ```

3. Запустите Docker Compose:
    ```sh
    docker-compose up --build
    ```

## Структура проекта

- `nginx/`: Директория с файлами для сборки образа nginx.
- `postgresql/`: Директория с файлами для сборки образа PostgreSQL.
- `docker-compose.yaml`: Конфигурационный файл для Docker Compose.

## Переменные окружения

Переменные окружения для сервиса PostgreSQL задаются в файле `.env`:

- `POSTGRES_USER`: Имя пользователя PostgreSQL.
- `POSTGRES_PASSWORD`: Пароль пользователя PostgreSQL.
- `CUSTOM_DB_USER`: Имя пользователя для кастомной базы данных.
- `CUSTOM_DB_PASSWORD`: Пароль пользователя для кастомной базы данных.
- `CUSTOM_DB_NAME`: Имя кастомной базы данных.
