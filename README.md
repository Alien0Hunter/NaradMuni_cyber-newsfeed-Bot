# Cyber-Security News Feed Bot (n8n → Telegram)

Pulls security news from multiple RSS feeds, formats nicely, and posts to Telegram (DM, group, or channel).

## Features
- Sources: The Hacker News, BleepingComputer, Krebs on Security, CISA Alerts
- Merged + capped to latest 10 items
- Message format:
  📰 <title>
  🔗 <link>
  🕒 <published time>

## Setup
1. Create a Telegram bot via @BotFather and get the token.
2. Add the bot to your channel/group or DM it.
3. Import the workflow into n8n (`news_to_telegram.json`).
4. Add your Telegram credential to the **Send to Telegram** node.
5. Set your chat ID (numeric or @channelusername).
6. Activate the workflow and it will fetch + post every hour.

## License
MIT
