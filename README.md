# Zomato Spend Analyzer 

An n8n + AI workflow system that:
- Reads Zomato invoices from Gmail
- Extracts spend details using an LLM
- Stores data in Google Sheets
- Generates monthly reports and recipe recommendations
- Sends Telegram alerts at 80% and 100% of your budget

## Workflows

- `workflows/Zomato – Email to Sheet.json`  
  Reads Zomato emails daily, parses invoices, and appends spend data into a Google Sheet.

- `workflows/Zomato – Monthly Report & Recipes.json`  
  Runs monthly, analyzes the past month’s data, generates charts and insights, and emails two reports:
  1) Spend analysis  
  2) Recipe recommendations based on most ordered items.

- `workflows/Zomato – Budget Alerts.json`  
  Checks your monthly spend against your budget and sends Telegram alerts when you hit 80% and 100%.

## Docs

- ![Architecture](docs/architecture-diagram.png)
- ![Sample Monthly Analysis](docs/Sample-monthly-analyis.png)
- ![Sample Monthly Recipes](docs/Sample-monthly-recipes.png)

## Tech Stack

- n8n
- OpenAI / LLMs
- Google Sheets
- QuickChart
- Telegram Bot API

