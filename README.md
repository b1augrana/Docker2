
# Задание 2

Создайте контейнер для REST API сервера любого вашего проекта из курса по Django (например, [CRUD: Склады и запасы](https://github.com/netology-code/dj-homeworks/tree/drf/3.2-crud/stocks_products)).

> **ВАЖНО**: поменяйте БД с postgresql на sqlite3. Чтобы ваш контейнер мог работать без зависимости от postgres (с этим мы разберемся на следующем занятии).

Проверьте конфигурацию Django на использование переменных окружения (environment).

- Приложите в репозиторий Dockerfile и файлы приложения.
- В README.md описать типовые команды для запуска контейнера c backend-сервером.

> Для проверки работоспособности вашего контейнера отправляйте запросы с помощью `VS Code REST Client` или `Postman`.
>
> 
## Документация по проекту

Команда для создания Docker-образа:

```bash
docker build -t <name> .
```

Команда для запуска Docker-container'а:

```bash
docker run --name <project_name> -d -p 8000:8000 <name>
``` 

Проверка работы сервера:

```bash
curl localhost:8000
``` 

