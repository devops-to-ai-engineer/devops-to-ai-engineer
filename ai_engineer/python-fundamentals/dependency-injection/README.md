# Dependency Injection

Supplying a function or class with the things it depends on (a database
connection, an LLM client, a config object) from the outside, rather than
constructing them internally — the core pattern behind FastAPI's `Depends()`.

## Why this matters
Every real agent/service in this repo needs to swap implementations
without touching business logic — a mock LLM client in tests, a real
Azure OpenAI client in production; a local vector store in dev, Pinecone
in production. DI is what makes that swap a config change instead of a
code change.

## Key concepts
- Constructor injection vs. FastAPI's `Depends()` function injection
- Interfaces/protocols as the contract DI relies on (see how
  `LLMClient` is meant to work as an abstract base across providers)
- Singleton vs. per-request dependency scope
- DI containers vs. "just pass it in" — when the extra machinery is worth it

## Planned contents
- `manual_di_example.py` — DI without a framework, just constructor args
- `fastapi_depends_example.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
