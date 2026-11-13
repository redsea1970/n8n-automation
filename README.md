# n8n Automation Portfolio

5 учебно-демонстрационных workflow n8n:

1. **01-telegram-notify** — Manual Trigger → Telegram Send Message
2. **02-google-sheets** — OAuth2 + Append Row (Name/Date/Status)
3. **03-parse-api** — Schedule + HTTP Request (JSON) + Code + Append Row
4. **04-ai-agent-telegram** — Telegram Trigger → AI Agent (OpenAI gpt-4o-mini) → Send Message
5. **05-release-digest** — Schedule → releases.atom → Code → Sheets → OpenAI summary → Telegram

## Запуск

### Вариант A: npm (WSL2)
```bash
npm install -g n8n
n8n start
```

### Вариант B: Docker
```bash
docker compose up -d
```

Редактор: http://localhost:5678

## Безопасность

Секреты (Bot Token, Chat ID, OpenAI key, OAuth JSON) — только через n8n Credentials. В репо — лишь `.env.example`.

## Структура

- `workflows/` — JSON-экспорты (импортируются в n8n)
- `docs/` — пошаговые инструкции по блокам 1–5
- `screenshots/` — плейсхолдеры (заполняются вручную)
