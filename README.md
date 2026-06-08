# Weekly Reporting — LangGraph + Swytchcode

Automates weekly metric reporting across tools:
1. Loads report data (hardcoded sample — Google Sheets integration coming soon)
2. Creates a Notion report page
3. Emails a summary to stakeholders via Resend

Built with [LangGraph](https://github.com/langchain-ai/langgraph) and [Swytchcode](https://swytchcode.com).

---

## Setup

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Copy and fill in your API keys
cp .env.example .env

# 3. Fetch all integrations
swytchcode bootstrap
```

## Run

```bash
python main.py
```

## Canonical IDs Used

| Service | Canonical ID          |
|---------|-----------------------|
| Notion  | `pages.page.create`   |
| Resend  | `emails.email.create` |
