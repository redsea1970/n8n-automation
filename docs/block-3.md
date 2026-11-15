# Блок 3: Парсинг API и Code

**Цель:** Автоматический парсинг курса валют по расписанию.

## Как это работает
1. `Schedule Trigger` запускает процесс каждую минуту.
2. `HTTP Request` делает GET-запрос к открытому API курсов валют (exchangerate-api).
3. `Code` извлекает из ответа дату и нужную валюту (RUB), формируя JSON.
4. `Google Sheets (Append Row)` записывает результат в таблицу.

## Импорт
Загрузите `workflows/03-parse-api.json`. Подключите свой Credential Google Sheets и укажите ID таблицы.
