# LangChain & LangGraph Deep Dive

| Topic | Covers |
|---|---|
| [`langchain/`](langchain/README.md) | Chains, tool calling, structured output — the base orchestration layer |
| [`langgraph/`](langgraph/README.md) | Explicit state graphs for branching, cyclical, and human-in-the-loop agent workflows |

The natural progression is left-to-right: start with a LangChain chain,
move to LangGraph once the workflow needs branches, retries, or
persistence that a linear chain can't express cleanly — this is exactly
the path the [`agentic-self-healing-azure`](../../aiops/agentic-self-healing-azure/README.md)
project is expected to take.

## Status

📋 Documentation-only placeholder — code and demos coming progressively.
