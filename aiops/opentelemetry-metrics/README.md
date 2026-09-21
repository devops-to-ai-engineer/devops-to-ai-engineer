# OpenTelemetry Metrics

Vendor-neutral instrumentation for traces, metrics, and logs — the
observability substrate everything else in AIOps reads from.

## Why this matters
An agent can only diagnose what it can see. Before any self-healing
logic makes sense, the signal layer — what gets measured, how it's
normalized, how noisy vs. reliable it is — has to be solid. Most of the
real engineering effort in AIOps lives here, not in the LLM call.

## Key concepts
- Traces vs. metrics vs. logs, and when each is the right signal type
- OTel Collector pipeline: receivers → processors → exporters
- Instrumenting an application vs. instrumenting infrastructure
  (application traces vs. Kubernetes events)
- Cardinality and cost control for metrics at scale
- Exporting to Prometheus/Grafana/Azure Monitor

## Planned contents
- `otel_collector_config.yaml` — reference collector configuration
- `k8s_signal_normalizer.py` — normalizing raw K8s events into a
  consistent schema for downstream diagnosis
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../agentic-self-healing-azure/`](../agentic-self-healing-azure/README.md) —
  the consumer of this signal layer
