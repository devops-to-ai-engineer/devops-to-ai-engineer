# AI Engineer

The reasoning, retrieval, and application layer — everything about
building AI-powered software, as distinct from operating it in
production (that's [`../aiops/`](../aiops/README.md)).

Organized as a rough learning path: fundamentals first, then RAG in
increasing depth, then the orchestration frameworks that tie it together.

| Topic | Covers |
|---|---|
| [`python-fundamentals/`](python-fundamentals/README.md) | Decorators, dependency injection, FastAPI, API design patterns |
| [`rag/`](rag/README.md) | Baseline pipeline → chunking → retrieval → agentic RAG → multimodal → RAGAS/LLM-judge evaluation |
| [`langchain-langgraph/`](langchain-langgraph/README.md) | LangChain fundamentals, then LangGraph for stateful/branching agent orchestration |

## How this connects to AIOps

The [`agentic-self-healing-azure`](../aiops/agentic-self-healing-azure/README.md)
project in `aiops/` is where these two halves meet: it's an AIOps system
built using AI Engineer techniques from this folder — agentic RAG over
runbooks, LangGraph-orchestrated decision-making, and the same
evaluation discipline covered in `rag/ragas-llm-judge/` and
`aiops/llm-eval/`.

## Status

📋 Documentation-only scaffold for now — code, notebooks, and working
demos are being added progressively to each subfolder. See the root
[`roadmap.md`](../roadmap.md) for sequencing and progress.
