# Tests

Test suite for this repo, mirroring the `ai_engineer/` and `aiops/`
folder structure so it's obvious where a given module's tests live.

## Planned structure

```
tests/
├── ai_engineer/
│   ├── python_fundamentals/
│   ├── rag/
│   └── langchain_langgraph/
└── aiops/
    ├── agentic_self_healing_azure/
    ├── opentelemetry_metrics/
    ├── llm_eval/
    └── policy_guardrails/
```

## Approach

- **Unit tests** for pure logic (chunking functions, policy precondition
  checks, confidence adjustment math) — fast, no external dependencies.
- **Eval-style tests** for anything LLM-touching (`aiops/llm-eval/`,
  `ai_engineer/rag/ragas-llm-judge/`) — a labeled case set with an
  accuracy threshold, not a single assert-equal, since LLM outputs
  aren't perfectly deterministic.
- **Integration tests** for the end-to-end demo path in
  `aiops/agentic-self-healing-azure/`, run against mocked signals/
  cluster state so they don't require live infrastructure or API keys.

`pytest` is the intended runner, wired into
[`../.github/workflows/ci.yml`](../.github/workflows/ci.yml) once tests
exist.

## Status

📋 Placeholder — tests will be added alongside the code they cover, not
written speculatively ahead of it.
