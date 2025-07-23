# 🧠 AI Sales Assistant

A local LLM-powered assistant that lets you upload Excel files, ask questions in natural language, and receive answers with charts and insights!

## 🚀 Features
- Upload `ad_sales`, `total_sales`, and `eligibility` Excel files
- Ask natural language questions like:
  - What is my total sales?
  - What is the RoAS?
  - Which product had the highest CPC?
- Get answers in plain English
- Auto-generate charts

## 📦 Setup

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run the app (requires Ollama + Mistral pulled)

```bash
uvicorn main:app --reload
```

Visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 🧪 Example curl

```bash
curl -X POST http://localhost:8000/ask/ -H "Content-Type: application/json" -d '{ "question": "What is my total sales?" }'
```

## 📁 File Upload UI
Use the web UI at `/` to upload:
- `Product level Adsales.xlsx`
- `Product level Total sales.xlsx`
- `Product level Eligibility.xlsx`

Enjoy!
