# LangChain

Framework for chaining LLM calls, tools, and memory into an orchestrated
pipeline — the base abstraction layer most agent frameworks (including
LangGraph) build on.

## Why this matters
LangChain is the fastest path to wiring a prompt, a retriever, and a
tool together without hand-rolling the plumbing. Understanding where its
abstractions help (rapid prototyping, standard integrations) vs. where a
simpler hand-written pipeline is more auditable is itself the skill —
not just "use LangChain for everything."

## Key concepts
- LCEL (LangChain Expression Language) for composing chains
- Tool/function-calling integration
- Output parsers and structured output enforcement
- Memory classes and their limits at scale
- Chains vs. explicit orchestration — when LangGraph (sibling folder)
  is the better fit

## Planned contents
- `basic_chain_demo.py`
- `tool_calling_demo.py`
- `structured_output_demo.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
