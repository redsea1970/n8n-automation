# n8n Automation Portfolio

Коллекция из 5 учебно-демонстрационных workflow на платформе **n8n**.

## 📂 Блоки
- **[Блок 1: Telegram-уведомления](docs/block-1.md)** — Manual Trigger → Telegram Send Message
- **[Блок 2: Google Sheets](docs/block-2.md)** — OAuth2 → Append Row (Name/Date/Status)
- **[Блок 3: Парсинг API](docs/block-3.md)** — Schedule → HTTP Request → Code → Google Sheets
- **[Блок 4: AI-агент](docs/block-4.md)** — Telegram Trigger → AI Agent (OpenAI) → Send Message
- **[Блок 5: Release Digest](docs/block-5.md)** — Schedule → Atom → Code → Sheets → OpenAI → Telegram

## 🚀 Запуск
### Вариант A: локально через npm (WSL2)
```bash
npm install -g n8n
n8n start
```
### Вариант B: Docker
```bash
docker compose up -d
```
Редактор: `http://localhost:5678` (или `5679`, если порт занят).

## 🔒 Безопасность
Все секреты (Telegram Bot Token, OpenAI API Key, Google OAuth2) хранятся **только в n8n Credentials**. В репозитории — только `.env.example` без реальных значений.

## 📦 Импорт workflow
1. Откройте n8n → Workflows → Import from file.
2. Выберите нужный `.json` из папки `workflows/`.
3. Создайте Credentials для Telegram/Google/OpenAI и укажите их в узлах.

## ���� 6: Uptime Monitor
�������� ����������� ����� ������ 5 ����� � ������������ � Telegram ��� �����. ���������: [docs/block-6.md](docs/block-6.md)
