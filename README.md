# 🧑‍💻 CodeSync — Real-time Collaborative Code Editor (Backend Only)

**CodeSync** — это бэкенд-платформа для совместного редактирования кода в реальном времени. Реализована на Django + WebSocket + Redis. Проект включает систему авторизации, управление комнатами, хранение документов и поддержку WebSocket-соединений для синхронного редактирования.

---

## 🔧 Текущий статус

> ⚠️ **Фронтенд находится в разработке.**
>
> Мы **открыты к сотрудничеству** с разработчиками, которые хотят помочь реализовать фронтенд на React, Vue или любом другом современном фреймворке.
>
> 📬 Если вы заинтересованы — создайте issue или свяжитесь с нами через GitHub!

---

## 📌 Возможности

- 🔐 JWT-аутентификация (регистрация, логин, refresh)
- 🏠 Комнаты редактирования (публичные и приватные)
- 📝 Хранение документов с автосохранением
- 🌐 WebSocket-редактирование кода в реальном времени
- 👥 Показ активных участников комнаты

---

## 🧱 Стек

- Django 4.x
- Django REST Framework (DRF)
- Django Channels
- Redis (для WebSocket-каналов)
- SimpleJWT

---

## 🏗️ Структура backend-проекта

```
CodeSync/
├── manage.py
├── codesync/           # Конфигурация Django
│   ├── settings.py
│   ├── urls.py
│   └── asgi.py         # WebSocket маршрутизация
├── auth/               # JWT авторизация
├── users/              # Профиль пользователя
├── rooms/              # Комнаты
├── documents/          # Документы
├── ws/                 # WebSocket consumers
└── requirements.txt
```

---

## ⚙️ Установка и запуск

```bash
# Установка зависимостей
pip install -r requirements.txt

# Запуск Redis (необходим для WebSocket)
redis-server

# Применение миграций
python manage.py migrate

# Запуск сервера
python manage.py runserver
```

---

## 📆 Roadmap

* [ ] JWT аутентификация
* [ ] CRUD комнат
* [ ] Документы с автосохранением
* [ ] WebSocket-редактор (backend)
* [ ] История изменений
* [ ] Версионность документа
* [ ] Видео/аудио-чат (в будущем)
* [ ] AI-комментарии к коду

---

## 🧑‍🤝‍🧑 Сотрудничество

Мы ищем:

* 🎨 Фронтенд-разработчиков (React, Vue, TypeScript)
* 📦 Специалистов по CI/CD и Docker
* 🤖 Энтузиастов AI/ML для интеграции GPT

Если вам интересно поучаствовать — добро пожаловать в [issues](https://github.com/Atambek07/CodeSync/issues) или создайте pull request.

---

## 👤 Автор

* Атамбек Абдисаламов — [GitHub](https://github.com/Atambek07)
* Элдар Абдрашитов — [GitHub](https://github.com/E1dar01)

---
