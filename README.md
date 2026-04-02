# RAGTennisQA
A lightweight Retrieval-Augmented Generation (RAG) system that
 answers questions from a tennis knowledge base using 
semantic search and LLM-based generation.
# Overview

This project implements an end-to-end RAG pipeline to enable context-aware question answering over structured markdown documents.

It demonstrates how to combine:

vector search (ChromaDB)
semantic embeddings (Sentence Transformers)
LLM generation (Qwen)

to build a simple but effective document-based QA system.

# How It Works
Load a markdown document (tennis dataset)
Split content using markdown headers
Generate embeddings using all-MiniLM-L6-v2
Store embeddings in ChromaDB
Retrieve the most relevant chunk for a query
Pass retrieved context to an LLM (Qwen)
Generate a context-aware answer

# Tech Stack
Python
LangChain
ChromaDB (Vector Database)
Sentence Transformers
Hugging Face Transformers
Qwen2.5-1.5B-Instruct

# RAGTennisQA/

│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── data/
│   └── tennis_details.md
│
└── notebooks/
    └── rag_pipeline_demo.ipynb
	
	
# installatins

git clone https://github.com/abhishekgawali/RAGTennisQA.git
cd RAGTennisQA
pip install -r requirements.txt