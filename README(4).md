# 🚀 Advanced Hybrid RAG System with FAISS, BM25, Cross-Encoder Re-Ranking, FLAN-T5, Whisper & Voice Assistant

## 📌 Project Overview
This project implements an **end-to-end Advanced Retrieval-Augmented Generation (RAG)** system for question answering over PDF documents. It combines **semantic search**, **keyword search**, **hybrid retrieval**, **cross-encoder re-ranking**, **LLM-based answer generation**, **answer verification**, **conversation memory**, **PDF evidence highlighting**, and **voice-based interaction**.

The system allows users to upload one or more PDF documents, ask questions in text or voice, retrieve the most relevant passages, generate grounded answers with citations, verify answer quality, and interact through a conversational interface.

---

# 🎯 Objectives

- Build a production-style Hybrid RAG pipeline.
- Retrieve accurate information from PDF documents.
- Combine semantic and keyword retrieval.
- Improve retrieval quality using Cross-Encoder re-ranking.
- Generate grounded answers using FLAN-T5.
- Verify generated answers automatically.
- Support conversational memory.
- Enable speech-to-text and text-to-speech interaction.
- Visualize evidence directly inside PDF pages.

---

# 🛠 Technologies Used

- Python
- LangChain
- FAISS
- Sentence Transformers
- Hugging Face Transformers
- FLAN-T5
- Cross-Encoder (MS MARCO MiniLM)
- BM25 (rank_bm25)
- PyPDF
- PyMuPDF (fitz)
- Librosa (if extended)
- Whisper
- gTTS
- Google Colab
- NumPy
- Matplotlib

---

# 📂 Complete Workflow

1. Upload PDF documents
2. Extract text from PDFs
3. Clean extracted text
4. Create LangChain documents
5. Chunk documents
6. Generate sentence embeddings
7. Build FAISS vector index
8. Create BM25 keyword index
9. Route queries (keyword / semantic / hybrid / summary)
10. Retrieve relevant chunks
11. Cross-Encoder re-ranking
12. Build contextual prompt
13. Generate answer using FLAN-T5
14. Verify generated answer
15. Display citations
16. Highlight evidence inside PDF
17. Maintain conversation memory
18. Dashboard reporting
19. Voice input using Whisper
20. Text-to-Speech using gTTS
21. Interactive chatbot

---

# 🧠 Concepts Covered

## Document Processing
- PDF Parsing
- Multi-PDF Support
- Text Cleaning
- Metadata Extraction
- LangChain Document Objects

## Text Chunking
- Recursive Character Text Splitter
- Chunk Size
- Chunk Overlap

## Embedding Models
- Sentence Transformers
- all-MiniLM-L6-v2
- Dense Vector Embeddings

## Vector Database
- FAISS
- Similarity Search
- Vector Indexing

## Keyword Retrieval
- BM25
- Tokenization
- Lexical Search

## Hybrid Retrieval
- Semantic Retrieval
- Keyword Retrieval
- Query Routing
- Hybrid Search Strategy

## Re-Ranking
- Cross-Encoder
- MS MARCO MiniLM
- Relevance Scoring
- Top-K Ranking

## Large Language Models
- FLAN-T5 Base
- Prompt Engineering
- Context-Augmented Generation
- Answer Generation

## Answer Verification
- LLM-based Verification
- Confidence Estimation
- Hallucination Reduction

## Conversational AI
- Chat Memory
- Multi-turn Conversations
- Context Retention

## Explainability
- Source Citations
- PDF Evidence Highlighting
- Retrieval Dashboard

## Voice AI
- Automatic Speech Recognition (Whisper)
- Speech-to-Text
- Text-to-Speech (gTTS)
- Voice Chat Interface

## Deployment Concepts
- Google Colab
- Interactive Chatbot
- Real-Time Question Answering

---

# 🤖 Models Used

## Embedding Model
- sentence-transformers/all-MiniLM-L6-v2

## Re-Ranker
- cross-encoder/ms-marco-MiniLM-L-6-v2

## Large Language Model
- google/flan-t5-base

## Speech Recognition
- openai/whisper-small

---

# ✨ Key Features

- Hybrid Retrieval (FAISS + BM25)
- Intelligent Query Routing
- Cross-Encoder Re-Ranking
- FLAN-T5 Answer Generation
- LLM Answer Verification
- Chat Memory
- PDF Evidence Highlighting
- Source Citations
- Voice Assistant
- Speech-to-Text
- Text-to-Speech
- Multi-PDF Support
- Interactive Dashboard

---

# 📁 Repository Structure

```text
├── transfomersp_ (1).ipynb
├── README.md
├── requirements.txt
└── documents/
```

---

# ▶️ Installation

```bash
git clone <repository-url>
cd <repository-name>
pip install -r requirements.txt
```

---

# ▶️ Run

```bash
jupyter notebook "transfomersp_ (1).ipynb"
```

Or run in Google Colab.

---

# 📈 Expected Outcome

The system retrieves the most relevant document chunks using hybrid retrieval, improves ranking with a Cross-Encoder, generates grounded answers with FLAN-T5, verifies answer quality, highlights supporting evidence in PDFs, and supports both text and voice conversations.

---

# 🔮 Future Improvements

- RAG evaluation using RAGAS
- LangSmith tracing
- LangFuse observability
- ChromaDB, Pinecone, or Weaviate integration
- Streaming responses
- FastAPI deployment
- Docker & Kubernetes
- Authentication and user management
- Multi-modal RAG
- Agentic RAG with LangGraph
