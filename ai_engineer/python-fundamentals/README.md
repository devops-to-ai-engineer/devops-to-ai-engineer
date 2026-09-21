# Python Fundamentals

The Python patterns that show up constantly in real AI/agent codebases —
not a general Python tutorial, but the specific mechanisms worth knowing
cold before building anything more complex in `ai_engineer/`.

| Topic | Why it's here |
|---|---|
| [`decorators/`](decorators/README.md) | Retry/backoff, caching, and the mechanism behind FastAPI routes and LangChain's `@tool` |
| [`dependency-injection/`](dependency-injection/README.md) | Swapping mock ↔ real LLM clients, dev ↔ prod vector stores, without touching business logic |
| [`fastapi/`](fastapi/README.md) | Exposing agent logic as a real, callable HTTP service |
| [`api-design-patterns/`](api-design-patterns/README.md) | Making that service's API stable, versioned, and safe to retry |

## Status

📋 Documentation-only placeholder — code and demos coming progressively.
