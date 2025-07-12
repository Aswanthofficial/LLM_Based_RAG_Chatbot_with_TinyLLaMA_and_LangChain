# LLM_Based_RAG_Chatbot_with_TinyLLaMA_and_LangChain

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline using:

- 🧠 **TinyLLaMA** (1.1B) for local question answering
- 🔗 **LangChain** to orchestrate the retrieval + generation workflow
- 🧾 **FAISS** for semantic document retrieval
- 📚 **HuggingFace Sentence Embeddings** to vectorize input text
- 📄 Text file loader and chunking for document ingestion

It enables local, private, and efficient **document-based QA** — ideal for notebooks, reports, or offline AI assistants.

---

## 📌 Key Technologies

| Component          | Tool/Library                            |
|--------------------|-----------------------------------------|
| LLM                | TinyLLaMA (via `llama-cpp-python`)      |
| Embeddings         | HuggingFace (`all-MiniLM-L6-v2`)        |
| Vector Database    | FAISS                                   |
| Retrieval Pipeline | LangChain `RetrievalQA`                 |
| Document Loader    | LangChain `TextLoader`                  |

---

## 🚀 Features

- ✅ Load and split `.txt` files into vectorized chunks
- ✅ Generate embeddings using SentenceTransformers
- ✅ Store and search vectors using FAISS
- ✅ Use a lightweight local LLM (TinyLLaMA) for generation
- ✅ Fully local, offline-compatible RAG pipeline

---

## 🛠️ Installation

Install dependencies:

```bash
pip install -q langchain llama-cpp-python faiss-cpu sentence-transformers
pip install langchain_community
