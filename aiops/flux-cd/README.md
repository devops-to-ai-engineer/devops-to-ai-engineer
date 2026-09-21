# Flux CD

GitOps continuous delivery for Kubernetes — the cluster's actual state is
continuously reconciled to match what's declared in Git, rather than
pushed to imperatively.

## Why this matters
For an agent that can trigger infrastructure changes, GitOps discipline
matters even more than usual: every change (agent-triggered or human)
should be visible as a Git commit, reviewable, and revertible. This
folder covers the pull-based GitOps model as one option; see `argocd`
for the alternative implementation.

## Key concepts
- Pull-based reconciliation vs. push-based CI/CD deployment
- Source controllers (Git, Helm, OCI) and Kustomize/Helm integration
- Progressive delivery (canary/blue-green) via Flagger
- Drift detection and automatic correction — conceptually similar to
  this repo's own agent drift-detection theme, applied to infra config
  instead of LLM behavior

## Planned contents
- `flux-bootstrap.md` — cluster bootstrap steps
- `kustomization.yaml` example
- `NOTES.md` — comparison notes vs. ArgoCD

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../argocd/`](../argocd/README.md)
