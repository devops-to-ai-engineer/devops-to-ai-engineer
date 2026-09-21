# ArgoCD

GitOps continuous delivery for Kubernetes with a strong UI/UX and
multi-cluster management focus — the alternative to Flux CD covered in
the sibling folder.

## Why this matters
Worth evaluating alongside Flux specifically for its application-centric
UI (useful for visualizing what the agent's remediation actions actually
changed) and its more explicit sync/health-status model.

## Key concepts
- Application CRDs and the sync/health status model
- App-of-apps pattern for managing many services declaratively
- Sync waves and hooks for ordered, multi-step deployments
- RBAC and multi-tenancy for a shared cluster

## Planned contents
- `application.yaml` example
- `app-of-apps/` pattern example
- `NOTES.md` — decision record: ArgoCD vs. Flux for this project

## Status
📋 Documentation-only placeholder — code and demos coming progressively.

## See also
- [`../flux-cd/`](../flux-cd/README.md)
