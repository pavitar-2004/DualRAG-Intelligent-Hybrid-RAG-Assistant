# DualRAG-Intelligent-Hybrid-RAG-Assistant

Enterprise-grade Hybrid Retrieval-Augmented Generation (RAG) AI assistant that combines document intelligence with general LLM reasoning using Qdrant vector search, NVIDIA semantic reranking, OpenRouter embeddings, and Google Gemini 2.5 Flash.

DualRAG can answer:
- 📄 Questions from uploaded documents
- 🌐 General knowledge questions
- 💬 Conversational follow-up queries

while providing source-backed responses through a modern ChatGPT-style interface.

---

# 🚀 Features

## 🧠 Hybrid Intelligence
- Retrieval-Augmented Generation (RAG)
- General AI answering fallback
- Confidence-based retrieval filtering

## 📄 Document Processing
- Upload and index documents
- Semantic chunking
- Vector embeddings generation
- Qdrant vector storage

## 🔍 Intelligent Retrieval
- Semantic vector search
- NVIDIA reranking pipeline
- Context-aware retrieval

## 💬 Conversational Experience
- ChatGPT-like UI
- Streaming responses
- Conversational memory
- Persistent chat history
- Markdown rendering

## 📚 Source Attribution
- Source citations
- Retrieved document references
- Confidence scoring

---

# 🏗️ Tech Stack

## Frontend
- Vite
- Vanilla JavaScript
- HTML/CSS

## Backend
- Python
- FastAPI

## AI Infrastructure
- Google Gemini 2.5 Flash
- OpenRouter Embeddings
- NVIDIA Reranker
- Qdrant Vector Database

---

# ⚙️ System Architecture

```text
User Query
    ↓
Embedding Generation
    ↓
Qdrant Vector Retrieval
    ↓
NVIDIA Semantic Reranking
    ↓
Context Construction
    ↓
Gemini Response Generation
    ↓
Final Answer + Sources

**📁 Project Structure**
dualrag/
│
├── backend/
│   ├── api/
│   ├── core/
│   ├── services/
│   ├── storage/
│   ├── requirements.txt
│   ├── app.py
│   └── .env.example
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
│
├── README.md
├── LICENSE
└── .gitignore

**Required API Keys**

Create a .env file inside backend/.

Required:

OpenRouter API Key
Google Gemini API Key
NVIDIA API Key

🛠️ Local Setup
1. Start Qdrant
docker run -p 6333:6333 qdrant/qdrant
2. Start Backend
cd backend
venv\Scripts\activate
python app.py
Backend runs on:
http://localhost:8000
3. Start Frontend
cd frontend
npm install
npm run dev

Frontend runs on:
http://localhost:5173
🌟 **Usage**
Upload documents
Ask questions from uploaded files
Ask general knowledge questions
Receive intelligent contextual responses
View cited document sources
🔥** Core Highlights**
Hybrid RAG + General AI architecture
Semantic retrieval pipeline
Context-aware answer generation
Source-backed responses
Full-stack implementation
Streaming AI responses
Memory-enabled conversations
Production-style backend structure

**Future Improvements**
PDF/DOCX advanced parsing
Multi-user authentication
Cloud deployment
Voice interaction
Advanced memory system
Multi-modal retrieval
