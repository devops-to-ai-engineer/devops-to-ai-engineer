# KEDA (Kubernetes Event-Driven Autoscaling)

Event-driven autoscaling for Kubernetes workloads — scaling on queue
depth, custom metrics, or other event sources instead of just CPU/memory.

## Why this matters
KEDA is both infrastructure *and* one of the agent's own remediation
tools: `rescale_via_keda` is a safer, more scoped action than restarting
individual pods when the real issue is a capacity/load problem across a
whole deployment.

## Key concepts
- ScaledObjects and scalers (Prometheus, queue-based, custom metrics)
- Scale-to-zero for cost optimization on bursty workloads
- Cooldown periods and avoiding scale-flapping
- GPU-aware scaling for inference workloads specifically

## Planned contents
- `scaledobject.yaml` — reference config for an inference-worker deployment
- `NOTES.md` — real-world tuning notes (thresholds, cooldowns)

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
