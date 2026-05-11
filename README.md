RAG PDF Analysis System
=======================
An AI-powered Retrieval-Augmented Generation (RAG) application that allows users to upload PDF documents, create embeddings, store them in a persistent vector database, and interact with the documents conversationally using OpenAI LLMs.

Project Overview
=======================
This project demonstrates how Large Language Models (LLMs), embeddings, and vector databases can be combined to build an intelligent document question-answering system.

The application:

Uploads PDF documents,
Extracts text from PDFs,
Splits content into chunks,
Generates embeddings using OpenAI,
Stores embeddings in a persistent ChromaDB vector database,
Retrieves semantically relevant chunks,
Uses OpenAI LLMs to answer user questions based on document context



Architecture
PDF Upload
    ↓
Text Extraction
    ↓
Chunking
    ↓
Embeddings Generation
    ↓
ChromaDB Vector Store (Persistent)
    ↓
User Query
    ↓
Semantic Similarity Search
    ↓
Relevant Chunks Retrieved
    ↓
OpenAI LLM Generates Final Answer

Features

PDF document ingestion,
Persistent vector database,
Semantic similarity search,
Conversational querying,
Multi-document support,
OpenAI embeddings integration,
ChromaDB vector storage,
LangChain integration,
Jupyter Notebook experimentation



Tech Stack

Programming Language: 
-----------------------
Python 3.12


Libraries & Frameworks: 
-----------------------
LangChain,
LangChain OpenAI,
ChromaDB,
PyPDFLoader,
OpenAI API,
Python-dotenv

Vector Database: 
-----------------------
ChromaDB


LLM & Embeddings :
-----------------------
GPT-4.1-mini,
text-embedding-3-small



Folder Structure
-----------------------
RAG_mini_project/
│
├── .venv/
├── .vscode/
├── Docs/
├── Vector/
├── notebooks/
│
├── .gitignore
├── pyproject.toml
├── README.md
└── uv.lock


Installation for the User
================================
Clone Repository
git clone <your-repo-url>cd RAG_mini_project

Create Virtual Environment
Using uv:
uv venv

Activate environment:
Windows
.venv\Scripts\activate

Install Dependencies
uv sync
OR
uv pip install -r requirements.txt

Environment Variables
Create a .env file:
OPENAI_API_KEY=your_openai_api_key

Run The Project
Open Jupyter Notebook:
jupyter notebook
Run:
RAG_PDF_Analysis_System.ipynb
RAG_PDF_Analysis_System_Part2.ipynb



How It Works
=============
Step 1 — Upload PDF
The system loads PDF documents using LangChain PDF loaders.
Step 2 — Text Extraction
Text content is extracted from the uploaded PDF.
Step 3 — Chunking
Large text is split into smaller chunks using RecursiveCharacterTextSplitter.
Step 4 — Embedding Generation
OpenAI embedding models convert text chunks into vector embeddings.
Step 5 — Vector Storage
Embeddings are stored inside ChromaDB for persistent semantic retrieval.
Step 6 — Query Processing
User queries are converted into embeddings.
Step 7 — Similarity Search
Relevant chunks are retrieved using semantic similarity search.
Step 8 — LLM Response Generation
Retrieved context is passed to the OpenAI LLM to generate accurate answers.

Sample Use Cases
----------------------
Research assistant,
Enterprise knowledge base,
Document Q&A system,
Legal document search,
Educational content assistant,
AI-powered PDF chatbot




This project demonstrates practical understanding of:

Retrieval-Augmented Generation (RAG)
Embeddings,
Vector Databases,
Semantic Search,
Chunking Strategies,
LLM Prompting,
Persistent Storage,
AI Pipeline Design,
OpenAI API Integration,
LangChain Orchestration



Future Enhancements

OCR support for scanned PDFs,
Multi-user support,
FastAPI backend,
Streamlit UI,
Metadata filtering,
Hybrid search,
Conversation memory,
Source citation,
Document summarization.


# Acknowledgement

Thank you for carefully going through this project.

This project was built as part of my learning journey in AI Engineering, Retrieval-Augmented Generation (RAG), Vector Databases, and OpenAI-based applications.

I continuously work on improving scalable AI + Data Engineering solutions and exploring modern LLM-powered architectures.

Feedback and suggestions are always welcome 🚀


Author
Rachit Nagda
AI + Data Engineering Enthusiast