# AIOps

Applying DevOps rigor — observability, IaC, GitOps, policy-as-code — to
AI/agent systems, and using AI agents to operate infrastructure. This is
the production/operational counterpart to
[`../ai_engineer/`](../ai_engineer/README.md).

| Topic | Covers |
|---|---|
| [`agentic-self-healing-azure/`](agentic-self-healing-azure/README.md) | **Flagship project** — an agent that detects, diagnoses, and remediates infra failures on Azure/AKS |
| [`opentelemetry-metrics/`](opentelemetry-metrics/README.md) | The signal layer everything else reads from — traces, metrics, logs |
| [`llm-eval/`](llm-eval/README.md) | Measuring whether the agent's operational decisions are actually good |
| [`policy-guardrails/`](policy-guardrails/README.md) | The declarative allow-list bounding what the agent can do |
| [`terraform/`](terraform/README.md) | IaC for the lab environment and agent-triggered infra changes |
| [`keda/`](keda/README.md) | Event-driven autoscaling — both infra and an agent remediation action |
| [`flux-cd/`](flux-cd/README.md) | GitOps delivery (pull-based) |
| [`argocd/`](argocd/README.md) | GitOps delivery (the ArgoCD alternative) |

## How this connects to AI Engineer

`agentic-self-healing-azure` is where AI Engineer techniques
(`../ai_engineer/rag/agentic-rag/`, `../ai_engineer/langchain-langgraph/langgraph/`)
get applied to a real operational problem, gated by the guardrails and
evaluation discipline defined in this folder.

## Status

📋 Documentation-only scaffold for now. See the root
[`roadmap.md`](../roadmap.md) for build sequencing.
