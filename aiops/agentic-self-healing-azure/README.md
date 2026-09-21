# Agentic Self-Healing Architecture on Azure

The flagship AIOps project in this repo: an AI agent that watches
Azure/Kubernetes infrastructure health signals, diagnoses failures, and
triggers scoped remediation — with human escalation as a hard fallback,
not an afterthought.

## Why this matters
This is where every other AIOps topic in this repo (OpenTelemetry
metrics, policy guardrails, KEDA, GitOps) and every relevant AI Engineer
topic (agentic RAG, LangGraph orchestration, LLM eval) come together into
one end-to-end system. It's the concrete answer to "what does AIOps
actually look like in production," not just a demo.

## Key concepts
- Signal → diagnosis → action → verification loop
- Confidence-gated automation (act only above a threshold; escalate
  below it — see [`../policy-guardrails/`](../policy-guardrails/README.md))
- Scoped, auditable remediation actions (restart, rescale, cordon) with
  an explicit allow-list, never an agent improvising an action
- Full observability of the agent's own decisions, not just the
  infrastructure it watches

## Planned architecture (high level)
```
Azure Monitor / OTel  →  Signal normalization  →  LLM diagnosis
        ↑                                              │
        │                                    confidence check
   AKS / KEDA  ←──── scoped remediation ────┐          │
                                             └── escalate → on-call
```

## Planned contents
- `architecture.md` — full design doc once implementation starts
- `agent/` — the core diagnose/act/escalate loop
- `demo/` — a runnable local demo (mock signals, no live cluster required)
- `NOTES.md`

## Status
📋 Documentation-only placeholder — this is the capstone project; other
AIOps and AI Engineer topics in this repo feed into it as they mature.
