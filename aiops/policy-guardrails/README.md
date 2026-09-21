# Policy Guardrails

The declarative rules that bound what an agent is allowed to do — a
pre-approved action allow-list, blast-radius limits, and hard escalation
triggers — enforced in code, never left to the LLM's judgment alone.

## Why this matters
This is the safety layer that makes autonomous remediation defensible in
a production/regulated environment. The rule: the agent's action-space
is defined here, declaratively, and the LLM selects *which* allowed
action to take — it never gets to invent a new one at runtime.

## Key concepts
- Allow-list design: action, preconditions, blast radius, reversibility
- Confidence thresholds and why false escalation should be cheaper than
  false remediation
- Hard stops that bypass confidence entirely (e.g. actions requiring
  human approval regardless of how "sure" the model is)
- Audit logging — every decision reviewable after the fact like any
  other production change

## Planned contents
- `remediation_actions.yaml` — the declarative allow-list
- `escalation_policy.md`
- `policy_engine.py` — evaluates preconditions against a proposed action
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
