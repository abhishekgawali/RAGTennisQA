# 🎾 RAGTennisQA

A lightweight Retrieval-Augmented Generation (RAG) system that answers questions from a tennis knowledge base using semantic search and LLM-based generation.

---

## 🚀 Overview

This project implements an end-to-end RAG pipeline to enable **context-aware question answering** over structured markdown documents.

The entire pipeline is implemented in a Jupyter Notebook for easy experimentation and demonstration.

It combines:

- Vector search (**ChromaDB**)
- Semantic embeddings (**Sentence Transformers**)
- LLM-based generation (**Qwen**)

---

## 🧠 How It Works

1. Load a markdown document (tennis dataset)
2. Split content using markdown headers
3. Generate embeddings using `all-MiniLM-L6-v2`
4. Store embeddings in **ChromaDB**
5. Retrieve relevant context for a query
6. Pass context to the LLM (Qwen)
7. Generate a context-aware answer

---

## 🛠 Tech Stack

- Python
- LangChain
- ChromaDB
- Sentence Transformers
- Hugging Face Transformers
- Qwen2.5-1.5B-Instruct

---

## 📂 Project Structure

```text
RAGTennisQA/
├── requirements.txt
├── README.md
├── .gitignore
├── data/
│   └── tennis_details.md
└── notebooks/
    └── rag_pipeline_demo.ipynb   <-- main implementation