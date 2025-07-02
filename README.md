# Langchain RAG Tutorial

# LangChain RAG Tutorial 📚

A simple yet powerful Retrieval-Augmented Generation (RAG) example using LangChain.  
This project lets you ask natural questions about a document and get accurate, grounded answers.

---

## 🧠 What It Does

1. **Ingests a document** (`alice_in_wonderland.md` by default).
2. **Splits** the text into manageable chunks.
3. **Embeds** each chunk into vector form.
4. **Stores** embeddings in a FAISS or Chroma vector DB.
5. **Retrieves** relevant chunks in response to user queries.
6. **Generates** answers using an LLM grounded in the retrieved context.

---

## ⚙️ Project Structure

- `create_database.py`  
  Loads, splits, embeds, and saves document chunks into your vector database.

- `query_data.py`  
  Takes a question, retrieves the top relevant chunks, and calls an LLM to produce a final answer.

- `alice_in_wonderland.md`  
  Example text used to demonstrate the pipeline.

- `requirements.txt`  
  Required packages for running the scripts.

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
pip install -r requirements.txt
pip install "unstructured[md]"
