# Movie Recommender Telegram Bot

## О проекте
Телеграм-бот, который рекомендует фильмы по названию, используя embeddings описаний фильмов и cosine similarity.

## Как использовать
1. Запусти бота.
2. Отправь название фильма (например, "The Matrix").
3. Получи список похожих фильмов с краткими описаниями.

## Установка

1. Клонируй репозиторий:
```bash
git clone https://github.com/yourusername/movie-recommender-bot.git
cd movie-recommender-bot
Создай виртуальное окружение и активируй его:

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Linux/macOS
source venv/bin/activate

Установи зависимости:

```bash
pip install -r requirements.txt
Создай файл .env в корне проекта и добавь туда токен бота:

```ini
BOT_TOKEN=твой_токен_от_telegram

Запуск бота

```bash
Копировать
Редактировать
python bot.py

Структура проекта

```bash
movie-recommender-bot/
├── bot.py              # Запуск бота
├── recommender.py      # Код с рекомендательной системой
├── data/               # Датасеты и эмбеддинги
│   ├── embeddings.pkl
│   └── movies_cleaned.csv
├── requirements.txt
├── .env                # Секреты (НЕ пушить в git)
└── README.md

Технологии

Python 3.12

python-telegram-bot

pandas

scikit-learn

sentence-transformers

torch