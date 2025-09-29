# 🚀 Инструкция по деплою на Vercel

## ✅ Все файлы готовы!

### 📁 Структура проекта:
```
1waion.CAVEMINES/
├── server.js                    # Основной сервер
├── vercel.json                  # Конфигурация Vercel
├── package.json                 # Зависимости
├── predictor.html               # Предсказатель
├── predictor-setup.html         # Настройка предсказателя
├── prod-rnd-frontend-php-orchestra.100hp.app/
│   ├── mines/
│   │   └── index.html           # Главная страница игры
│   └── static/
│       ├── js/
│       │   ├── main.95a51fb23a11010e8f6e.js
│       │   └── runtime.830375236abe52ab9f6f.js
│       └── css/
│           └── main.144a5b0d.css
└── prod-rnd-backend-php-orchestra.100hp.app/
    └── mines/
        └── settings.html        # Настройки игры
```

## 🎯 Способы деплоя:

### 1. Через Vercel CLI (рекомендуется):
```bash
# Установить Vercel CLI
npm install -g vercel

# Войти в аккаунт
vercel login

# Деплой
vercel --prod
```

### 2. Через веб-интерфейс Vercel:
1. Зайти на https://vercel.com
2. Нажать "New Project"
3. Подключить GitHub репозиторий
4. Выбрать папку с проектом
5. Нажать "Deploy"

### 3. Через GitHub:
1. Загрузить все файлы в GitHub репозиторий
2. Подключить репозиторий к Vercel
3. Автоматический деплой при push

## 🔧 Что исправлено:

1. ✅ **Сервер запускается локально** - добавлен код запуска
2. ✅ **Созданы отсутствующие JS файлы** - main.js и runtime.js
3. ✅ **Исправлена обработка корневого пути** - `/` отдает mines игру
4. ✅ **Предсказатель работает** - привязан к Player ID
5. ✅ **Статические файлы работают** - CSS, JS загружаются

## 🎮 После деплоя:

- **Главная страница**: `https://your-app.vercel.app/`
- **Mines игра**: `https://your-app.vercel.app/mines/`
- **Предсказатель**: `https://your-app.vercel.app/predictor-setup`
- **API**: `https://your-app.vercel.app/mines/...`

## 📱 Предсказатель:

1. Открыть игру
2. F12 → Console → найти "🎮 Player ID for Predictor"
3. Скопировать ID
4. Открыть `/predictor-setup`
5. Вставить ID и запустить предсказатель

**🎉 Готово к деплою!** 🚀
