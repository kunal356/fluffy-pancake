# 🧠 ShopSense AI — Smarter Product Decisions, Instantly

Find, compare, and choose the right products faster with an AI that actually understands what you need.

---

## 🚀 What is ShopSense AI?

**ShopSense AI** is a smart product companion that helps you:

* Compare products in seconds
* Get clear, trustworthy answers
* Discover better alternatives tailored to your needs

It combines product data and intelligent search to give responses that are **useful, accurate, and easy to trust** — even across follow-up questions.

---

## ✨ Features

* 💬 **Chat Naturally**
  Ask questions the way you normally would — no keywords needed.

* 🔎 **Instant Comparisons**
  Get side-by-side insights without digging through multiple tabs.

* 🔁 **Better Alternatives**
  Not satisfied? It suggests smarter options automatically.

* 📚 **Fact-Based Answers**
  Responses are backed by real product data and relevant sources.

* 🧠 **Understands Context**
  Remembers what you asked earlier to keep conversations smooth.

* ⚡ **Real-Time Experience**
  Fast, interactive responses in a clean web interface.

---

## 🏗️ How It Works

```
You ask → System finds relevant info → AI processes it → You get a clear answer
```

Behind the scenes, it:

* Finds the most relevant product information
* Combines it with your query
* Generates a response grounded in real data

---

## 🧰 Tech Stack

### 🖥️ Frontend

* Streamlit

### ⚙️ Backend

* FastAPI

### 🧠 Language Models

* Local LLMs (via Ollama)
* Hugging Face Transformers
* OpenRouter (optional)

### 📦 Embeddings

* Sentence Transformers (`all-MiniLM-L6-v2`)

### 🗄️ Data Search

* FAISS
  OR
* ChromaDB

### 📄 Data

* Product dataset (CSV / JSON)
* Optional external sources

---

## 📂 Project Structure

```
├── app/
│   ├── frontend/
│   ├── backend/
│   ├── core/              # search + response logic
│   ├── prompts/
│   ├── evaluation/
│   └── utils/
│
├── data/
│   ├── products.json
│   └── index/
│
├── notebooks/
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup

### 1️⃣ Clone

```bash
git clone https://github.com/yourusername/shopsense-ai.git
cd shopsense-ai
```

---

### 2️⃣ Install

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Prepare Data Index

```bash
python app/core/build_index.py
```

---

### 4️⃣ Run Backend

```bash
uvicorn app.backend.main:app --reload
```

---

### 5️⃣ Start App

```bash
streamlit run app/frontend/app.py
```

---

## 🧪 Evaluation

The system is tested using:

* **Answer Quality** → Does it actually help?
* **Factual Accuracy** → Is it grounded in real data?
* **User Feedback** → Do users find it useful?

---

## 🎯 Design Principles

* Keep answers clear and concise
* Avoid guessing — stick to known data
* Stay helpful across follow-up questions
* Prioritize user intent over keywords

---

## 📸 Example Prompts

* “Which laptop is better for coding under $1000?”
* “Compare iPhone and Samsung for camera quality”
* “Give me a better alternative to this product”

---

## 🚧 What’s Next

* Smarter search (combine keyword + semantic)
* Better UI/UX
* Personalized recommendations
* Voice interaction

---

## 🤝 Contributing

Open to ideas, improvements, and feedback!

---

## 📜 License

MIT License

---

## ⭐ Support

If you like this project, drop a ⭐ on GitHub!

---
