# 💊 RxSaathi – Symptom & Prescription Assistant (RAG-powered)

---

## 📝 Overview  

**RxSaathi** is an **AI-powered chatbot** that helps users understand medical symptoms in simple language and provides **educational insights** about medicines and prescriptions using **RAG (Retrieval-Augmented Generation)**.  

⚠️ **Disclaimer:** This app is **not a medical device**. It does **not prescribe** or diagnose. It only summarizes trusted medical information. Always consult a **licensed doctor** for actual treatment.  

👨‍💻 **Author:** *Vivek Yadav – FullStack Developer (AI/ML)*  

---

## ✨ Features  

- 🩺 **Symptom Explainer** – User-friendly explanation of symptoms  
- 📚 **RAG-powered Prescription Info** – Retrieves medicine details (vector embeddings)  
- 🔐 **SSO Authentication** – Secure login via OAuth (Google/GitHub)  
- 🤖 **LangChain + OpenAI** – Smart conversational AI pipeline  
- 🧾 **Citations & Sources** – All answers come with references  
- 🚨 **Safety Guardrails** – No prescriptions, triage alerts for emergencies  

---

## 🏗️ Tech Stack  

| Layer        | Tech Used |
|--------------|-----------|
| 🎨 Frontend  | React + Vite, Tailwind/Chakra (optional UI lib) |
| ⚡ Backend   | Python FastAPI, Uvicorn, Pydantic |
| 🧠 AI / RAG  | LangChain, OpenAI API (Chat + Embeddings) |
| 📦 Vector DB | FAISS / Chroma (Dev) • PGVector (Prod) |
| 🔑 Auth      | OAuth (Google/GitHub) + JWT |
| 🗄️ Storage   | PostgreSQL (users, chat logs, metadata) |

---

## 📂 Project Structure  


---

## 🔒 Safety & Compliance  

✔️ Never prescribes or adjusts dosage  
✔️ Always cites sources  
✔️ Detects **red-flag symptoms** → emergency warning  
✔️ Clear **country-specific disclaimers**  
✔️ Data privacy (user consent + deletion option)  

---

## ⚙️ Setup & Installation  

### 1️⃣ Prerequisites  
- Node.js 18+  
- Python 3.10+  
- Docker & PostgreSQL (optional for prod)  

---

### 2️⃣ Backend Setup (FastAPI)  

```bash
cd apps/api
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

# Run FastAPI
uvicorn main:app --reload --port 8000
