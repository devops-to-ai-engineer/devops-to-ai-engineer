# API Design Patterns

Patterns for designing APIs that are easy to consume, version, and evolve
— relevant both for a REST API wrapping an agent and for the internal
"API" an agent exposes to its own tools.

## Why this matters
A messy API design compounds every time another consumer (a frontend, a
second service, a partner team) starts depending on it. Getting request/
response shapes, versioning, and error handling right early avoids
painful breaking changes later — especially for an agent API where the
response shape (diagnosis, confidence, action taken) needs to stay stable
as the agent's internals change.

## Key concepts
- REST resource modeling vs. RPC-style action endpoints (relevant for
  "trigger remediation" style calls that aren't naturally resource-based)
- Versioning strategies (URL path, header-based)
- Consistent error response shapes
- Idempotency for action-triggering endpoints (important: retrying a
  "restart pod" call should never double-restart)
- Pagination and filtering for list endpoints (e.g. incident history)

## Planned contents
- `error_handling_example.py`
- `idempotency_key_example.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
