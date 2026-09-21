# Retrieval Strategy

How relevant chunks actually get found and ranked — beyond a single raw
cosine-similarity search, which is the naive baseline this folder moves
past.

## Why this matters
Similarity search alone often surfaces chunks that are semantically
close but not actually the most useful — a re-ranking or hybrid step
usually closes a meaningful chunk of the quality gap for very little
added complexity.

## Key concepts
- Dense (embedding) vs. sparse (BM25/keyword) retrieval, and hybrid
  search combining both
- Re-ranking retrieved candidates with a cross-encoder
- Metadata filtering (restrict search to the right document type/source
  before ranking)
- Query expansion / rewriting to improve recall on ambiguous queries
- Top-k selection trade-offs (more context vs. more noise/cost)

## Planned contents
- `hybrid_retriever.py`, `reranker.py`, `metadata_filtered_search.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../agentic-rag/`](../agentic-rag/README.md) — where retrieval
  becomes a multi-step, agent-driven decision rather than one fixed call
