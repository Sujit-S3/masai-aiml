# MASAI AI/ML — Capstone Projects

This repository contains my capstone project work completed as part of the **Certificate Program in Artificial Intelligence and Machine Learning** at MASAI.

## Projects

### [zepto-data-ai-platform](./zepto-data-ai-platform)

A full-stack AI/ML platform built around a Zepto-themed use case, covering three end-to-end modules:

| Module | Description | Marks |
|--------|-------------|-------|
| **data_pipeline** | Web scraping with `requests` + `BeautifulSoup`, data cleaning, SQLite storage, and SQL + pandas queries | 25 |
| **analytics** | Titanic dataset EDA, classification (Logistic Regression, Decision Tree, Random Forest), imbalance handling (SMOTE), hyperparameter tuning, regression | 50 |
| **support_assistant** | RAG-based support chatbot — sentence-transformers embeddings, ChromaDB vector store, LangGraph state machine, FastAPI REST API | 25 |

**Tech used:** Python, pandas, scikit-learn, sentence-transformers, ChromaDB, LangGraph, FastAPI, SQLite, BeautifulSoup, Jupyter

→ See the [project README](./zepto-data-ai-platform/README.md) for full setup and run instructions.

## Structure

```
MASAI-AIML/
└── zepto-data-ai-platform/   ← Capstone project (submodule)
    ├── data_pipeline/         Module 1 — scrape → clean → SQLite → SQL queries
    ├── analytics/             Module 2 — EDA → modeling → evaluation → joblib
    └── support_assistant/     Module 3 — ingest → embed → retrieve → FastAPI
```

## Setup

Clone with submodules:

```bash
git clone --recurse-submodules https://github.com/Sujit-S3/masai-aiml.git
cd masai-aiml/zepto-data-ai-platform
python -m venv .venv
source .venv/Scripts/activate   # Windows
python -m pip install -r requirements.txt
```
