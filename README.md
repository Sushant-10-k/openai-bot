# Perplexity-2.0-ChatBot

# 🤖 OpenAI LLaMA3 Chatbot (Fullstack)

A fullstack chatbot application powered by [Ollama](https://ollama.com/) and LLaMA3, with a React + Vite frontend and a Node.js + Express backend. The backend uses your local GPU to run LLaMA3 efficiently and cost-free!

---

## 🚀 Features

- 💬 AI chatbot using LLaMA3 via Ollama
- 🎯 Frontend built with React & TailwindCSS (Vite)
- ⚙️ Backend built with Node.js + Express
- 🔐 Secure environment with `.env` support
- 🔄 Connects locally via REST API (`/api/chat`)

---

## 📁 Project Structure

openai-bot/
├── backend/ # Node.js + Express backend (Ollama client)
│ ├── server.js
│ ├── .env # Contains OPENAI_API_KEY (optional)
│ └── package.json
├── frontend/ # React + Vite frontend
│ ├── src/
│ ├── tailwind.config.js
│ └── package.json
└── README.md


---

## ⚙️ Getting Started

### 🧠 Prerequisites

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [Ollama](https://ollama.com/) (local LLaMA3 model runner)
- Git installed

### 🛠️ Backend Setup

```bash
cd backend
npm install
# Add your environment variable
echo PORT=3000 >> .env
# Start the server
npm run dev

Frontend Setup

cd frontend
npm install
npm run dev

Local GPU Inference with Ollama

Make sure you have pulled the model:

ollama pull llama3
ollama serve
