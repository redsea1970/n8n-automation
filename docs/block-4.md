# Блок 4: AI-агент в Telegram

**Цель:** Ответы на сообщения в Telegram с помощью нейросети (AI Agent).

## Как это работает
1. `Telegram Trigger` ловит новое сообщение от пользователя.
2. `AI Agent` получает текст сообщения и обрабатывает его с помощью LLM.
3. `OpenAI Chat Model` (опционально) предоставляет модель `gpt-4o-mini`.
4. `Telegram (Send Message)` отправляет ответ обратно в чат.

## Безопасность (Mock)
В репозитории нет реальных ключей OpenAI. Для работы замените фиктивный ключ в Credential на свой. Без ключа workflow можно импортировать для демонстрации структуры.

## Импорт
Загрузите `workflows/04-ai-agent-telegram.json`. Создайте Credential Telegram и OpenAI.

![Схема Блок 4](../screenshots/04-ai-agent.png)
