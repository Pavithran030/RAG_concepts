# RAG (Retrieval-Augmented Generation) Learning Guide

## What is RAG?

RAG combines **retrieval** and **generation** to create AI systems that can answer questions based on specific documents or knowledge bases.

### Simple Analogy
Think of RAG like how you use a library:
- Without RAG: You try to answer questions from memory alone
- With RAG: You search the library, find relevant books, then use that information to answer better

## Core RAG Concept in 4 Steps

```
User Question
     ↓
[1] RETRIEVE → Search documents for relevant info
     ↓
Relevant chunks of text
     ↓
[2] COMBINE → Put question + relevant text together
     ↓
Prompt for AI
     ↓
[3] GENERATE → AI uses all info to answer
     ↓
Better, more accurate answer
```

## Key Components

| Component | Purpose | Example |
|-----------|---------|---------|
| **Documents** | Your knowledge base | PDFs, articles, code docs |
| **Chunks** | Split documents into pieces | Paragraphs, sections |
| **Embeddings** | Convert text to numbers | Vector representation |
| **Vector DB** | Store & search embeddings | Pinecone, Faiss, Chroma |
| **Retriever** | Find relevant chunks | Search by similarity |
| **LLM** | Generate the answer | GPT, Claude, Llama |

## Learning Path

### Phase 1: Foundations (Beginner)
✅ Understand embeddings & similarity search
✅ Learn chunking strategies
✅ Build a simple retriever

### Phase 2: Simple RAG (Intermediate)
✅ Combine retrieval + generation
✅ Use OpenRouter APIs
✅ Create your first RAG system

### Phase 3: Enhancement (Advanced)
✅ Optimize retrieval quality
✅ Add filtering & reranking
✅ Production improvements

## What You'll Build

**Project:** A simple RAG system that answers questions about documents you provide

**By the end:**
- Ask questions in plain English
- System finds relevant information
- AI generates accurate answers using that info
- You'll understand the whole RAG pipeline

---

## Ready? Start with: `01_embeddings_basics.ipynb`
