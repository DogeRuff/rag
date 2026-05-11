# RAG Pipeline with ChromaDB and Ollama

A Retrieval Augmented Generation pipeline built over academic papers using local embeddings and a local LLM, with no API keys required.

---

## Overview

This project implements a fully local RAG pipeline that:
- Loads and chunks academic PDF papers
- Generates embeddings locally with HuggingFace
- Stores vectors in ChromaDB
- Retrieves relevant chunks via cosine similarity
- Generates answers using Mistral 7B via Ollama

---

## Papers used as knowledge base
- LoRA: Low-Rank Adaptation of Large Language Models
- QLoRA: Efficient Finetuning of Quantized LLMs
- Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
- DARE-TIES: Model Merging

---

## Requirements
- Python 3.12
- Miniconda
- Ollama with Mistral installed

```bash
ollama pull mistral
```

---

## Installation

```bash
conda create -n rag-project python=3.12 -y
conda activate rag-project
pip install langchain langchain-community langchain-huggingface langchain-ollama langchain-text-splitters chromadb pypdf sentence-transformers ollama ipykernel
```

---

## Usage
Add your PDF files to the `data/` folder and run the notebook `rag_chromadb_pipeline.ipynb` cell by cell.

---

## Author
Alonso Guevara Perez — Systems Engineer