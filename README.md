# AI Engineer Portfolio — Bala Gali

Senior .NET & Cloud Developer transitioning to AI Engineering.
MSc Computer Science, University of East London.

## Projects

### 1. London Property Q&A Assistant — RAG Pipeline

**Week 2 — Days 5 & 6**

A Retrieval Augmented Generation system built over 
real London property data that answers investor questions 
grounded entirely in the documents — no hallucination.

**v1 — Basic RAG**
- Semantic search over 50 real London property listings
- FAISS vector store with HuggingFace embeddings
- Grounded answers — never hallucinates missing data

**v2 — Production RAG**
- RecursiveCharacterTextSplitter chunking strategy
- MMR retrieval for diverse, non-repetitive results
- Source citations on every answer
- Metadata-based data freshness tracking (2023 vs 2024)
- Pre-computed summary documents for aggregate queries

Stack: Python · LangChain · FAISS · HuggingFace · Groq LLM

📓 [v1 Notebook](property_qa_assistant.ipynb)
📓 [v2 Notebook](property_qa_assistant_v2.ipynb)

---
### 2. London Property AI Assistant — REST API

**Week 2 — Day 7 Capstone Project**

A production-pattern AI application exposing four REST 
endpoints — combining RAG, LangChain memory, structured 
JSON output, and FastAPI into one complete system.

**Endpoints:**
- `POST /ask` — RAG-powered Q&A over 50 real London properties
- `POST /analyse` — Structured JSON investment assessment
- `POST /chat` — Multi-turn conversation with memory
- `GET /health` — Production health check

**What makes this production-ready:**
- FastAPI with Pydantic request/response models
- LangChain LCEL chains for all AI logic
- MMR retrieval with source citations
- Conversation memory persisted across turns
- Auto-generated Swagger UI documentation
- Tested via ngrok public URL

Stack: Python · FastAPI · LangChain · FAISS · 
       HuggingFace · Groq LLM · ngrok · Pydantic

📓 [View Notebook](property_ai_assistant_api.ipynb)

## Skills Being Built
- Python for AI — NumPy, Pandas | ✅ Complete 
- Prompt Engineering — few-shot, CoT, JSON output | ✅ Complete 
- LangChain — chains, memory, pipelines | ✅ Complete 
- RAG — embeddings, FAISS, chunking, MMR | ✅ Complete 
- FastAPI — REST endpoints, Pydantic, Swagger | ✅ Complete 
- AI Agents — tool calling, LangGraph | 🔄 Week 3 
- Azure AI deployment | ⏳ Week 4 
- Azure AI Engineer AI-102 certification | ⏳ Week 4 

## Roadmap
- ✅ Week 1 — Python for AI, data pipelines
- ✅ Week 2 — Prompt engineering, LangChain, RAG
- 🔄 Week 3 — AI agents, tool calling, LangGraph
- ⏳ Week 4 — Capstone project, FastAPI, Azure AI deployment

## Background
7+ years as .NET and Cloud Developer across UK, Thailand, and India.
Currently building toward Generative AI Engineer role in UK market — Q3 2026.

📧 gali.ajayreddy@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/bala-gali-390725144)
