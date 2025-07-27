# 🤖 Smart Upwork Screener

**Smart Upwork Screener** is a Telegram bot that helps freelancers monitor Upwork in real time – *no RSS needed*.  
It scrapes job listings using Upwork's internal API, filters them through an LLM based on your skillset, and pings your Telegram only when there's a relevant match.

---

## 🚀 Features

- 🔎 Scrapes latest jobs via Upwork’s internal (unofficial) JSON API
- 🧠 Filters each post using a pluggable LLM (OpenAI, Ollama, etc.)
- 📬 Sends relevant jobs straight to your Telegram chat
- ⚙️ Fully customizable filter logic (skill tags, prompt, relevance scoring)
- 🔄 Designed for automation & extensibility

---

## 🛠️ Tech Stack

- Python 3.10+
- `requests` or `httpx` for API calls
- `python-telegram-bot`
- `openai`, `llama-cpp-python`, `ollama`, or `transformers`
- Optional: `apscheduler` or `asyncio` for polling

---

## 📌 Use Case

You're a backend dev (e.g. Python + AWS + FastAPI). Instead of checking Upwork manually, the bot auto-fetches job listings, evaluates them using your skill profile, and notifies you instantly when a match is found – saving time and energy.

---

## ⚠️ Notes

- 🚫 **No RSS used** – Upwork deprecated RSS feeds in August 2024
- 🔐 Uses **unofficial API**, subject to change if Upwork updates their frontend
- 🛡 Consider using headers or proxies to bypass scraping blocks if needed

---

## 🔮 Roadmap

- [ ] Add local database or file cache for processed job deduplication
- [ ] Multi-query support with config files
- [ ] GUI or CLI config editor for prompt/skills
- [ ] Local-only LLM fallback with dynamic switching

---

## 📂 Project Structure

