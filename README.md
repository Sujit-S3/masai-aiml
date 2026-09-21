# MASAI AI/ML — Capstone Projects

This repository contains my capstone project work, which I completed as part of the **Certificate Program in Artificial Intelligence and Machine Learning** at MASAI. I put a lot of effort into ensuring this project not only meets the requirements but also showcases my ability to build end-to-end data and AI solutions from scratch.

## Projects

### [zepto-data-ai-platform](./zepto-data-ai-platform)

I decided to build a full-stack AI/ML platform centered around a Zepto-themed use case. I broke the project down into three connected modules, which allowed me to demonstrate my skills across the entire ML lifecycle:

| Module | Description | Marks |
|--------|-------------|-------|
| **data_pipeline** | For this module, I wrote a web scraper using `requests` and `BeautifulSoup`. I focused heavily on data cleaning and normalization before storing the data in a SQLite database. Finally, I crafted several SQL queries and verified them using `pandas` to ensure data integrity. | 25 |
| **analytics** | Here, I performed an extensive Exploratory Data Analysis (EDA) on the Titanic dataset. I trained and evaluated three classification models (Logistic Regression, Decision Tree, Random Forest). To tackle class imbalance, I implemented SMOTE. I also spent time tuning hyperparameters to squeeze out the best performance, and finished with a regression analysis. | 50 |
| **support_assistant** | I built a RAG-based support chatbot to demonstrate my GenAI skills. I used `sentence-transformers` for creating embeddings, which I then stored in a local `ChromaDB` vector store. For the agent's logic, I designed a state machine using `LangGraph`, and I wrapped the whole thing in a `FastAPI` REST API so it could be queried externally. | 25 |

**Technologies I Used:** Python, pandas, scikit-learn, sentence-transformers, ChromaDB, LangGraph, FastAPI, SQLite, BeautifulSoup, Jupyter.

→ See my detailed [project README](./zepto-data-ai-platform/README.md) for full setup instructions and an in-depth breakdown of my design decisions.

## Structure

```
MASAI-AIML/
└── zepto-data-ai-platform/   ← My capstone project (included as a submodule)
    ├── data_pipeline/         Module 1 — My pipeline for scraping, cleaning, and querying via SQL
    ├── analytics/             Module 2 — My notebooks for EDA, modeling, and evaluation
    └── support_assistant/     Module 3 — My RAG pipeline (ingest, embed, retrieve, and API)
```

## Setup Instructions

If you'd like to run my code on your machine, here are the steps I use to set it up:

```bash
git clone --recurse-submodules https://github.com/Sujit-S3/masai-aiml.git
cd masai-aiml/zepto-data-ai-platform

# I recommend using a virtual environment to avoid dependency conflicts:
python -m venv .venv
source .venv/Scripts/activate   # (For Windows)
# If you are on Linux/Mac, use: source .venv/bin/activate

# Install all the packages I used for this project:
python -m pip install -r requirements.txt
```
