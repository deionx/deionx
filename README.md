<div align="center">
[![Deionx](https://raw.githubusercontent.com/deionx/deionx/refs/heads/main/deionx-logo.svg)](https://github.com/deionx)
    
# DEIONX

### Full-Stack Engineer · Systems Architect · AI Engineer

**I build software that survives contact with reality.**

Production systems · Developer tooling · AI · Automation · Infrastructure

<br />

[![GitHub](https://img.shields.io/badge/GitHub-DEIONX-181717?style=for-the-badge&logo=github)](https://github.com/deionx)
[![Profile Views](https://komarev.com/ghpvc/?username=deionx&style=for-the-badge&color=7C3AED)](https://github.com/deionx)

</div>

---

## `> whoami`

I'm **Deion** — a software engineer interested in the intersection of:

- ⚙️ **Systems**
- 🧠 **AI**
- 🎨 **Product**
- 🚀 **Infrastructure**
- 🤖 **Automation**

I like taking ambiguous problems, turning them into clean systems, and shipping software that is **fast, observable, maintainable, and useful**.

My engineering philosophy is simple:

> **Good software isn't just code that works.  
> It's software that keeps working.**

---

## `// engineering philosophy`

```mermaid
flowchart LR
    A["Problem"] --> B["Constraints"]
    B --> C["Architecture"]
    C --> D["Implementation"]
    D --> E["Measure"]
    E --> F["Improve"]
    F --> C

    style A fill:#18181b,color:#fff,stroke:#7c3aed
    style B fill:#18181b,color:#fff,stroke:#7c3aed
    style C fill:#18181b,color:#fff,stroke:#06b6d4
    style D fill:#18181b,color:#fff,stroke:#06b6d4
    style E fill:#18181b,color:#fff,stroke:#22c55e
    style F fill:#18181b,color:#fff,stroke:#22c55e
```

### The rules

**01 · Design before implementation**

Understand the problem, boundaries, constraints, and failure modes first.

**02 · Measure everything**

If something matters, it should be observable.

**03 · Automate the boring parts**

Manual repetition is an opportunity for tooling.

**04 · Make failure boring**

Timeouts, retries, rollbacks, graceful degradation, and clear recovery paths.

**05 · Keep complexity earned**

Every abstraction should solve a real problem.

**06 · Ship progressively**

Small changes. Fast feedback. Observable deployments.

---

# `// stack`

## Languages

<p>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" />
<img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
</p>

## Frontend

<p>
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
</p>

## Backend

<p>
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
</p>

## Infrastructure

<p>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
<img src="https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white" />
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
</p>

## Observability

<p>
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" />
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" />
<img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white" />
<img src="https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white" />
</p>

---

# `// what I build`

<table>
<tr>

<td width="50%" valign="top">

## ⚙️ Systems

I enjoy designing software around:

- clear boundaries
- explicit contracts
- predictable failure modes
- scalability
- performance
- observability

</td>

<td width="50%" valign="top">

## 🧠 AI

Interested in practical AI systems:

- model integration
- inference
- agents
- evaluation
- automation
- AI-native applications

</td>

</tr>

<tr>

<td width="50%" valign="top">

## 🎨 Product

Building interfaces that are:

- fast
- accessible
- composable
- maintainable
- intentionally designed

</td>

<td width="50%" valign="top">

## 🚀 Infrastructure

Making engineering teams faster through:

- CI/CD
- automation
- cloud infrastructure
- developer tooling
- reproducible environments
- observability

</td>

</tr>
</table>

---

# `// system architecture`

When I think about a production system, I think in layers:

```mermaid
flowchart TB

    U["Users / Clients"]

    U --> EDGE["Edge / CDN"]

    EDGE --> API["API Gateway"]

    API --> AUTH["Authentication"]
    API --> SERVICES["Application Services"]

    SERVICES --> WORKERS["Background Workers"]
    SERVICES --> CACHE["Redis / Cache"]
    SERVICES --> DB["Primary Database"]

    WORKERS --> QUEUE["Message Queue"]
    QUEUE --> EVENTS["Event Processing"]

    DB --> ANALYTICS["Analytics / Data"]
    EVENTS --> ANALYTICS

    SERVICES --> OBS["Observability"]
    WORKERS --> OBS
    API --> OBS

    OBS --> METRICS["Metrics"]
    OBS --> LOGS["Logs"]
    OBS --> TRACES["Traces"]
    OBS --> ALERTS["Alerts"]

    style U fill:#18181b,color:#fff,stroke:#7c3aed
    style EDGE fill:#18181b,color:#fff,stroke:#7c3aed
    style API fill:#18181b,color:#fff,stroke:#06b6d4
    style AUTH fill:#18181b,color:#fff,stroke:#06b6d4
    style SERVICES fill:#18181b,color:#fff,stroke:#06b6d4
    style WORKERS fill:#18181b,color:#fff,stroke:#06b6d4
    style CACHE fill:#18181b,color:#fff,stroke:#f59e0b
    style DB fill:#18181b,color:#fff,stroke:#22c55e
    style QUEUE fill:#18181b,color:#fff,stroke:#f59e0b
    style EVENTS fill:#18181b,color:#fff,stroke:#f59e0b
    style ANALYTICS fill:#18181b,color:#fff,stroke:#22c55e
    style OBS fill:#18181b,color:#fff,stroke:#ec4899
    style METRICS fill:#18181b,color:#fff,stroke:#ec4899
    style LOGS fill:#18181b,color:#fff,stroke:#ec4899
    style TRACES fill:#18181b,color:#fff,stroke:#ec4899
    style ALERTS fill:#18181b,color:#fff,stroke:#ec4899
```

### Architectural defaults

| Principle | Approach |
|---|---|
| **Boundaries** | Keep responsibilities explicit |
| **APIs** | Stable contracts and predictable behavior |
| **Data** | Choose storage based on workload |
| **Async work** | Queues and workers where appropriate |
| **Caching** | Reduce unnecessary computation and I/O |
| **Observability** | Metrics, logs, and traces from day one |
| **Deployments** | Small, reversible, observable changes |
| **Failure** | Graceful degradation over catastrophic failure |

---

# `// development lifecycle`

```mermaid
flowchart LR

    P["Problem"] --> R["Research"]
    R --> D["Design"]
    D --> B["Build"]
    B --> T["Test"]
    T --> S["Ship"]
    S --> O["Observe"]
    O --> I["Iterate"]

    I --> D

    style P fill:#18181b,color:#fff,stroke:#7c3aed
    style R fill:#18181b,color:#fff,stroke:#7c3aed
    style D fill:#18181b,color:#fff,stroke:#06b6d4
    style B fill:#18181b,color:#fff,stroke:#06b6d4
    style T fill:#18181b,color:#fff,stroke:#22c55e
    style S fill:#18181b,color:#fff,stroke:#22c55e
    style O fill:#18181b,color:#fff,stroke:#f59e0b
    style I fill:#18181b,color:#fff,stroke:#ec4899
```

**Problem → Research → Design → Build → Test → Ship → Observe → Iterate**

---

# `// AI × software`

```mermaid
flowchart LR

    INPUT["User / Application"] --> ROUTER["AI Router"]

    ROUTER --> MODEL["Model"]
    ROUTER --> TOOLS["Tools"]
    ROUTER --> MEMORY["Context / Memory"]

    MODEL --> EVAL["Evaluation"]
    TOOLS --> EVAL
    MEMORY --> EVAL

    EVAL --> OBS["Observability"]

    OBS --> COST["Cost"]
    OBS --> LATENCY["Latency"]
    OBS --> QUALITY["Quality"]
    OBS --> RELIABILITY["Reliability"]

    style INPUT fill:#18181b,color:#fff,stroke:#7c3aed
    style ROUTER fill:#18181b,color:#fff,stroke:#06b6d4
    style MODEL fill:#18181b,color:#fff,stroke:#06b6d4
    style TOOLS fill:#18181b,color:#fff,stroke:#06b6d4
    style MEMORY fill:#18181b,color:#fff,stroke:#06b6d4
    style EVAL fill:#18181b,color:#fff,stroke:#22c55e
    style OBS fill:#18181b,color:#fff,stroke:#ec4899
    style COST fill:#18181b,color:#fff,stroke:#f59e0b
    style LATENCY fill:#18181b,color:#fff,stroke:#f59e0b
    style QUALITY fill:#18181b,color:#fff,stroke:#22c55e
    style RELIABILITY fill:#18181b,color:#fff,stroke:#22c55e
```

The interesting part isn't simply **calling a model**.

It's building systems around AI that remain:

`reliable` · `observable` · `fast` · `affordable` · `testable`

---

# `// currently exploring`

<table>
<tr>
<td align="center" width="25%">

### AI Systems

Agents  
Inference  
Evaluation  
Tool use

</td>

<td align="center" width="25%">

### Distributed Systems

Queues  
Events  
Caching  
Reliability

</td>

<td align="center" width="25%">

### Developer Experience

Tooling  
Automation  
CI/CD  
Workflows

</td>

<td align="center" width="25%">

### Performance

Latency  
Throughput  
Profiling  
Optimization

</td>
</tr>
</table>

---

# `// engineering > hype`

Technology is a tool.

The question I care about is:

> **Does it make the system better?**

```mermaid
flowchart TD

    A["Interesting Technology"] --> B{"Solves a Real Problem?"}

    B -->|No| C["Don't Use It"]
    B -->|Yes| D{"Complexity Worth It?"}

    D -->|No| C
    D -->|Yes| E["Prototype"]

    E --> F{"Measured Improvement?"}

    F -->|No| C
    F -->|Yes| G["Production"]

    style A fill:#18181b,color:#fff,stroke:#7c3aed
    style B fill:#18181b,color:#fff,stroke:#06b6d4
    style C fill:#18181b,color:#fff,stroke:#ef4444
    style D fill:#18181b,color:#fff,stroke:#06b6d4
    style E fill:#18181b,color:#fff,stroke:#f59e0b
    style F fill:#18181b,color:#fff,stroke:#22c55e
    style G fill:#18181b,color:#fff,stroke:#22c55e
```

> **Complexity should be earned.**

---

# `// github`

<div align="center">

<a href="https://github.com/deionx?tab=repositories">
<img src="https://img.shields.io/badge/Explore_My_Repositories-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br />
<br />

<a href="https://github.com/deionx">
<img height="180" src="https://github-readme-stats.vercel.app/api?username=deionx&show_icons=true&hide_border=true&theme=transparent&rank_icon=github" />
</a>

<a href="https://github.com/deionx">
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=deionx&layout=compact&hide_border=true&theme=transparent" />
</a>

<br />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=deionx&hide_border=true&theme=transparent" />

</div>

---

<div align="center">

### DEIONX

`systems` · `software` · `ai` · `automation` · `performance`

<br />

**Make it work. Make it observable. Make it last.**

<br />

⭐ **Build things. Break things. Learn things. Ship things.**

</div>
