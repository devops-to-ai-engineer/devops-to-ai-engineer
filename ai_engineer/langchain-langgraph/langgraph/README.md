# LangGraph

Graph-based orchestration for agents with explicit state, branching, and
cycles — for workflows a linear LangChain chain can't cleanly express.

## Why this matters
Real agent workflows branch: retry a failed step, escalate on low
confidence, run parallel investigation paths. Modeling this as an
explicit state graph (rather than a single linear chain) makes the
control flow reviewable and testable — critical for an agent whose
decisions might trigger real infrastructure actions (see the AIOps
`agentic-self-healing-azure` topic).

## Key concepts
- Nodes, edges, and conditional edges
- Shared state schema across the graph (TypedDict/Pydantic state)
- Cycles for retry loops vs. plain DAGs
- Persistence/checkpointing — resuming a long-running or interrupted
  agent process
- Human-in-the-loop interrupts for low-confidence decision points

## Planned contents
- `incident_response_graph.py` — a state graph modeling detect →
  diagnose → remediate/escalate → resolve
- `checkpointing_demo.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../../rag/agentic-rag/`](../../rag/agentic-rag/README.md) — a
  natural use case for a LangGraph-orchestrated retrieval loop
