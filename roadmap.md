# Roadmap

A build-order checklist for this repo. Nothing here is on a deadline —
it's sequenced so each phase gives the next one something real to build
on, rather than 20 disconnected topics.

Update a box to `[x]` when a folder's README status moves from 📋 to ✅.

## Phase 1 — Python & API Foundations
- [ ] `ai_engineer/python-fundamentals/decorators/`
- [ ] `ai_engineer/python-fundamentals/dependency-injection/`
- [ ] `ai_engineer/python-fundamentals/fastapi/`
- [ ] `ai_engineer/python-fundamentals/api-design-patterns/`

## Phase 2 — RAG Foundations
- [ ] `ai_engineer/rag/rag-pipeline/`
- [ ] `ai_engineer/rag/chunking-strategy/`
- [ ] `ai_engineer/rag/retrieval-strategy/`

## Phase 3 — Advanced & Agentic RAG
- [ ] `ai_engineer/rag/agentic-rag/`
- [ ] `ai_engineer/rag/multimodal-rag/`
- [ ] `ai_engineer/rag/ragas-llm-judge/`

## Phase 4 — Orchestration Frameworks
- [ ] `ai_engineer/langchain-langgraph/langchain/`
- [ ] `ai_engineer/langchain-langgraph/langgraph/`

## Phase 5 — AIOps Foundations
- [ ] `aiops/opentelemetry-metrics/`
- [ ] `aiops/policy-guardrails/`
- [ ] `aiops/terraform/`
- [ ] `aiops/keda/`
- [ ] `aiops/flux-cd/` or `aiops/argocd/` (pick one first, add the other later)

## Phase 6 — LLM Evaluation Discipline
- [ ] `aiops/llm-eval/`
- [ ] `tests/` wired into `.github/workflows/ci.yml`

## Phase 7 — Capstone: Agentic Self-Healing System
- [ ] `aiops/agentic-self-healing-azure/` — brings together agentic RAG,
      LangGraph orchestration, OTel signals, policy guardrails, and LLM
      eval into one working system

## Ongoing
- [ ] Keep each folder's `README.md` "Status" line accurate as code lands
- [ ] Keep [`README.md`](README.md)'s structure table in sync with any
      new/renamed folders
