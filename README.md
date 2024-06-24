# Проект "тестовое для madsoft"

Проект представляет собой пример приложения, использующего FastAPI вместе с базой данных PostgreSQL и хранилищем MinIO.

## Содержание

1. [Введение](#введение)
2. [Компоненты проекта](#компоненты-проекта)
3. [Запуск проекта](#запуск-проекта)

## Введение

Проект разработан для демонстрации использования FastAPI в комбинации с PostgreSQL и MinIO. FastAPI — современный фреймворк для создания веб-приложений на Python с поддержкой асинхронных операций. PostgreSQL используется в качестве базы данных для хранения данных приложения, а MinIO — как локальное хранилище для файлов.

## Компоненты проекта

- **PostgreSQL**: Реляционная база данных для хранения данных приложения.
- **FastAPI**: Фреймворк для создания веб-приложений на Python.
- **MinIO**: Локальное хранилище объектов для сохранения и работы с файлами.

## Запуск проекта

Для запуска проекта необходимо выполнить следующие шаги:

1. **Настройка окружения**:
   - Я уже создал  `.env` и специально не добавил его в gitignore.

2. **Запуск через Docker**:
   - Убедитесь, что у вас установлен Docker и Docker Compose.
   - Выполните сборку и запуск контейнеров Docker:

     ```bash
     docker-compose -f minio-docker-compose.yml up -d
     ```

3. **Доступ к приложению**:
   - После успешного запуска контейнеров приложение FastAPI будет доступно по адресу `http://localhost:8000`.
   - Панель управления MinIO доступна по адресу `http://localhost:9000`, используйте учетные данные `minioadmin:minioadmin` для входа.

4. **Запуск миграций базы данных**:
   - Я уже создал миграцию, а контейнер автоматически ее применяет


Эти инструкции помогут вам настроить и запустить проект локально.

