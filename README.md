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

### 3. London Property Advisor Agent
**Week 3 — Day 2**

A conversational AI property advisor with persistent memory,
specialist persona, and autonomous tool calling.

Features:
- Multi-turn memory — remembers deposit, areas, and context across turns
- Custom system prompt — "Alex" specialist persona with rules
- 5 tools — property search, yield calculation, mortgage, market trends
- Two-agent pipeline — research agent feeds analysis agent
- Autonomous reasoning — 8 tool calls on complex investment questions

Stack: Python · LangGraph · LangChain · Groq LLM

📓 [View Notebook](property_advisor_agent.ipynb)

### 4. Property Research Agent — LangGraph StateGraph
**Week 3 — Day 3**

A stateful AI workflow using LangGraph's StateGraph to research 
property areas, analyse them with an LLM, and conditionally route 
based on confidence — branching to a mortgage calculation step 
only when confidence is high, otherwise ending early.

Features:
- Typed state (TypedDict) flowing through 4 nodes
- Conditional edges — real branching logic, not a fixed pipeline
- Debugged a real state-tracking bug where a node's intended 
  next step diverged from what actually executed
- Graph visualised via Mermaid

Stack: Python · LangGraph · Groq LLM

📓 [View Notebook](property_langgraph_workflow.ipynb)

### 5. Autonomous Property Research Agent — Week 3 Capstone
**Week 3 — Days 5-7**

A fully autonomous property investment research agent combining 
LangGraph StateGraph, multi-tool ReAct agents, and live web search 
into one coherent system.

Features:
- Multi-tool ReAct agent running **inside** a LangGraph node — 
  agents within graphs, not just standalone agents
- Live web search (Tavily) combined with local property database
- Conditional routing based on LLM confidence assessment
- Diagnosed and fixed two Groq-specific tool-calling bugs 
  (type schema mismatch + LLM pre-computing arguments it 
  should have passed raw)

Stack: Python · LangGraph · LangChain · Groq LLM · Tavily Search

[View Notebook](property_agent_capstone.ipynb)

### 6. Property Research API — FastAPI Cloud Deployment
**Week 4 — Day 1**

A production-ready REST API wrapping the property investment 
research logic built across Weeks 1-3, deployed to the cloud 
with a public URL.

Endpoints:
- `GET /property/{area}` — property data by London area
- `POST /mortgage` — mortgage payment calculator
- `POST /compare` — yield comparison across multiple areas
- `GET /areas` — list all available areas
- `GET /docs` — interactive Swagger documentation

Features:
- Pydantic request/response validation
- Proper HTTP error handling (404, 400, 422)
- Auto-generated OpenAPI documentation
- Deployed on Render via GitHub integration

Stack: Python · FastAPI · Pydantic · Uvicorn · Render

🌐 [Live API](https://property-api-rpdk.onrender.com/docs) · 
📦 [GitHub Repo](https://github.com/gali-ai-engineer/property-api)

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
- ✅ Week 2 — Prompt engineering, LangChain, RAG, FastAPI
- ✅ Week 3 — Agents, tool calling, LangGraph (complete)
- 🔄 Week 4 — Capstone, FastAPI deployment, Azure AI, AI-102 cert prep

## Background
7+ years as .NET and Cloud Developer across UK, Thailand, and India.
Currently building toward Generative AI Engineer role in UK market — Q3 2026.

📧 gali.ajayreddy@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/bala-gali-390725144)
