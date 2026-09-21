# Agentic RAG

RAG where retrieval itself is a decision the agent makes — deciding
*whether* to retrieve, *what* to retrieve, and *whether the retrieved
context is even good enough* to answer with — rather than always doing
one fixed retrieval step per query.

## Why this matters
Naive RAG retrieves unconditionally, even for queries that don't need
it, and never checks whether what came back is actually sufficient. An
agentic loop can decide "this needs a second, more specific search" or
"the retrieved context doesn't answer this, escalate/say so" instead of
confidently generating from weak context.

## Key concepts
- Retrieval as a tool call the agent can choose to invoke (or not)
- Self-grading retrieved context before generating (corrective RAG)
- Iterative/multi-hop retrieval loops
- Deciding when to stop retrieving and either answer or say "I don't
  have enough information" — directly relevant to this repo's broader
  confidence/escalation theme

## Planned contents
- `retrieval_tool.py` — retrieval exposed as an agent-callable tool
- `corrective_rag_loop.py` — self-grading + re-retrieval loop
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../../langchain-langgraph/langgraph/`](../../langchain-langgraph/langgraph/README.md) —
  natural orchestration substrate for this loop
