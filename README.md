# Artbent

Статический сайт Artbent. Главная точка входа проекта — `index.html`.

## Локальный тестовый деплой

Из корня проекта:

```bash
python3 -m http.server 8080
```

Откройте <http://localhost:8080/>. Остановка сервера: `Ctrl+C`.

## Структура

- `index.html` — корневая точка входа, открывает главную страницу сайта.
- `Artbent Landing.dc.html` — главная страница сайта с runtime-поддержкой и навигацией по проекту.
- `standalone/Artbent Landing.html` — автономная сборка лендинга с встроенными ресурсами.
- `Artbent *.dc.html` — исходные Design/Code страницы с runtime-поддержкой.
- `design-tokens/` — токены дизайна в CSS и JSON.
- `uploads/` и `screenshots/` — материалы проекта.
- `404.html` — fallback для статического хостинга.

## Публикация

Загрузите содержимое этой папки на любой static hosting. Специальный build step не требуется: хостинг должен раздавать `index.html` из корня проекта.