# Local PDF Chat Application (Offline RAG)

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
2. Split text into semantic chunks  
3. Generate embeddings  
4. Store embeddings in ChromaDB  
5. Retrieve top-k relevant chunks  
6. Construct context-aware prompt  
7. Generate final answer using local LLM  

---

## 🧠 Architecture Flow

![Architecture Flow](images/mermaid-diagram.png)

> Make sure `mermaid-diagram.png` is inside an `images/` folder in your repository.

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/DarshanKamate1254/local-pdf-rag.git
cd local-pdf-rag
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install chromadb pypdf sentence-transformers torch requests streamlit
```

---

## 🖥️ Setup Local LLM (LM Studio)

1. Install **LM Studio**  
2. Download a supported model (e.g., Mistral, LLaMA, Phi)  
3. Start the local server  
4. Default API endpoint:

```
http://localhost:1234/v1/chat/completions
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

Upload your PDF and start chatting with your document.

---

## 📸 Demo

<p align="center">
  <img src="Screenshot 2026-03-03 181904.png">
</p>

> Ensure your screenshot is placed inside the `images/` folder and named `demo.png`.

---

## 🔐 Privacy & Security

- No cloud API calls  
- No data leaves your machine  
- Fully offline processing  
- Ideal for sensitive or enterprise environments  

---

## 🚀 Future Improvements

- Hybrid Search (BM25 + Vector similarity)  
- Multi-document collections  
- Metadata filtering  
- Streaming responses  
- FastAPI backend integration  
- Dockerized deployment  

---

## 📜 License

MIT License

