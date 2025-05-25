# 💸 AI Finance Agent

An intelligent agent powered by OpenAI and Phi SDK that can retrieve and compare financial information such as **stock prices**, **analyst recommendations**, and **fundamentals** for companies using natural language queries.

---

## 🚀 Features

- 💬 Ask questions like:
  - _“Compare Tesla and Microsoft’s stock fundamentals.”_
  - _“Summarize analyst recommendations for Apple and Infosys.”_
- 📊 Displays responses in **formatted markdown tables**.
- 🔧 Integrates financial tools using `yfinance`.
- 🧠 Uses custom tool to convert **company names to stock symbols**.
- ✅ Built-in support for:
  - TSLA, AAPL, MSFT, GOOGL, AMZN, INFY, Phidata

---

## 🛠️ Tech Stack

- **Language**: Python 🐍
- **Agent Framework**: [Phi](https://docs.phidata.io/)
- **Models**: `OpenAI GPT-4o` (default), with support for `Groq LLaMA3`
- **Financial Data Source**: `yfinance`
- **Environment Variables**: managed via `dotenv`

---

## 🧾 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/palak-parhawk-2003/AI-Agents.git
cd AI-Agents
```
### 2. Install dependencies

```bash
pip install phi openai yfinance python-dotenv
```

### 3. Set up .env file

```bash
GROQ_API_KEY=your_groq_api_key_here
OPENAI_API_KEY=your_openai_key_here
```

---

## ▶️ How to Run
```bash
python 2_finance_agent.py
```
This will:
  a. Use the OpenAI GPT-4o model
  b. Invoke custom tool get_company_symbol
  c. Pull real-time data from Yahoo Finance
  d. Print agent response in a readable markdown format

---

## 📌 Notes

1. Ensure your API keys are active and have quota left to avoid RateLimitError.
2. If you encounter Error code: 429 - quota exceeded, check your OpenAI usage.

