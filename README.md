# ENG:
# 🤖 A friend search bot with a rating system

A Telegram bot for finding friends with a rating system, likes and "poop" (dislikes). An analogue of popular bots like "Davinchik".

## ✨ Opportunities

### 🎯 Main functions
- **Rating system**: Likes (❤️) and "poop" (💩) to rate other users
- **Rating System**: Dynamic ELO rating that changes after each rating
- **Levels and Experience**: Level up for your activity in the bot
- **User Feed**: Random users to rate from your rating range
- **Top Players**: Ranking of the top 10 users by rating

### 👤 User profile
- **Personalization**: Name, Bio, Age, City
- **Avatar**: The ability to set a profile photo
- **Statistics**: Detailed statistics of likes/poop received and delivered
- **Achievements**: Achievement system for various actions
- **Balance**: Internal currency (🔥 Lights and 💎 Crystals)

### 🔄 Interactions
- **Mutual likes**: Shows who liked you back
-**Browsing History**: Tracking who viewed your profile
- **Complaint system**: An opportunity to complain about violators
- **Admin Panel**: Bot management for administrators

## 🚀 Quick Start

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/dating-bot.git
cd dating-bot
```

2. **Install dependencies:**
```bash
pip install -r requirements.txt
```

3. **Set up the bot:**
- Get the bot token from [@BotFather](https://t.me/BotFather )
   - Insert the token into the file `bot.py `:
``python
   BOT_TOKEN = "YOUR_TOKEN IS HERE"
   ``
- Enter your ID in the list of administrators:
   ```python
   ADMIN_IDS = [YOUR_ID_ HERE] # You can find out the ID from @userinfobot
   ```

4. **Launch the bot:**
```bash
python bot.py
```

## 📱 Bot Commands

### Basic Commands
- `/start` - Start working with the bot, register
- `/help' - Help for commands
- `/profile` - Show your profile
- `/feed' - Show the feed of users for evaluation
- `/top` - Top rated players
- `/stats` - Bot stats and your stats

### Profile Commands
- `/edit_profile' - Edit profile
- `/set_avatar' - Set avatar (send photo)
- `/rules` - Bot rules
- `/donate` - To support the project

## 🎮 How rating works

### Rating system:
- **Like**: +10-20 to the user's rating, +1 to your rating
- **💩 Turd**: -10-20 to the user's rating, -1 to your rating

### Level system:
- Experience is awarded for each action
- Level = (Experience/100) + 1
- Each level provides new opportunities

### Currencies:
- **🔥 Lights**: Awarded for activity (likes, daily entry)
- **💎 Crystals**: Premium currency (not used yet, reserved)

## 🗄️ Database structure

### Main tables:
- **users** - user data (rating, level, statistics)
- **interactions** - interactions between users (likes/poop)
- **profile_views** - profile browsing history
- **reports** - complaints about users
- **achievements** - user achievements

## ⚙️ Technical mishmash

- **Python 3.8+**
- **aiogram 3.x**
- **aiosqlite** - asynchronous SQLite
- **Pillow** - working with images

## 🛡️ Security and moderation

- **Data validation**: Checking the age, length of the text
- **Complaint System**: Users can complain about violators
- **Admin Panel**: Administrators can view complaints and ban users
- **Anti-cheating**: Limits on the number of ratings per day

## 🤝 Participation in the development

1. Fork the repository
2. Create a branch for the new feature:
```bash
git checkout -b feature/new-feature
``
3. Commit the changes:
```bash
git commit -am 'Added a new feature'
``
4. Submit the changes:
```bash
git push origin feature/new-feature
````
5. Create A Pull Request

## 📝 Usage Rules

1. **Minimum age**: 12 years
2. **Respect for others**: No insults or spam
3. **Content**: Avatars with violence, pornography, and drug propaganda are prohibited
4. **Fair Play**: Rating cheating is prohibited
5. **Privacy**: Do not share personal information

## 🆘 Support

### Common problems:
1. **The bot does not start**: Check the token and the Python version
2. **Database Errors**: Delete the `dating_bot.db` file and restart the bot
3. **Users do not appear**: Multiple registered users are needed

### Contacts:
- Create an Issue in the repository for bugs and suggestions
- Write in Telegram: @username (if any)
- Email: your.email@example.com

## 🎉 Thanks

- To the Telegram Developer Community
- To all testers and users of the bot


---

* **If you liked the project, put a star on GitHub!** ⭐

**Enjoy using it! Make new friends and increase your rating!** 🚀

---

## 🔗 Useful links

- [aiogram documentation](https://docs.aiogram.dev /)
- [Telegram Bot API](https://core.telegram.org/bots/api )
- [Usage Examples](https://github.com/aiogram/aiogram/tree/dev-3.x/examples )
- [Bot Templates](https://github.com/MasterGroosha/telegram-bot-template )


## 💡 Ideas and suggestions

Do you have an idea how to improve the bot? Create an Issue with the label `enhancement'!

---

**Created with ❤️ for the Telegram community**


# RU:
# 🤖 Бот для поиска друзей с рейтинговой системой

Telegram-бот для поиска друзей с системой рейтингов, лайков и "какашек" (дизлайков). Аналог популярных ботов вроде "Давинчика".

## ✨ Возможности

### 🎯 Основные функции
- **Система оценок**: Лайки (❤️) и "какашки" (💩) для оценки других пользователей
- **Рейтинговая система**: Динамический рейтинг ELO, который меняется после каждой оценки
- **Уровни и опыт**: Повышайте уровень за активность в боте
- **Лента пользователей**: Случайные пользователи для оценки из вашего рейтингового диапазона
- **Топ игроков**: Рейтинг топ-10 пользователей по рейтингу

### 👤 Профиль пользователя
- **Персонализация**: Имя, био, возраст, город
- **Аватарка**: Возможность установить фото профиля
- **Статистика**: Подробная статистика лайков/какашек полученных и поставленных
- **Достижения**: Система достижений за различные действия
- **Баланс**: Внутренняя валюта (🔥 Огни и 💎 Кристаллы)

### 🔄 Взаимодействия
- **Взаимные симпатии**: Показывает, кто лайкнул вас в ответ
- **История просмотров**: Отслеживание, кто смотрел ваш профиль
- **Система жалоб**: Возможность пожаловаться на нарушителей
- **Админ-панель**: Управление ботом для администраторов

## 🚀 Быстрый старт

### Установка

1. **Клонируйте репозиторий:**
```bash
git clone https://github.com/yourusername/dating-bot.git
cd dating-bot
```

2. **Установите зависимости:**
```bash
pip install -r requirements.txt
```

3. **Настройте бота:**
   - Получите токен бота у [@BotFather](https://t.me/BotFather)
   - Вставьте токен в файл `bot.py`:
   ```python
   BOT_TOKEN = "ВАШ_ТОКЕН_ЗДЕСЬ"
   ```
   - Укажите ваш ID в списке администраторов:
   ```python
   ADMIN_IDS = [ВАШ_ID_ЗДЕСЬ]  # Узнать ID можно у @userinfobot
   ```

4. **Запустите бота:**
```bash
python bot.py
```

## 📱 Команды бота

### Основные команды
- `/start` - Начать работу с ботом, регистрация
- `/help` - Справка по командам
- `/profile` - Показать ваш профиль
- `/feed` - Показать ленту пользователей для оценки
- `/top` - Топ игроков по рейтингу
- `/stats` - Статистика бота и ваша статистика

### Команды профиля
- `/edit_profile` - Редактировать профиль
- `/set_avatar` - Установить аватар (отправить фото)
- `/rules` - Правила бота
- `/donate` - Поддержать проект

## 🎮 Как работает рейтинг

### Система оценок:
- **❤️ Лайк**: +10-20 к рейтингу пользователя, +1 к вашему рейтингу
- **💩 Какашка**: -10-20 к рейтингу пользователя, -1 к вашему рейтингу

### Уровневая система:
- Опыт начисляется за каждое действие
- Уровень = (Опыт/100) + 1
- Каждый уровень даёт новые возможности

### Валюты:
- **🔥 Огни**: Начисляются за активность (лайки, ежедневный вход)
- **💎 Кристаллы**: Премиум-валюта (пока не используется, зарезервировано)

## 🗄️ Структура базы данных

### Основные таблицы:
- **users** - данные пользователей (рейтинг, уровень, статистика)
- **interactions** - взаимодействия между пользователями (лайки/какашки)
- **profile_views** - история просмотров профилей
- **reports** - жалобы на пользователей
- **achievements** - достижения пользователей

## ⚙️ Техническая мешанина

- **Python 3.8+**
- **aiogram 3.x**
- **aiosqlite** - асинхронный SQLite
- **Pillow** - работа с изображениями

## 🛡️ Безопасность и модерация

- **Валидация данных**: Проверка возраста, длины текста
- **Система жалоб**: Пользователи могут жаловаться на нарушителей
- **Админ-панель**: Администраторы могут просматривать жалобы и банить пользователей
- **Анти-накрутка**: Лимиты на количество оценок в день

## 🤝 Участие в разработке

1. Форкните репозиторий
2. Создайте ветку для новой функции:
```bash
git checkout -b feature/новая-функция
```
3. Зафиксируйте изменения:
```bash
git commit -am 'Добавил новую функцию'
```
4. Отправьте изменения:
```bash
git push origin feature/новая-функция
```
5. Создайте Pull Request

## 📝 Правила использования

1. **Минимальный возраст**: 12 лет
2. **Уважение к другим**: Без оскорблений и спама
3. **Контент**: Запрещены аватары с насилием, порнографией, пропагандой наркотиков
4. **Честная игра**: Запрещены накрутки рейтинга
5. **Конфиденциальность**: Не делитесь личной информацией

## 🆘 Поддержка

### Частые проблемы:
1. **Бот не запускается**: Проверьте токен и версию Python
2. **Ошибки базы данных**: Удалите файл `dating_bot.db` и перезапустите бота
3. **Пользователи не появляются**: Нужно несколько зарегистрированных пользователей

### Контакты:
- Создайте Issue в репозитории для багов и предложений
- Напишите в Telegram: @username (если есть)
- Email: your.email@example.com

## 🎉 Благодарности

- Сообществу Telegram-разработчиков
- Всем тестерам и пользователям бота


---

⭐ **Если вам понравился проект, поставьте звезду на GitHub!** ⭐

**Приятного использования! Находите новых друзей и повышайте свой рейтинг!** 🚀

---

## 🔗 Полезные ссылки

- [Документация aiogram](https://docs.aiogram.dev/)
- [Telegram Bot API](https://core.telegram.org/bots/api)
- [Примеры использования](https://github.com/aiogram/aiogram/tree/dev-3.x/examples)
- [Шаблоны ботов](https://github.com/MasterGroosha/telegram-bot-template)


## 💡 Идеи и предложения

Есть идея как улучшить бота? Создайте Issue с меткой `enhancement`!

---

**Создано с ❤️ для сообщества Telegram**
