# 🧠 Conversational RAG with PDF Uploads and Chat History

This project is a **Conversational Retrieval-Augmented Generation (RAG) app** built with **Streamlit**. It lets users upload one or more PDF documents and then chat with the contents in a context-aware, multi-turn dialogue.

Powered by:
- 📄 PDF ingestion with LangChain loaders
- 🔍 Chunking + Embeddings using HuggingFace + ChromaDB
- 🤖 LLM via Groq's blazing-fast Gemma-2B model
- 🧠 Memory-augmented prompts to keep track of conversation history

---

## 🚀 Features

- 📚 Upload one or more PDF files
- 🧩 Splits documents into chunks using `RecursiveCharacterTextSplitter`
- 🧠 Embeds chunks using `all-MiniLM-L6-v2` from HuggingFace
- 💾 Stores embeddings in a local Chroma vector store
- 🔄 Reformulates follow-up questions using chat history
- 🤖 Answers questions using retrieved context and LLM (Gemma 2B via Groq API)
- 💬 Maintains chat history per session
- 🔐 Supports secure Groq API key input in the frontend

---

## 📦 Tech Stack

| Tool        | Purpose                            |
|-------------|------------------------------------|
| Streamlit   | UI for chat + file upload          |
| LangChain   | Orchestration + memory management  |
| ChromaDB    | Local vector store for retrieval   |
| HuggingFace | Embeddings model (`MiniLM`)        |
| Groq        | LLM backend (Gemma-2B-IT)           |
| PyPDFLoader | PDF parsing                        |

---