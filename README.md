# AI Engineer Roadmap

A working repo, not a tutorial repo — this is where I'm building out
real implementations, demos, and one flagship project spanning **AI
Engineering** and **AIOps**, organized as a roadmap so it grows in a
sensible order instead of 30 disconnected folders.

Most topic folders currently hold documentation only (see each folder's
Status line) — code, notebooks, and demos are being committed
progressively as I work through [`roadmap.md`](roadmap.md).

## About me

I'm an AI Engineer and AIOps specialist with 10+ years across cloud
infrastructure, DevOps, and applied AI engineering — spanning AWS,
Azure, and IBM Cloud in regulated, high-scale environments (banking and
financial services, including Societe Generale and KPMG). My background
started in cloud and DevOps — CI/CD, Kubernetes, Infrastructure as Code —
and has extended into AIOps and GenAI engineering: designing production
AI infrastructure, building autonomous multi-agent systems (LangChain,
LangGraph), and engineering RAG pipelines with proper evaluation and
observability.

I don't see AI engineering and DevOps as separate disciplines. AIOps,
done right, is DevOps rigor applied to AI/ML systems — models fail in
production the same way services do: silently, under load, at 3 AM. This
repo is where I build and document that combined skill set in public.

- BIBHUTI BHUSAN PANDA
- 🎓 B.Tech, Computer Science & Engineering
- ☁️ AWS · Azure · IBM Cloud certified
- 💼 Currently: Lead Software Engineer — AIOps
- 📍 Bengaluru, India

## Repository structure

```
.
├── .github/            # Issue/PR templates, CI workflow
├── tests/              # Test suite (mirrors ai_engineer/ and aiops/)
├── ai_engineer/        # AI engineering: Python, RAG, LangChain/LangGraph
│   ├── python-fundamentals/
│   ├── rag/
│   └── langchain-langgraph/
├── aiops/              # AIOps: self-healing infra, observability, GitOps
│   ├── agentic-self-healing-azure/   ← flagship project
│   ├── opentelemetry-metrics/
│   ├── llm-eval/
│   ├── policy-guardrails/
│   ├── terraform/
│   ├── keda/
│   ├── flux-cd/
│   └── argocd/
├── roadmap.md          # Build-order checklist
└── README.md           # You are here
```

See [`ai_engineer/README.md`](ai_engineer/README.md) and
[`aiops/README.md`](aiops/README.md) for what each topic folder covers,
and [`roadmap.md`](roadmap.md) for the order things are being built in.

## Why two top-level folders

`ai_engineer/` and `aiops/` are deliberately kept separate: one is about
**building** AI-powered software (RAG, agents, orchestration
frameworks), the other is about **operating** it and using it to operate
other things (observability, guardrails, GitOps, self-healing infra).
The flagship project,
[`aiops/agentic-self-healing-azure/`](aiops/agentic-self-healing-azure/README.md),
is where both halves meet.

## Status & contributing

This is a personal learning-in-public repo — issues and PRs against my
own roadmap are tracked via the templates in `.github/`. Not actively
seeking outside contributions, but feel free to open an issue if
something's unclear or you spot a mistake.

## License

MIT — see [LICENSE](LICENSE).
