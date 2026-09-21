# Chunking Strategy

How source documents get split into retrievable pieces — the
highest-leverage, most under-discussed decision in a RAG pipeline. Bad
chunking silently caps retrieval quality no matter how good the
embedding model or LLM is.

## Why this matters
Fixed-size character chunking is the easy default and the wrong choice
for structured documents (runbooks, API docs, markdown with headers) —
it can split a numbered step or a code block right at the point that
matters most for retrieval.

## Key concepts
- Fixed-size vs. semantic vs. structure-aware chunking (splitting on
  headers/sections)
- Chunk size and overlap trade-offs
- Recursive character splitting vs. sentence-boundary splitting
- Metadata-preserving chunking (tracking source section for citation)
- Chunking's direct downstream effect on retrieval recall — measurable
  via [`../ragas-llm-judge/`](../ragas-llm-judge/README.md)

## Planned contents
- `fixed_size_chunker.py`, `semantic_chunker.py`, `markdown_aware_chunker.py`
- `chunking_eval.py` — recall@k comparison across strategies
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
