# RAG Pipeline (Baseline)

The end-to-end retrieval-augmented generation pipeline: ingest documents
→ chunk → embed → store → retrieve → augment the LLM prompt → generate.
This folder is the baseline, single-hop version that every other RAG
topic in this repo builds on or complicates.

## Why this matters
Before agentic RAG, multimodal RAG, or re-ranking make sense, the basic
pipeline needs to actually work end-to-end and be measurable. This is
where that reference implementation lives.

## Key concepts
- The five-stage pipeline: ingest → chunk → embed → retrieve → generate
- Grounding — making sure the LLM's answer is actually supported by
  retrieved context, not just plausible-sounding
- Where each other RAG topic in this repo plugs in: chunking-strategy
  (stage 2), retrieval-strategy (stage 4), ragas-llm-judge (measuring
  the whole thing)

## Planned contents
- `ingest.py`, `embed.py`, `vector_store.py`, `retriever.py`, `generate.py`
- `end_to_end_demo.py` — runs the full pipeline on a small sample doc set
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../chunking-strategy/`](../chunking-strategy/README.md)
- [`../retrieval-strategy/`](../retrieval-strategy/README.md)
- [`../ragas-llm-judge/`](../ragas-llm-judge/README.md) — how this
  pipeline gets evaluated
