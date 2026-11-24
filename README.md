# Привет, я Максим 👋

## Python Backend Developer · AI / LLM Engineering

Разрабатываю backend-сервисы, REST API, AI-интеграции и решения для автоматизации бизнес-процессов.

Специализируюсь на Python Backend Engineering: проектировании API, асинхронной разработке, работе с базами данных, интеграции внешних сервисов и production-инфраструктуре.

В AI-направлении работаю над интеграцией LLM в backend-системы, архитектурой AI Gateway, автоматизацией обработки данных и применением AI coding agents в процессе разработки.

Имею опыт коммерческой разработки, командной работы, code review, самостоятельной реализации клиентских проектов и координации команды разработчиков.

**Основной стек:**

`Python` `FastAPI` `Django` `DRF` `PostgreSQL` `SQLAlchemy` `Redis` `Docker` `LLM API`

---

# 🛠 Technology Stack

### Backend Engineering

`Python` `FastAPI` `Django` `Django REST Framework` `Flask` `REST API` `Pydantic`

### Databases & Storage

`PostgreSQL` `SQLite` `Redis` `SQLAlchemy 2.0` `Django ORM` `Alembic` `MinIO`

### Async & Background Processing

`asyncio` `aiohttp` `Aiogram 3` `Celery`

### AI / LLM Engineering

`LLM API` `OpenAI API` `DeepSeek API` `AI Gateway` `Provider Routing` `Fallback` `Token Usage Tracking` `Prompt Engineering`

### AI-Assisted Development

`OpenAI Codex` `Cline` `AGENTS.md` `Context Engineering` `Harness Engineering`

### Testing & Code Quality

`pytest` `unittest` `Ruff` `Unit Testing` `Integration Testing` `Code Review`

### DevOps & Infrastructure

`Docker` `Docker Compose` `Linux` `Nginx` `Gunicorn` `GitHub Actions` `CI/CD` `VPS`

### Development Tools

`Git` `GitHub` `GitLab` `Poetry` `Postman` `VS Code` `PyCharm` `Docker Hub`

---

# 🤖 AI / LLM Engineering

Работаю над созданием backend-сервисов, предоставляющих единый интерфейс для взаимодействия с AI-моделями.

Основные направления:

- интеграция LLM через API;
- OpenAI-compatible API;
- асинхронное взаимодействие с AI-провайдерами;
- provider abstraction и routing;
- streaming responses;
- fallback между LLM-провайдерами;
- rate limiting и управление доступом;
- учёт token usage и стоимости запросов;
- обработка ошибок, timeout и отказов внешних сервисов;
- тестирование AI-интеграций.

Постепенно расширяю практический опыт в области Structured Outputs, Tool Calling, RAG, Embeddings, Vector Search и LangGraph.

---

# 🧠 AI-Assisted Development & Harness Engineering

Использую AI coding agents в коммерческих, командных и собственных проектах.

Развиваю воспроизводимый процесс агентной разработки, в котором AI-инструменты работают в рамках требований проекта, архитектурных ограничений и автоматизированных проверок.

### Engineering Workflow

```text
Requirements Analysis
        ↓
Task Decomposition
        ↓
Project Context / AGENTS.md
        ↓
AI-Assisted Implementation
        ↓
Automated Tests & Linting
        ↓
Git Diff & Code Review
        ↓
Integration & Delivery
```

### Инженерные практики

- Декомпозиция задач и формирование критериев готовности.
- Подготовка AGENTS.md и контекста кодовой базы.
- Определение архитектурных ограничений для AI-агентов.
- Управление областью изменений и зависимостями.
- Работа с агентами в существующих репозиториях.
- Проверка изменений через pytest, Ruff и Git diff.
- Ручной контроль архитектуры, бизнес-логики и качества кода.
- Итеративное улучшение инструкций и процесса разработки.

**Основные инструменты:** OpenAI Codex, Cline, Git, pytest, Ruff, AGENTS.md.

**Направления развития:** Harness Engineering, Context Engineering, Agentic Workflows, AI Evaluation.

---

# 🚀 Featured Projects

## 🤖 AI Subscription Platform / AI Gateway

`Personal Engineering Project` `In Development`

Многосервисная backend-платформа для предоставления доступа к LLM через единый API с управлением подписками, тарифами, API-ключами и потреблением ресурсов.

### Architecture

```text
                    Client
                       │
                       ▼
                   Core API
               Django / DRF
                       │
           ┌───────────┴───────────┐
           ▼                       ▼
      PostgreSQL               AI Gateway
                               FastAPI
                                   │
                          ┌────────┴────────┐
                          ▼                 ▼
                        Redis         Provider Layer
                                            │
                                    ┌───────┴───────┐
                                    ▼               ▼
                                  OpenAI         DeepSeek
```

### Core API

- Аутентификация и управление пользователями.
- Тарифные планы и подписки.
- Генерация и валидация API-ключей.
- Webhook-интеграции.
- Внутренний API для AI Gateway.

### AI Gateway

- OpenAI-compatible API.
- Асинхронная интеграция LLM-провайдеров.
- Provider abstraction.
- Streaming и fallback-сценарии.
- Rate limiting через Redis.
- Учёт потребления токенов и стоимости запросов.
- Обработка ошибок и timeout.
- Логирование использования AI-моделей.
- Автоматизированное тестирование.

**Stack:** `Python` `FastAPI` `Django` `DRF` `PostgreSQL` `SQLAlchemy` `Redis` `Alembic` `OpenAI API` `DeepSeek API` `pytest` `Docker`

---

## 📸 HubBox — Photo Hosting Backend

`Team Project` `Backend Engineering` `In Development`

Командная разработка backend-части фотохостинга с REST API, управлением фотографиями и альбомами, пользовательской лентой, поиском и социальными функциями.

### Мой вклад

- Разработка функциональности в рамках слоистой архитектуры Router → Service → Repository.
- Реализация REST API модуля Albums.
- Управление пользовательскими и системными альбомами.
- Разграничение доступа и проверки владельцев.
- Разработка бизнес-логики привязки фотографий к альбомам.
- Разработка backend-функциональности модуля Feed.
- Асинхронная работа с PostgreSQL и миграциями Alembic.
- Интеграция с существующей инфраструктурой хранения файлов и фоновых задач.
- Unit- и integration-тестирование.

### Engineering Practices

```text
Issue
  ↓
Feature Branch
  ↓
Implementation
  ↓
Tests & Linting
  ↓
Merge Request
  ↓
Code Review
```

Работаю с существующей кодовой базой, соблюдаю архитектурные соглашения и командный GitLab workflow.

На одном из этапов разработки успешно прошли **275 тестов проекта в Docker**. После доработок модуля Feed успешно прошли **40 профильных тестов**.

**Stack:** `Python 3.12` `FastAPI` `Pydantic v2` `PostgreSQL` `SQLAlchemy Async` `Alembic` `Redis` `Celery` `MinIO` `pytest` `Docker Compose` `Poetry` `Ruff` `GitLab`

**Repository:** [HubBox Backend — GitLab](https://gitlab.pointpulse.ru/l1/hubbox/backend)

---

## 🌌 Astro Prototype — Interactive Landing Page

`Commercial Project` `AI-Assisted Development` `Delivered`

Коммерческий промо-сайт для дейтинг-приложения, реализованный по индивидуальному техническому заданию заказчика.

Основная задача — создание интерактивного пользовательского интерфейса, презентация возможностей приложения и привлечение пользователей.

### Мой вклад

- Анализ бизнес-требований и декомпозиция технического задания.
- Самостоятельная реализация коммерческого проекта.
- Работа с интерактивными элементами, адаптивностью и пользовательскими сценариями.
- Применение OpenAI Codex в процессе разработки.
- Согласование изменений и передача готового продукта заказчику.

**Результат:** проект успешно завершён и принят заказчиком.

**Approach:** `AI-Assisted Development` `OpenAI Codex` `Requirements Analysis` `Web Development`

**Repository:** [astro-prototype](https://github.com/Maksim-1995/astro-prototype)

---

## 💈 Barbershop Booking Bot — «Народная цирюльня»

`Commercial Project` `Business Automation` `Delivered`

Коммерческий Telegram-бот для автоматизации записи клиентов и управления расписанием парикмахерской.

### Основной функционал

- Онлайн-запись с выбором услуги и мастера.
- Автоматический расчёт доступных временных слотов.
- Предотвращение конфликтов бронирования.
- Перенос и отмена записей.
- Автоматические уведомления.
- Административная система управления услугами, мастерами и расписанием.

### Engineering

- Асинхронная архитектура на Aiogram 3.
- Service Layer и SQLAlchemy ORM.
- Валидация данных и обработка сетевых ошибок.
- 38 unit-тестов.
- Контейнеризация и автоматизированный CI/CD.
- Production-развёртывание на Linux/VPS.

### CI/CD Pipeline

```text
Git Push → Unit Tests → Docker Build
                            ↓
                       Docker Hub
                            ↓
                        VPS Deploy
```

**Результат:** автоматизация процесса записи клиентов и сокращение объёма ручной работы администратора.

**Stack:** `Python` `Aiogram 3` `asyncio` `SQLAlchemy` `SQLite` `Pydantic Settings` `unittest` `Docker` `GitHub Actions` `Linux`

**Links:**

- [Telegram Bot](https://t.me/ai_bar_baros_bot)
- [GitHub Repository](https://github.com/Maksim-1995/tg_bot_for_barber)
- [Docker Hub](https://hub.docker.com/r/maksim1995/barber_bot)

---

## 📊 Alexlarin Parser — Educational Content Automation

`Data Engineering` `Parsing` `AI Automation`

Python-проект для автоматизации сбора, извлечения и структурирования образовательного контента.

### Data Processing Pipeline

```text
HTML / PDF / JavaScript
           ↓
    Data Extraction
           ↓
     Normalization
           ↓
  Tasks / Answers / Images
           ↓
    Structured Export
```

### Основной функционал

- Автоматическая загрузка исходных материалов.
- Парсинг HTML, PDF и JavaScript.
- Извлечение текстовых заданий, изображений и ответов.
- Обработка обфусцированного JavaScript.
- Структурирование образовательного контента.
- Формирование Excel-файлов и архивов с результатами.
- Эксперименты с LLM для автоматизации обработки сложных заданий.
- Внедрение практик Harness Engineering в процесс разработки.

**Stack:** `Python` `Requests` `PyMuPDF` `openpyxl` `jsbeautifier` `LLM API` `OpenAI Codex` `AGENTS.md`

---

## 🍽 Foodgram — Recipe Sharing Platform

`Backend Engineering` `REST API` `DevOps`

Backend-приложение для публикации и обмена рецептами с REST API и SPA-фронтендом.

### Engineering Highlights

- REST API на Django REST Framework.
- Аутентификация и разграничение доступа.
- Проектирование связанных моделей PostgreSQL.
- Фильтрация, пагинация и поиск.
- Работа с пользовательскими медиафайлами.
- Подписки, избранное и автоматическое формирование списка покупок.
- Более 1100 тестовых сценариев.
- Контейнеризация и автоматизированный CI/CD.
- Production-развёртывание на VPS.

### Infrastructure

```text
Client
   ↓
 Nginx
   ↓
Gunicorn
   ↓
Django / DRF
   ↓
PostgreSQL

Docker Compose · Persistent Volumes · CI/CD
```

**Stack:** `Python` `Django` `DRF` `PostgreSQL` `Docker Compose` `Nginx` `Gunicorn` `GitHub Actions`

**Links:**

- [GitHub Repository](https://github.com/Maksim-1995/foodgram)
- [Production Website](https://maksim-foodgram.duckdns.org)

---

## 🔐 Auth Service — JWT & RBAC

`Backend Engineering` `Security`

Backend-сервис с собственной реализацией JWT-аутентификации и ролевой моделью управления доступом.

### Engineering Highlights

- Access и Refresh JWT-токены.
- Middleware аутентификации.
- Token Blacklist.
- Role-Based Access Control.
- Управление ролями, ресурсами и правами доступа.
- Проверка разрешений на уровне бизнес-операций.
- REST API для защищённых ресурсов.

**Stack:** `Python` `Django` `DRF` `PostgreSQL` `PyJWT` `RBAC`

---

## ⭐ YaMDb — Reviews & Rating REST API

`Team Project` `Backend Development` `Team Leadership`

Командный REST API-проект, реализованный командой из трёх Python-разработчиков.

**Role:** Python Backend Developer / Team Lead.

### Backend Development

- Проектирование моделей произведений, категорий и жанров.
- Реализация REST API.
- Фильтрация и импорт данных из CSV.
- Интеграция модулей приложения.

### Team Leadership

- Декомпозиция и распределение задач.
- Координация командной разработки.
- Code review pull requests.
- Контроль интеграции компонентов.
- Подготовка общей версии проекта.

**Stack:** `Python` `Django` `DRF` `JWT` `django-filter` `pytest` `Git`

**Repository:** [api_yamdb](https://github.com/Maksim-1995/api_yamdb)

---

# 📦 Other Projects

| Project | Description | Technologies |
|---|---|---|
| [YaCut](https://github.com/Maksim-1995/async-yacut) | Сервис сокращения ссылок с REST API | Flask, SQLAlchemy, SQLite |
| [Blogicum](https://github.com/Maksim-1995/django-sprint4) | Блог-платформа с пользовательскими публикациями | Django, PostgreSQL, pytest |

---

# 🎯 Engineering Focus

Мой профессиональный фокус находится на пересечении нескольких инженерных направлений.

```text
         Python Backend Engineering
                     │
         ┌───────────┴───────────┐
         ▼                       ▼
   Data & APIs            AI / LLM Engineering
         │                       │
         ▼                       ▼
    Automation            Agentic Development
         │                       │
         └───────────┬───────────┘
                     ▼
          Production Infrastructure
```

### Backend Engineering

- Архитектура backend-сервисов.
- Асинхронное программирование.
- Проектирование API и моделей данных.
- Распределённые системы и взаимодействие сервисов.
- Производительность, надёжность и безопасность.

### AI / LLM Engineering

- AI Gateway и LLM-интеграции.
- Provider Routing и Fallback.
- AI-инфраструктура и управление потреблением ресурсов.
- Автоматизация обработки данных.
- Agentic Workflows и Harness Engineering.

### Current Learning

`LangGraph` `RAG` `Embeddings` `Vector Search` `pgvector` `Qdrant` `AI Evaluation` `Observability` `ML Fundamentals`

---

# 🤝 Open to Opportunities

Рассматриваю возможности профессионального развития в направлениях:

- Python Backend Developer.
- Backend Software Engineer.
- AI / LLM Engineer.
- AI Integration Engineer.
- AI Automation Engineer.

Интересуют проекты, связанные с разработкой backend-сервисов, интеграцией AI-моделей, автоматизацией бизнес-процессов и созданием надёжных программных систем.

---

# 📫 Contacts

| Platform | Profile |
|---|---|
| GitHub | [Maksim-1995](https://github.com/Maksim-1995/) |
| GitLab | [Maksim-1995](https://gitlab.pointpulse.ru/Maksim-1995) |
| Telegram | [@MaksimKME](https://t.me/MaksimKME) |
