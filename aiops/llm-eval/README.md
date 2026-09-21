# LLM Evaluation (for AIOps)

Measuring whether the agent's diagnoses and decisions are actually good —
accuracy, hallucination rate, confidence calibration, and cost/latency —
specifically for an operational agent, not a chatbot.

## Why this matters
An AIOps agent's mistakes have real consequences (a wrong restart, a
missed escalation), so "does it work" needs a harder answer than
eyeballing a few examples. This is what gates any change to the prompt,
model, or policy before it ships — see the CI angle in the root
`tests/` folder.

## Key concepts
- Accuracy against a labeled set of known failure signatures
- Confidence calibration — does the model's stated confidence actually
  track its correctness rate?
- False-escalation rate vs. false-remediation rate, and why they're not
  symmetric costs
- Drift detection — catching when live performance degrades from the
  eval-time baseline
- Cost/latency benchmarking per model/prompt version

## Planned contents
- `eval_suite/cases.yaml` — labeled signal → expected diagnosis pairs
- `eval_metrics.py`
- `confidence_calibration.py`
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../../ai_engineer/rag/ragas-llm-judge/`](../../ai_engineer/rag/ragas-llm-judge/README.md) —
  the same measurement discipline applied to RAG instead of ops decisions
