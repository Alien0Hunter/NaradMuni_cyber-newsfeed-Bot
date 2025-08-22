# n8n CyberSecurity News Feeds → Telegram 

One‑click n8n workflow that polls several security RSS feeds and posts formatted headlines to Telegram.
https://www.linkedin.com/posts/cbbobhate_bot-n8n-cybersecurity-activity-7360658077064343553-1uaM?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAABkCw-wBhyGewVYWEa7ruGWgkRa2Vpefr8I 

🚨 Never Miss a Cyber Threat Again
Meet my telegram AI-Powered Cybersecurity Threat & News hashtag#Bot 🤖 — built with hashtag#n8n + Telegram for instant updates.

Get real-time alerts from:
⚡ Hacker News
⚡ BleepingComputer
⚡ CISA Alerts

## Features
- Sources: Hacker News (security), BleepingComputer, Krebs, CISA alerts
- Merge + de‑dupe + limit to top N items
- Nicely formatted message (`title → link → date`) sent to Telegram
- Hourly schedule (Cron) by default

## Quick Start
1. **Import the workflow**
   - In n8n → *Workflows* → *Import from File* → select `workflows/news_to_telegram.json`.

2. **Set credentials**
   - Open the **Send a text message (Telegram)** node.
   - Create/select your **Telegram credential** (Bot token from `@BotFather`).  
   - In **Chat ID**, enter your user/channel chat id (e.g., `281072746` or `-100xxxxxxxxxx`).

3. **Run once**
   - Click **Execute workflow** to test. You should receive 10 messages.

4. **Turn it on**
   - Toggle the workflow to **Active** so the **Cron** runs every hour.

## Changing Feeds or Frequency
- Add/remove RSS nodes and point them into the **Merge Feeds** node.
- Edit **Cron** node to set your own schedule (e.g., every 6 hours).

## Repo Layout
```
workflows/
  └── news_to_telegram.json   # Import this into n8n
.gitignore
LICENSE
README.md
```

## Deploy to GitHub
```bash
git init
git add .
git commit -m "n8n: cybersecurity news to Telegram workflow"
git branch -M main
git remote add origin <YOUR_REPO_URL>
git push -u origin main
```

🔒 Stay informed. Stay secure. Stay Connected https://www.linkedin.com/in/cbbobhate/
