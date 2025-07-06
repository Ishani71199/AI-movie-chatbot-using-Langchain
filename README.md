# 🎬 AI-movie-chatbot-using-Langchain

This repo contains a movie-based conversational AI system using Langchain as framework.

## 🚀 Project Overview

This project builds a **natural language question-answering system** over an IMDb movie dataset using vector similarity search and memory-augmented LLM chains. It demonstrates modern RAG (Retrieval-Augmented Generation) techniques with open-source tools.

## 📌 Features

- ✅ IMDb Movie Data Ingestion
- ✅ Text Embedding via **text-embedding-3-large**
- ✅ Vector storage and similarity search using **Qdrant** 
- ✅ Retrieval-Augmented QA using **LangChain**
- ✅ Conversational Memory Support

## 🧰 Tech Stack

| Tool        | Description                              |
|-------------|------------------------------------------|
| 🧠 Hugging Face Transformers | For text embeddings |
| 📦 Qdrant    | Vector DB with HNSW indexing            |
| 🧩 LangChain | For chaining LLM with retriever and memory |
| 🐍 Python    | Core implementation (Jupyter Notebook)  |

## 📂 Dataset

-  Dataset Link [https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows]
- **IMDb Dataset**: Contains information such as movie titles, genres, overview, directors, ratings, and more.
-  Loaded and preprocessed from CSV into vector embeddings for similarity search.

## 🧪 How It Works

1. **Data Preprocessing**: Clean and extract metadata from IMDb dataset.
2. **Vector Embedding**: Generate sentence embeddings for movie summaries.
3. **Indexing in Qdrant**: Store vectors using HNSW-based similarity index.
4. **Query Pipeline**:
    - User asks a natural language question.
    - The retriever fetches the top `k` similar movie records.
    - LangChain LLM generates a response based on context.
    - Past chat is retained using memory.

## 🛠️ Installation

pip install -r requirements.txt
