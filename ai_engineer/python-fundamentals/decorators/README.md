# Decorators

Python decorators — functions that wrap other functions/classes to add
behavior without changing their code. The mechanism behind a lot of what
looks like "magic" in FastAPI, pytest, and dataclasses.

## Why this matters
Decorators show up constantly in production AI/ops code: `@retry` around
a flaky LLM call, `@lru_cache` around an expensive embedding lookup,
`@app.get(...)` in FastAPI, `@tool` in LangChain for registering agent
tools. Understanding how they actually work (closures, `functools.wraps`)
is the difference between using them and debugging them when they go
wrong.

## Key concepts
- Functions as first-class objects, closures
- `functools.wraps` and why it matters for introspection/debugging
- Decorators with arguments (`@retry(max_attempts=3)`)
- Class-based decorators
- Real-world uses: retry/backoff, caching, timing/logging, auth checks,
  LangChain's `@tool` decorator

## Planned contents
- `basic_decorator.py`
- `decorator_with_args.py`
- `retry_decorator.py` — a real retry/backoff decorator for flaky LLM API calls
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
