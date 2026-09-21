# FastAPI

The async Python web framework used to expose agent/model endpoints as
real services — request validation, auto-generated OpenAPI docs, and
native `async`/`await` support.

## Why this matters
An agent that only runs as a CLI script isn't deployable behind a load
balancer or callable from another service. FastAPI is the layer that
turns `ai_engineer` agent logic into a real HTTP service other systems
(a chatbot frontend, an internal dashboard, another microservice) can
call.

## Key concepts
- Path/query/body params and Pydantic request validation
- Async endpoints and why that matters for I/O-bound LLM calls
- Dependency injection via `Depends()` (see sibling folder)
- Background tasks for long-running agent runs
- Streaming responses (token-by-token LLM output over HTTP)

## Planned contents
- `main.py` — a minimal FastAPI app exposing an agent-diagnose endpoint
- `streaming_response_demo.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
