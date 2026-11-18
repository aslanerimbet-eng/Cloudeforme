# Telegram Bot

Простой шаблон бота на Python (python-telegram-bot) для деплоя на Railway.

## Локальный запуск

1. Создай бота через [@BotFather](https://t.me/BotFather) и получи токен.
2. Скопируй `.env.example` в `.env` и вставь токен:
   ```
   BOT_TOKEN=твой_токен
   ```
3. Установи зависимости:
   ```
   pip install -r requirements.txt
   ```
4. Запусти:
   ```
   python bot.py
   ```

## Деплой на Railway

1. Залей этот репозиторий на GitHub.
2. В Railway: New Project → Deploy from GitHub repo → выбери репозиторий.
3. В разделе Variables добавь `BOT_TOKEN` со значением токена.
4. Railway сам подхватит `Procfile` и `requirements.txt` и запустит бота.

## Структура

- `bot.py` — код бота (команды `/start`, `/help`, эхо на сообщения)
- `requirements.txt` — зависимости
- `Procfile` — команда запуска для Railway
- `.env.example` — пример переменных окружения
