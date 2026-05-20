# IntelliRAG — Production-Grade Hybrid RAG Pipeline

[![Live Demo](https://img.shields.io/badge/Live_Demo-Click_Here-brightgreen?style=for-the-badge)](https://sulaxmi22.github.io/projects/intellirag/frontend/index.html)
[![Portfolio](https://img.shields.io/badge/Portfolio-sulaxmi22.github.io-blue?style=for-the-badge)](https://sulaxmi22.github.io)

## VIEW LIVE DEMO
**https://sulaxmi22.github.io/projects/intellirag/frontend/index.html**

> Hybrid RAG pipeline achieving 91% context precision via BM25 + dense vector search + cross-encoder reranking

---

## Problem Statement

Most RAG implementations are toy demos. In enterprise settings, you need hybrid search, reranking, evaluation metrics, and citation enforcement. IntelliRAG demonstrates production-grade patterns used at companies like AT&T, Google, and OpenAI.

## Key Features

| Feature | Description |
|---------|-------------|
| Hybrid Search | BM25 keyword + dense vector similarity with Reciprocal Rank Fusion |
| Cross-Encoder Reranking | Re-scores retrieved chunks for higher precision |
| Corrective RAG | Self-evaluates retrieval quality, falls back to web search if poor |
| Streaming Responses | Server-Sent Events for real-time token streaming |
| Source Citations | Every answer maps to specific document chunks |
| RAGAS Evaluation | Automated faithfulness, answer relevancy, context precision metrics |

## Evaluation Results

| Metric | Score |
|--------|-------|
| Context Precision | 91% |
| Faithfulness | 92% |
| Answer Relevancy | 89% |

## Quick Start

git clone https://github.com/sulaxmiraskar/intellirag.git
cd intellirag
pip install -r requirements.txt
cp .env.example .env
python -m uvicorn backend.main:app --reload --port 8000

## Tech Stack

Python, FastAPI, LangChain, FAISS, ChromaDB, BM25, OpenAI, RAGAS

## Built by Sulaxmi Raskar
Senior Full-Stack AI Engineer - RAG pipelines, LangChain, FastAPI, Python

Portfolio: https://sulaxmi22.github.io
Live Demo: https://sulaxmi22.github.io/projects/intellirag/frontend/index.html
