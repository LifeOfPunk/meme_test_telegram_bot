# Структура проекта MeeMee Bot

## 📁 Основные директории

```
oldbotmememe/
├── src/                    # Исходный код бота
│   ├── bot_start.js       # Основной бот
│   ├── bot_start_admin.js # Админ-бот
│   ├── config.js          # Конфигурация
│   ├── redis.js           # Подключение к Redis
│   ├── controllers/       # Контроллеры
│   ├── screens/           # Экраны и клавиатуры
│   ├── services/          # Сервисы (User, Payment, Generation, Referral)
│   └── utils/             # Утилиты
│
├── docs/                   # 📚 Документация
│   ├── README.md          # Описание документации
│   ├── REFERRAL_SYSTEM_CHANGES.md
│   ├── ИНСТРУКЦИЯ_ПО_ТЕСТАМ.md
│   └── ... (все .md файлы)
│
├── tests/                  # 🧪 Тесты
│   ├── README.md          # Описание тестов
│   ├── test_referral_flow.js
│   ├── test_expert_referral_flow.js
│   ├── test_full_system.js
│   └── ... (все test_*.js файлы)
│
├── scripts/                # 🔧 Скрипты
│   ├── README.md          # Описание скриптов
│   ├── start.sh           # Запуск бота
│   ├── stop.sh            # Остановка бота
│   ├── add_quota_manually.js
│   └── ... (все скрипты)
│
├── media/                  # 🎨 Медиа файлы
│   ├── README.md          # Описание медиа
│   ├── start.png          # Приветственное изображение
│   ├── veo3.png           # Процесс генерации
│   ├── mother.MP4         # Видео мемов
│   └── ... (все изображения и видео)
│
├── utils/                  # 🛠️ Утилиты
│   ├── README.md          # Описание утилит
│   ├── supervisor_meemee.conf
│   └── ... (конфиг файлы)
│
├── logs/                   # 📝 Логи
├── node_modules/           # 📦 Зависимости
├── .env                    # 🔐 Переменные окружения
├── package.json            # 📋 Зависимости проекта
└── README.md               # 📖 Главная документация
```

## 🚀 Быстрый старт

### Установка
```bash
npm install
```

### Запуск
```bash
./scripts/start.sh
or 
pm2 start src/bot_start.js --name meemee_bot
pm2 start src/bot_start_admin.js --name meemee_bot_admin
pm2 start src/redis.js --name meemee_redis
pm2 start src/backend/index.js --name meemee_backend
```

### Тестирование
```bash
# Тест реферальной системы
node tests/test_referral_flow.js
node tests/test_expert_referral_flow.js

# Полное тестирование
node tests/test_full_system.js
```

## 📚 Документация

Вся документация находится в папке `docs/`:
- [Инструкция по тестам](docs/ИНСТРУКЦИЯ_ПО_ТЕСТАМ.md)
- [Изменения реферальной системы](docs/REFERRAL_SYSTEM_CHANGES.md)
- [Деплой на сервер](docs/DEPLOY_TO_SERVER.md)

## 🧪 Тесты

Все тесты находятся в папке `tests/`. Подробнее см. [tests/README.md](tests/README.md)

## 🔧 Скрипты

Все скрипты находятся в папке `scripts/`. Подробнее см. [scripts/README.md](scripts/README.md)

## 🎨 Медиа

Все медиа-файлы находятся в папке `media/`. Подробнее см. [media/README.md](media/README.md)

## ⚙️ Конфигурация

- `.env` - переменные окружения (не коммитится)
- `.env.example` - пример переменных окружения
- `src/config.js` - конфигурация бота

## 🔑 Основные функции

- ✅ Генерация видео-мемов с помощью AI
- ✅ Реферальная система (обычная и экспертная)
- ✅ Платежи (крипто и фиат)
- ✅ Админ-панель
- ✅ Рассылки
- ✅ Inline режим
- ✅ Статистика

##  СМОТРИМ ВСЕ В ДИРЕКТОРИИ /docs

## 📞 Контакты

Разработчик: @ivasoft
Владелец: @aiviral_manager
# meme_test_telegram_bot
