# RAGAS & LLM-as-Judge

Evaluating RAG pipeline quality with reference-free and reference-based
metrics (RAGAS: faithfulness, answer relevance, context precision/
recall) and using a second LLM as a grading judge for outputs that don't
have a single correct answer.

## Why this matters
"It looks right" isn't a metric. Without a scoring framework, it's
impossible to tell whether a change to chunking, retrieval, or prompting
actually improved anything — this is what turns RAG development from
vibes into measurement, and is the same discipline this repo's broader
eval-suite theme is built on.

## Key concepts
- RAGAS metrics: faithfulness (is the answer grounded in retrieved
  context?), answer relevance, context precision/recall
- LLM-as-judge: using a strong model to score outputs against a rubric,
  including known failure modes of this approach (judge bias, verbosity
  bias)
- Building a ground-truth eval set (see the Hugging Face datasets angle
  in `ai_engineer/rag/rag-pipeline/`'s broader eval story)
- Regression testing a RAG pipeline in CI using these metrics

## Planned contents
- `ragas_eval.py`
- `llm_judge.py` — a structured-rubric grading prompt + parser
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
