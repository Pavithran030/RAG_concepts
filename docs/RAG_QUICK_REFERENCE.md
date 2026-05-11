# RAG Quick Reference Guide

## RAG in One Picture

```
Document Upload/Loading
        ↓
Chunking (split into pieces)
        ↓
Embedding (convert to vectors)
        ↓
Vector Store (index & store)
        ↓
        ←→ USER ASKS QUESTION
        ↓
Retrieval (find relevant chunks)
        ↓
Prompt Augmentation (add context to query)
        ↓
LLM Generation (get answer from model)
        ↓
Return Answer
```

## Core Concepts Explained Simply

### 1. **Embeddings**
- Converts text into numbers (vectors)
- Similar meaning = similar vectors
- Used for finding relevant documents
- Example: "cat" and "dog" are closer together than "cat" and "algorithm"

### 2. **Chunking**
- Splitting long documents into smaller pieces
- Better retrieval accuracy
- Typical sizes: 256-512 tokens per chunk

### 3. **Vector Similarity**
- Measures how similar two texts are (0 to 1)
- Cosine similarity: most common metric
- Used to rank search results

### 4. **Retrieval**
- Finding the most relevant chunks for a query
- Uses vector similarity
- Returns top-k results

### 5. **Augmentation**
- Adding retrieved documents to the original prompt
- Gives LLM context to generate better answers

### 6. **Generation**
- LLM reads: question + context
- Generates accurate answer
- Result depends on context quality

## Common RAG Architectures

### Simple RAG (Best for Learning)
```
Query → Retriever → Top-k docs → LLM → Answer
```

### Multi-step RAG (More Complex)
```
Query → Query Expansion → Multi-retriever → Reranker → LLM → Answer
```

### Hybrid RAG (Most Powerful)
```
Query → BM25 + Vector Search → Fusion → Reranker → LLM → Answer
```

## Evaluation Metrics

| Metric | What it measures | Range |
|--------|-----------------|-------|
| **Retrieval Precision** | How many retrieved docs are relevant | 0-1 |
| **Retrieval Recall** | How many relevant docs were retrieved | 0-1 |
| **Answer Quality** | How good is the final answer | Subjective |
| **Latency** | How fast is the system | Milliseconds |

## Common Mistakes to Avoid

❌ Chunks too long → Irrelevant information included
❌ Chunks too short → Missing context
❌ Poor embeddings → Wrong documents retrieved
❌ No query preprocessing → Noisy searches
❌ Ignoring retrieved document quality → Bad answers

## Resources for Next Steps

**Free/Open-source:**
- LangChain: RAG framework
- LlamaIndex: Data indexing
- HuggingFace: Models & embeddings
- FAISS: Vector search
- Chroma: Vector database

**Paid APIs:**
- OpenAI: GPT-4 + embeddings
- Anthropic: Claude API
- Cohere: Embeddings API
- OpenRouter: Multi-model API

## When to Use RAG?

✅ **Good use cases:**
- Q&A over company documents
- Customer support
- Knowledge base search
- Research assistance
- Code documentation

❌ **Not ideal for:**
- Real-time streaming
- Private data (careful with API calls)
- Knowledge requiring reasoning across 10+ documents
