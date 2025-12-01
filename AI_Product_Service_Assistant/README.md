# AI-Powered Customer Support Assistant (n8n + RAG)

## Overview
This project is an **AI-powered customer support assistant** designed to intelligently answer customer inquiries about **Pickering Laboratories’ instruments, reagents, consumables, and services** using real product data from the company’s catalog.

The assistant delivers a conversational experience similar to chatting with a **knowledgeable support specialist**—available anytime, anywhere—while ensuring all responses are grounded in verified documentation through **Retrieval-Augmented Generation (RAG)**.

---

## 🔧 End-to-End System Architecture

### 1️⃣ Knowledge Base & Vector Embedding Pipeline
- 📥 Automatic catalog download from **Google Drive**
- 📄 Document loading and text extraction
- 🧩 Text chunking and preprocessing
- 🧠 Embedding using **Cohere (embed-english-v3.0)**
- 🗃️ Storage in **Supabase Vector Database** for fast semantic search  

This pipeline creates a **continuously updated, AI-searchable knowledge base**.

---

### 2️⃣ Retrieval-Augmented Generation (RAG) Engine
- 🧠 **Cohere Chat Model** for natural language understanding
- 🔎 **Supabase Vector Search** for relevant document retrieval
- 💬 **PostgreSQL Chat Memory** for multi-turn conversations
- 🤖 **n8n AI Agent** to orchestrate workflow logic and tools  

The assistant retrieves the most relevant product content and generates **accurate, context-aware responses**.

---

### 3️⃣ Frontend Chat Interface (Lovable)
A modern, responsive customer-facing interface built with **Lovable**, featuring:
- Clean, branded UI
- Real-time conversational experience
- Secure API integration
- Fully deployable on the web or embeddable into any product site  

**Example User Query:**
> “Tell me about the UVE Photochemical Reactor.”

The assistant instantly returns **verified product information** from the knowledge base.

---

## 💼 Business Impact
This solution demonstrates how AI-driven automation can:

- ✔ Enhance customer support with instant responses  
- ✔ Improve answer accuracy using RAG (no hallucinations)  
- ✔ Scale product knowledge automatically with new document uploads  
- ✔ Boost product discovery and sales  
- ✔ Reduce repetitive support workload  
- ✔ Provide 24/7 global customer assistance  

---

## 🌟 Motivation
This project was built to demonstrate how **AI, automation, and structured product data** can be combined to solve real-world challenges in:

- Customer Service  
- Product Discovery  
- Technical Support  
- Knowledge Automation  

---

## 🛠️ Built With
- **n8n** – Workflow orchestration & AI agent logic  
- **Cohere** – Embeddings & chat model  
- **Supabase** – Vector store & chat memory  
- **Lovable** – Frontend chat interface  

Inspired by real-world use cases from **Pickering Laboratories**.

---

## ⚙️ How to Use
1. Import the provided n8n workflow `.json` file into your n8n instance.
2. Configure credentials for:
   - Google Drive  
   - Cohere  
   - Supabase  
3. Deploy the frontend via Lovable.
4. Activate the workflow.

---

## ⚠️ Disclaimer
This project is a **demonstration system for portfolio and educational purposes** and is not an official production deployment for Pickering Laboratories.

---

## 👤 Author
**Kennedy**
