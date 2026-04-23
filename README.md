# RAG (Retrieval-Augmented Generation) Learning Package

A beginner-friendly set of guides and notebooks to learn RAG from core concepts to a working prototype and simple production patterns.

## Quick start

Choose one path:

### Fastest (5 minutes)
1. Read `RAG_LEARNING_GUIDE.md`.

### Standard (30 minutes)
1. Read `RAG_LEARNING_GUIDE.md`.
2. Read `GETTING_STARTED.md`.
3. Run `01_beginner_rag_from_scratch.ipynb` (first 3 cells).

### Full (2–3 hours)
1. Follow `GETTING_STARTED.md`.
2. Complete tutorials 1–3.
3. Experiment with your own data.

## What's included

### Guides
- `START_HERE.md` — navigation
- `RAG_LEARNING_GUIDE.md` — core concepts
- `GETTING_STARTED.md` — setup and step-by-step
- `LEARNING_ROADMAP.md` — suggested learning path
- `RAG_QUICK_REFERENCE.md` — definitions and quick lookup

### Tutorials
- `01_beginner_rag_from_scratch.ipynb` — foundation RAG
- `02_rag_with_real_embeddings.ipynb` — semantic embeddings
- `03_rag_with_llm_integration.ipynb` — LLM integration

## Installation

```bash
# Core
pip install numpy scikit-learn

# Tutorial 2
pip install sentence-transformers

# Tutorial 3
pip install requests
```

## Notes
- Tutorials 1–2 run on CPU and are free to run.
- Tutorial 3 uses an external LLM API (see `GETTING_STARTED.md` for setup).

## Resources
- Sentence Transformers: https://www.sbert.net/
- OpenRouter docs: https://openrouter.ai/docs
- LangChain: https://python.langchain.com/
