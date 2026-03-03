## 📄 Overview

A fully offline **Retrieval-Augmented Generation (RAG)** system that enables conversational question-answering over uploaded PDF documents using a locally hosted LLM.

Built for privacy-focused environments where cloud APIs are not allowed.

---

## 🚀 Key Features

- 💬 Conversational QA over PDF documents  
- 📚 PDF text extraction using **PyPDF**  
- 🔎 Semantic search using **Sentence Transformers**  
- 🧠 Persistent vector storage via **ChromaDB**  
- 🤖 Local LLM inference using **LM Studio**  
- 🔐 Fully offline — no external API calls  
- ⚡ Fast embedding generation powered by **PyTorch**  

---

## 🔄 Processing Pipeline

1. Extract text from PDF  
2. Split into semantic chunks  
3. Generate embeddings  
4. Store embeddings in ChromaDB  
5. Retrieve top-k relevant chunks  
6. Construct prompt  
7. Generate answer via local LLM  

---

## 🧠 Architecture Flow

```
PDF → Text Extraction → Chunking → Embeddings → ChromaDB
          ↑                                  ↓
        User Query ← Semantic Retrieval ← Prompt → LLM Response
```

