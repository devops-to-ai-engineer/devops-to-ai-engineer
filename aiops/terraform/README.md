# Terraform

Infrastructure-as-code for the AIOps lab environment and for any
infrastructure changes the agent itself might trigger.

## Why this matters
Any action the agent can take should be deployable and auditable the
same way any other infra change is — through IaC and version control,
not ad hoc scripts run by hand. This folder is also where the sandbox
cluster used by the self-healing demo gets defined.

## Key concepts
- Provider configuration (Azure/AzureRM) and state management
- Module design for reusable infra components (cluster, node pool, KEDA
  installation)
- Plan/apply workflow integrated into CI (see `flux-cd`/`argocd` for the
  GitOps alternative for application-level deployments)

## Planned contents
- `main.tf` — AKS sandbox cluster definition
- `modules/` — reusable cluster/networking modules
- `NOTES.md`

## Status
📋 Documentation-only placeholder — code and demos coming progressively.
