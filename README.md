# Привет, я Максим 👋

### Python Backend Developer

Разрабатываю backend-приложения на **Python**. Основной стек — **Django, Django REST Framework, PostgreSQL и Docker**.

Работаю с проектированием REST API, реляционными базами данных, аутентификацией и авторизацией, тестированием и контейнеризацией приложений.

Изучаю интеграцию **LLM и AI API** в backend-сервисы: structured outputs, tool calling, RAG и построение AI Gateway.

Есть опыт развёртывания проектов на Linux-серверах с использованием **Docker Compose, Nginx, Gunicorn и CI/CD**.

---

## 🛠 Технологии

### Backend

`Python` `Django` `Django REST Framework` `Flask` `REST API` `Gunicorn`

### AI / LLM

`LLM API` `Prompt Engineering` `AI API Integration`

Изучаю и применяю подходы к интеграции LLM в backend-приложения:

* интеграция LLM через REST API;
* Prompt Engineering;
* Structured Outputs;
* Tool / Function Calling;
* асинхронное взаимодействие с AI API;
* обработка ошибок, timeout и retry;
* проектирование AI Gateway;
* rate limiting;
* контроль token usage и стоимости запросов;
* кэширование AI-запросов;
* fallback между LLM-провайдерами.

**В процессе изучения:**
`RAG` `Embeddings` `Vector Search` `pgvector / Qdrant` `LangChain` `LangGraph`

### Базы данных

`PostgreSQL` `SQLite`

### Асинхронная разработка

`asyncio` `Aiogram` `Telebot`

### Тестирование

`Pytest` `unittest`

### DevOps и инфраструктура

`Docker` `Docker Compose` `Nginx` `Linux` `GitHub Actions` `CI/CD`

### Инструменты

`Git` `GitHub` `Docker Hub` `Postman` `PyCharm` `Requests`

### Дополнительно

`ООП` `Алгоритмы и структуры данных` `Рефакторинг`

### Frontend — базовый уровень

`HTML` `CSS` `Bootstrap`

---

# 🚀 Проекты

## 🍽 Foodgram — сервис публикации рецептов

Backend веб-приложения для публикации и обмена кулинарными рецептами с **REST API** и SPA-фронтендом.

### Возможности

* регистрация и аутентификация пользователей;
* создание, редактирование и удаление рецептов;
* загрузка изображений рецептов и аватаров;
* подписки на авторов;
* добавление рецептов в избранное;
* добавление рецептов в список покупок;
* автоматическое формирование и скачивание списка ингредиентов;
* фильтрация рецептов по тегам;
* поиск ингредиентов;
* пагинация API;
* административная панель Django.

### Backend

REST API реализован на **Django REST Framework**.

В проекте реализованы:

* кастомная модель пользователя;
* аутентификация через Djoser;
* serializers и ViewSets DRF;
* permissions;
* filtering и pagination;
* загрузка и хранение изображений;
* связи между пользователями, рецептами, ингредиентами и тегами;
* PostgreSQL для хранения данных.

### Инфраструктура

Проект полностью контейнеризирован.

Production-окружение:

`Nginx → Docker Gateway → Gunicorn → Django → PostgreSQL`

Используются отдельные Docker-контейнеры для:

* backend;
* frontend;
* PostgreSQL;
* Nginx gateway.

Настроены:

* Docker Compose;
* Gunicorn;
* Nginx;
* persistent volumes для PostgreSQL, static и media;
* Django migrations;
* сбор статических файлов;
* CI/CD через GitHub Actions;
* автоматическая сборка Docker-образов;
* публикация образов в Docker Hub;
* автоматический деплой приложения на сервер.

**Стек:**
`Python` `Django` `DRF` `PostgreSQL` `Docker` `Docker Compose` `Nginx` `Gunicorn` `GitHub Actions` `CI/CD`

**GitHub:**
https://github.com/Maksim-1995/foodgram

**Demo:**
http://176.12.75.107/

---

## 🔗 YaCut — сервис сокращения ссылок

Веб-приложение на **Flask** для создания коротких ссылок.

Пользователь может передать исходный URL и получить сокращённую ссылку с автоматически сгенерированным или собственным коротким идентификатором.

### Возможности

* создание коротких ссылок;
* автоматическая генерация уникального идентификатора;
* пользовательские короткие идентификаторы;
* перенаправление на оригинальный URL;
* проверка уникальности идентификаторов;
* валидация пользовательских данных;
* REST API для создания коротких ссылок;
* обработка ошибок API.

### Backend

В проекте используются:

* Flask;
* Flask-SQLAlchemy;
* SQLAlchemy ORM;
* Flask-WTF и WTForms;
* REST API;
* JSON-запросы и ответы;
* обработка исключений и ошибок API;
* разделение приложения на модели, формы, views и API.

**Стек:**
`Python` `Flask` `Flask-SQLAlchemy` `SQLAlchemy` `WTForms` `REST API` `SQLite`

**GitHub:**
https://github.com/Maksim-1995/async-yacut

---

## 📝 Blogicum — блог-платформа на Django

Веб-приложение для публикации постов и взаимодействия пользователей.

### Возможности

* регистрация и аутентификация;
* создание и редактирование публикаций;
* категории публикаций;
* комментарии;
* профили пользователей;
* загрузка изображений;
* пагинация;
* административная панель Django;
* тестирование приложения.

**Стек:**
`Python` `Django` `PostgreSQL` `SQLite` `Bootstrap` `Pytest`

**GitHub:**
https://github.com/Maksim-1995/project_blogicum

**Demo:**
https://maksim1995k.pythonanywhere.com/

---

## 📚 Сейчас изучаю

### Backend

* углублённо PostgreSQL;
* FastAPI;
* архитектуру backend-приложений;
* проектирование REST API;
* асинхронный Python.

### AI Engineering

* интеграцию LLM API;
* Structured Outputs;
* Tool / Function Calling;
* RAG;
* Embeddings;
* Vector Search;
* pgvector / Qdrant;
* LangChain;
* LangGraph.

### DevOps

* Docker;
* CI/CD;
* Linux;
* production-развёртывание backend-приложений.

---

## 📫 Контакты

**GitHub:**
https://github.com/Maksim-1995/

**Telegram:**
@MaksimKME
