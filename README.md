# marketing_campaign

AI-based **Marketing Campaign Generator** project: exploratory analysis of product data in SQLite, LangChain SQL and campaign agents, output guardrails, and generated campaign assets (title, email draft, CTA).

## Contents

| File | Description |
|------|-------------|
| `Campaign Generator Fullcode Notebook (2).ipynb` | Full implementation: EDA, LLM setup, SQL agent, campaign agent, guardrails, campaign generator, tests for two Product IDs. |
| `Campaign Generator Lowcode Notebook (2).ipynb` | Template / low-code variant with blanks to complete. |
| `products.db` | SQLite database with `products` table (product_id, product_name, target_age, target_profession, product_details). |
| `config.example.json` | Example API configuration; copy to `config.json` locally (not committed). |

## Setup

1. Python 3.x; install packages from the pip cell in the notebook (OpenAI, LangChain, pandas, etc.).
2. Copy `config.example.json` to `config.json` and add your OpenAI API key and base URL, **or** set credentials in the notebook cell as documented there.
3. **Google Colab:** Upload `products.db` to `/content/` (or mount Drive and point `db_path` accordingly). **Local:** Run the notebook from this directory so `products.db` resolves.

## Run order

Run all cells top to bottom after installing dependencies and restarting the kernel (per notebook note).

## Security

Do not commit `config.json` or real API keys. The committed notebook uses a placeholder for the API key; rotate any key that was ever committed elsewhere.
