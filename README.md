Here’s a **clean, professional README.md** you can directly use for your GitHub repo 👇

---

# 📱 AI-Powered MSME Business Advisor for Kirana Stores

A **WhatsApp-based AI assistant** that helps small kirana store owners manage their business using **voice, text, and images**.

---

## 🚀 Problem Statement

Millions of small shop owners in India:

* Don’t track cash flow properly
* Struggle with GST understanding
* Rely on memory for credit (udhar)
* Lack access to business insights

👉 This project provides a **simple, WhatsApp-first AI solution**.

---

## 💡 Solution

A smart assistant that:

* Works directly on WhatsApp
* Accepts voice notes, receipts, and text
* Provides actionable business insights in Hindi

---

## ✨ Features

### 🔥 Core Features

* 📊 **Cash Flow Guard**
  Tracks income vs expenses and warns about losses

* 💰 **Conversational GST Assistant**
  Answers questions like *“Can I pay GST?”* in simple language

* 📒 **Udhar (Credit) Tracker**
  Tracks customer credit and payments

* 📱 **WhatsApp AI Assistant**
  Full chatbot interface using WhatsApp

---

### ⚡ Additional Features

* 🎤 **Voice Input (Hinglish)**
  Speak instead of typing

* 📷 **OCR (Assistive Receipt Scanner)**
  Extract data from handwritten/printed bills

* 📊 **Dashboard**
  Visual overview of business performance

---

### 🚀 Smart Features

* 🤖 **AI Suggestions**
  “What should I do today?”

* 📉 **Loss Detection**
  Explains why profit is low

* 🌍 **Community Insights (Demo)**
  Trending products in nearby stores

---

## 🧱 Tech Stack

| Layer     | Technology            |
| --------- | --------------------- |
| Interface | WhatsApp (Twilio API) |
| Backend   | FastAPI (Python)      |
| AI Models | OpenAI (GPT, Whisper) |
| OCR       | Google Vision API     |
| Database  | MongoDB / Firebase    |
| Cache     | Redis                 |
| Frontend  | React + Tailwind      |
| Hosting   | Render / Vercel       |

---

## ⚙️ System Architecture

```
User (WhatsApp)
        ↓
Twilio WhatsApp API
        ↓
FastAPI Backend (Webhook)
        ↓
--------------------------------
| Input Processing            |
| - Speech-to-Text (Whisper) |
| - OCR (Vision API)         |
--------------------------------
        ↓
--------------------------------
| Business Logic             |
| - Cash Flow Engine        |
| - GST Engine              |
| - Udhar Tracker           |
--------------------------------
        ↓
Database + Cache
        ↓
Response → WhatsApp / Dashboard
```

---

## ⚡ Low Latency Design

* ✅ Instant responses for:

  * GST queries
  * Cash flow queries

* 🔁 Background processing:

  * OCR
  * Voice

* 🧠 Precomputed:

  * Profit
  * GST
  * Udhar balances

---

## 🛠️ Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/your-username/kirana-ai-assistant.git
cd kirana-ai-assistant
```

---

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

---

### 3. Run FastAPI server

```bash
uvicorn main:app --reload
```

---

### 4. Expose server using ngrok

```bash
ngrok http 8000
```

Copy the HTTPS URL.

---

### 5. Setup WhatsApp Bot (Twilio)

1. Go to Twilio Console
2. Open **WhatsApp Sandbox**
3. Join sandbox via WhatsApp
4. Set webhook URL:

```
https://your-ngrok-url/webhook
```

---

## 🧪 Example Commands

| Input              | Output        |
| ------------------ | ------------- |
| `sale 500`         | Adds sale     |
| `expense 200`      | Adds expense  |
| `gst?`             | GST response  |
| `ramesh udhar 200` | Tracks credit |

---

## 🎯 Demo Flow

1. Add sales via WhatsApp
2. Ask GST question
3. Add udhar entry
4. Upload receipt (OCR demo)
5. Show dashboard

---

## ⚠️ Limitations

* OCR accuracy depends on handwriting
* Community insights use demo data
* GST calculations are simplified

---

## 🚀 Future Improvements

* Multi-language support
* Better OCR model
* Real-time community insights
* Loan recommendation system

---

## 🏆 Impact

* Helps small businesses make better decisions
* Reduces manual bookkeeping
* Improves financial awareness

---

## 👨‍💻 Team

* Team Name: NaN Sense
* Lead: PM Razeen

---

## 📄 License

MIT License
