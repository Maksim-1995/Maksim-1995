# Привет, я Максим 👋

## Python Backend Developer · ML / LLM Engineering

Разрабатываю backend-сервисы на **Python** и развиваюсь в направлении **ML/AI Engineering**.

Основной стек:

`Python` `Django` `Django REST Framework` `FastAPI` `PostgreSQL` `Docker`

Работаю с:

- проектированием и разработкой REST API;
- реляционными базами данных и ORM;
- аутентификацией и разграничением доступа;
- асинхронным Python;
- интеграцией внешних API;
- тестированием backend-кода;
- Docker и CI/CD;
- production-развёртыванием на Linux;
- интеграцией LLM в backend-сервисы.

В AI-направлении особенно интересуюсь тем, как **ML/LLM-модели превращаются в production-сервисы**: AI Gateway, structured outputs, tool calling, RAG, embeddings, vector search, rate limiting, caching, fallback и контроль использования моделей.

Есть опыт коммерческой разработки, командной работы, code review и роли тимлида.

---

# 🛠 Технологии

### Backend

`Python` `Django` `Django REST Framework` `FastAPI` `Flask` `REST API`

### Databases

`PostgreSQL` `SQLite` `Django ORM` `SQLAlchemy`

### Async

`asyncio` `aiohttp` `Aiogram 3`

### ML / AI / LLM

`LLM API` `AI API Integration` `Prompt Engineering` `Structured Outputs` `Tool Calling` `AI Gateway`

Изучаю и применяю:

`RAG` `Embeddings` `Vector Search` `pgvector` `Qdrant` `LangGraph`

### Testing

`Pytest` `unittest`

### DevOps

`Docker` `Docker Compose` `Linux` `Nginx` `Gunicorn` `GitHub Actions` `CI/CD`

### Tools

`Git` `GitHub` `Docker Hub` `Postman` `PyCharm`

---

# 🤖 AI / ML Engineering

Сейчас развиваюсь на стыке **Python Backend и ML Engineering**.

Работаю над архитектурой сервисов, которые предоставляют единый backend-интерфейс для взаимодействия с AI-моделями.

Практикую:

- интеграцию LLM через API;
- Structured Outputs;
- Tool / Function Calling;
- асинхронную работу с AI API;
- timeout / retry;
- provider routing;
- fallback между LLM-провайдерами;
- rate limiting;
- caching;
- контроль token usage;
- обработку ошибок AI-провайдеров;
- проектирование AI Gateway.

Следующее направление развития:

**RAG → Embeddings → Vector Search → pgvector / Qdrant → LangGraph**

---

# 🚀 Основные проекты

## 🤖 AI Subscription Service / AI Gateway

Backend-проект для предоставления доступа к AI-моделям через единый API.

Архитектура разделена на основной backend и отдельный AI Gateway:

`Client → Core API → AI Gateway → LLM Provider`

### Backend

**Core API:**

`Django` `Django REST Framework` `PostgreSQL`

**AI Gateway:**

`FastAPI` `asyncio` `LLM API`

В проекте развиваю:

- API для взаимодействия с AI-сервисами;
- маршрутизацию запросов между LLM-провайдерами;
- fallback при ошибках основного провайдера;
- API-key authentication;
- rate limiting;
- учёт использования AI API;
- контроль token usage;
- обработку timeout и ошибок внешних API;
- тестирование provider layer;
- разделение основной бизнес-логики и AI-инфраструктуры.

Проект использую для изучения архитектуры backend-сервисов и production-интеграции LLM.

---

## 🍽 Foodgram — REST API сервиса рецептов

Полноценное backend-приложение для публикации и обмена рецептами с REST API и SPA-фронтендом.

### Backend

REST API реализован на **Django REST Framework**.

Реализованы:

- кастомная модель пользователя;
- регистрация и аутентификация;
- permissions;
- CRUD рецептов;
- подписки на авторов;
- избранное;
- список покупок;
- фильтрация и пагинация;
- поиск ингредиентов;
- загрузка изображений;
- связанные модели через ForeignKey и ManyToMany;
- административная панель Django.

В базу загружается около **2200 ингредиентов**.

Проект проходит **1134+ тестовых сценариев** моделей и API.

### Production

Проект полностью контейнеризирован.

```text
Nginx
  ↓
Docker
  ↓
Gunicorn
  ↓
Django / DRF
  ↓
PostgreSQL
```

Настроены:

- Docker Compose;
- PostgreSQL 16;
- Nginx;
- Gunicorn;
- persistent volumes;
- migrations;
- static/media;
- GitHub Actions;
- автоматическая сборка Docker-образов;
- публикация образов;
- автоматический deployment на VPS.

**Стек:**

`Python` `Django` `DRF` `PostgreSQL` `Docker` `Docker Compose` `Nginx` `Gunicorn` `GitHub Actions`

**GitHub:**
[https://github.com/Maksim-1995/foodgram](https://github.com/Maksim-1995/foodgram)

**Production:**
[http://maksim-foodgram.duckdns.org](http://maksim-foodgram.duckdns.org)

---

## 💈 Telegram-бот «Народная цирюльня»

Коммерческий проект для автоматизации записи клиентов в парикмахерскую.

**Работающий бот:**
[https://t.me/ai_bar_baros_bot](https://t.me/ai_bar_baros_bot)

### Для клиентов

- выбор услуги;
- выбор мастера;
- просмотр доступных дат и времени;
- автоматическое формирование свободных слотов;
- онлайн-запись;
- перенос и отмена записи;
- уведомления;
- подтверждение записи.

### Для администратора

Реализована отдельная административная система:

- управление услугами;
- управление мастерами;
- настройка расписания;
- управление выходными и праздничными датами;
- просмотр записей;
- ручное создание записи;
- перенос и техническая отмена;
- настройка интервала слотов;
- заполнение demo-данными.

### Backend

Бот построен на **Aiogram 3** и асинхронном Python.

Архитектура разделена на:

```text
handlers
services
models
keyboards
filters
utils
```

Используются:

- routers;
- FSM;
- service layer;
- SQLAlchemy ORM;
- асинхронная работа с БД;
- валидация пользовательских данных;
- логирование;
- обработка сетевых ошибок;
- защита от повторных действий пользователя.

Проект покрыт **38 unit-тестами**.

### CI/CD

```text
Push в main
     ↓
Unit tests
     ↓
Docker build
     ↓
Docker Hub
     ↓
Deploy на VPS
```

Production-настройка включает:

- Docker / Docker Compose;
- persistent volume для SQLite;
- GitHub Actions;
- deployment по SSH;
- автоматический restart;
- хранение секретов через GitHub Secrets и `.env`.

**Стек:**

`Python` `Aiogram 3` `asyncio` `SQLAlchemy` `SQLite` `Pydantic Settings` `unittest` `Docker` `GitHub Actions` `Linux`

**GitHub:**
[https://github.com/Maksim-1995/tg_bot_for_barber](https://github.com/Maksim-1995/tg_bot_for_barber)

**Docker Hub:**
[https://hub.docker.com/r/maksim1995/barber_bot](https://hub.docker.com/r/maksim1995/barber_bot)

---

## ⭐ YaMDb — REST API сервиса отзывов

Командный backend-проект, разработанный командой из **3 Python-разработчиков**.

В проекте выполнял роли:

**Python Developer + Team Lead**

### В роли тимлида

- организовал работу команды;
- участвовал в распределении и приоритизации задач;
- отслеживал прогресс разработки;
- координировал интеграцию частей проекта;
- проводил **code review pull request'ов**;
- участвовал в устранении замечаний;
- отвечал за подготовку общей версии проекта к проверке.

### В роли разработчика

Отвечал за:

- модели произведений;
- категории;
- жанры;
- REST API для этих ресурсов;
- serializers;
- views;
- filtering;
- импорт данных из CSV.

В проекте также реализованы:

- JWT-аутентификация;
- роли `user / moderator / admin`;
- permissions;
- отзывы;
- комментарии;
- рейтинг произведений.

**Стек:**

`Python` `Django` `Django REST Framework` `PyJWT` `django-filter` `Pytest` `Git`

**GitHub:**
[https://github.com/Maksim-1995/api_yamdb](https://github.com/Maksim-1995/api_yamdb)

---

# 📦 Другие проекты

## 🔗 YaCut

Сервис сокращения ссылок на Flask.

Реализованы REST API, генерация коротких идентификаторов, валидация, SQLAlchemy ORM и обработка ошибок.

**Стек:**
`Python` `Flask` `SQLAlchemy` `WTForms` `REST API` `SQLite`

**GitHub:**
[https://github.com/Maksim-1995/async-yacut](https://github.com/Maksim-1995/async-yacut)

---

## 📝 Blogicum

Блог-платформа на Django.

Реализованы:

- регистрация и аутентификация;
- публикации;
- категории;
- комментарии;
- профили;
- изображения;
- пагинация;
- административная панель;
- тестирование.

**Стек:**
`Python` `Django` `PostgreSQL` `Pytest` `Bootstrap`

**GitHub:**
[https://github.com/Maksim-1995/django-sprint4](https://github.com/Maksim-1995/django-sprint4)

---

# 📚 Сейчас изучаю

### Backend Engineering

- углублённый PostgreSQL;
- FastAPI;
- архитектуру backend-сервисов;
- асинхронный Python;
- производительность API;
- Redis;
- взаимодействие между сервисами.

### ML / AI Engineering

- Machine Learning fundamentals;
- RAG;
- Embeddings;
- Vector Search;
- pgvector;
- Qdrant;
- LangGraph;
- production-интеграцию ML/LLM-моделей.

### DevOps

- Docker;
- CI/CD;
- Linux;
- production deployment;
- мониторинг backend-сервисов.

---

# 🎯 Профессиональный фокус

Моя основная специализация — **Python Backend Development**.

Одновременно развиваюсь в направлении **ML / AI Engineering**, прежде всего в задачах интеграции моделей в реальные backend-системы.

Мне особенно интересны проекты на пересечении:

```text
Python Backend
     +
Data
     +
ML / LLM
     +
Production Infrastructure
```

Цель — развиваться как инженер, способный не только работать с AI-моделью, но и построить вокруг неё надёжный backend-сервис: API, хранение данных, ограничения, тестирование, мониторинг и production-инфраструктуру.

---

# 📫 Контакты

**GitHub:**
[https://github.com/Maksim-1995/](https://github.com/Maksim-1995/)

**Telegram:**
[https://t.me/MaksimKME](https://t.me/MaksimKME)
