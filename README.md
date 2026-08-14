<!--
  README.md — deionx profile (Pro grade, 2026)
  Paste this into the repository named `deionx`
-->

# <img src="./deionx-logo.svg" alt="deionx logo" width="220" style="vertical-align:middle"> DEIONX

<p align="center">
  <strong>Full‑stack Engineer • Systems Architect • AI Systems Specialist</strong><br/>
  Building resilient systems, high‑performance products, and developer tools that scale.
</p>

---

## About

**Deionx** is a pragmatic engineer who blends systems thinking, production engineering, and applied AI to deliver measurable outcomes. I design and ship production‑grade software that balances **performance**, **clarity**, and **developer experience**. My work focuses on building reliable APIs, modular frontends, automation pipelines, and AI‑enabled tooling that accelerate teams.

**Core strengths**
- **System Design** — resilient, observable, cost‑efficient architectures  
- **API Engineering** — contract‑first design, versioning, and backward compatibility  
- **Frontend Engineering** — componentized, accessible, and high‑performance UI  
- **AI Systems** — model integration, inference at scale, and safe observability  
- **Automation** — CI/CD, infra as code, release pipelines, and developer DX  
- **Performance** — p95/p99 optimization, microbenchmarks, and real user metrics

---

## Vision

I build software that lasts. That means:
- **Design first**: contracts, telemetry, and failure modes defined before code.  
- **Measure everything**: metrics, traces, and SLOs drive decisions.  
- **Automate relentlessly**: reduce manual toil and increase developer velocity.  
- **Ship with confidence**: tests, canaries, and progressive rollouts.

---

## Tech Stack

**Languages**  
`TypeScript` • `Python` • `Rust` • `Go`

**Frontend**  
`React` • `Next.js` • `Tailwind CSS` • `Vite` • `Storybook`

**Backend**  
`Node.js` • `FastAPI` • `gRPC` • `Postgres` • `Redis`

**Cloud and Infra**  
`Docker` • `Kubernetes` • `Terraform` • `Vercel` • `AWS` • `Edge Functions`

**Observability and Data**  
`Prometheus` • `Grafana` • `OpenTelemetry` • `Sentry` • `ClickHouse`

**AI and ML Integration**  
Model orchestration, inference at the edge, prompt engineering, and safe telemetry.

---

## Signature Projects

### Platform API
- **Role**: Lead engineer — API design, schema evolution, performance tuning.  
- **Highlights**: sub‑50ms p95 responses, automated canary deploys, contract tests.

### Design System
- **Role**: Creator — tokens, accessible components, cross‑product theming.  
- **Highlights**: zero‑runtime CSS, strict accessibility rules, visual regression tests.

### Dev Automation Suite
- **Role**: Architect — CI templates, release automation, local dev tooling.  
- **Highlights**: reduced release time by 70%, standardized observability.

### Playground and Experiments
- **Role**: Research and prototyping — wasm, edge compute, microbenchmarks.  
- **Highlights**: reproducible benchmarks and small, focused POCs.

---

## Architecture Notes

**Principles**
- **Single responsibility** per service and clear ownership.  
- **Observable by default**: metrics, traces, and structured logs.  
- **Contract driven**: OpenAPI / gRPC first, with automated contract tests.  
- **Progressive rollout**: feature flags, canaries, and automated rollbacks.

**Patterns**
- **API Gateway** for routing and auth, with thin edge logic.  
- **Event driven** for eventual consistency and decoupling.  
- **Sidecar telemetry** for consistent tracing and metrics.

---

## Local Development

**Clone and run**
```bash
git clone https://github.com/deionx/deionx.git
cd deionx
# example: start platform-api
cd platform-api
pnpm install
pnpm dev
