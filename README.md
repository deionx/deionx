<!--
  README.md — deionx profile
  Paste this into the repository named `deionx`
-->

# DEIONX

<!-- Inline full wordmark SVG (keeps README self-contained and crisp) -->
<!-- File: assets/deionx-wordmark.svg (optional) -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 300" width="100%" height="120" role="img" aria-label="deionx logo">
  <defs>
    <linearGradient id="g1" x1="0" x2="1">
      <stop offset="0" stop-color="#6C63FF"/>
      <stop offset="0.5" stop-color="#00E0FF"/>
      <stop offset="1" stop-color="#00FFA3"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <style>
      .brand { font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; font-weight: 800; letter-spacing: -1px; }
      .tag { font-family: Inter, system-ui, Roboto, Arial; font-weight: 600; font-size: 28px; fill:#9aa0b4; }
    </style>
  </defs>

  <rect width="100%" height="100%" fill="transparent"/>

  <g transform="translate(40,20)">
    <rect x="0" y="0" width="220" height="220" rx="28" fill="url(#g1)" opacity="0.12"/>
    <g transform="translate(24,24)" filter="url(#glow)">
      <text x="18" y="120" font-size="110" fill="url(#g1)" font-weight="900" font-family="Inter, Arial" style="letter-spacing:2px">DX</text>
    </g>
  </g>

  <g transform="translate(320,140)">
    <text class="brand" x="0" y="0" font-size="86" fill="#0f1724">deion</text>
    <text class="brand" x="360" y="0" font-size="86" fill="url(#g1)">x</text>
    <text class="tag" x="0" y="60">Full‑stack Engineer • Systems Architect</text>
  </g>
</svg>

---

### About

**Deionx** — Full‑stack engineer and systems architect focused on high‑performance systems, delightful frontends, and developer experience. I build production‑grade APIs, modular design systems, and automation that scales. My work is pragmatic, measurable, and crafted for long‑term velocity.

**Core strengths**
- **System Design**: resilient, observable, and cost‑efficient architectures  
- **Frontend Engineering**: fast, accessible, componentized UI with great DX  
- **Automation**: CI/CD, infra as code, release pipelines, and developer tooling  
- **Performance**: p95/p99 optimization, microbenchmarks, and real user metrics

---

### Tech Stack

**Languages**  
`TypeScript` • `Python` • `Rust` • `Go`

**Frontend**  
`React` • `Next.js` • `Tailwind CSS` • `Vite`

**Backend**  
`Node.js` • `FastAPI` • `gRPC` • `Postgres`

**Infra & Observability**  
`Docker` • `Kubernetes` • `Terraform` • `Prometheus` • `Grafana` • `OpenTelemetry`

---

### Killer Assets

**Compact monogram SVG** (use as avatar, favicon, or app icon)

```svg
<!-- deionx compact monogram -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 300 300" width="160" height="160" role="img" aria-label="deionx monogram">
  <defs>
    <radialGradient id="rg" cx="30%" cy="20%">
      <stop offset="0" stop-color="#00E0FF"/>
      <stop offset="0.6" stop-color="#6C63FF"/>
      <stop offset="1" stop-color="#8A00FF"/>
    </radialGradient>
    <filter id="soft" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="6" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      .mono { font-family: Inter, system-ui, Roboto, Arial; font-weight: 900; fill: white; }
    </style>
  </defs>

  <rect width="100%" height="100%" rx="36" fill="url(#rg)"/>
  <g transform="translate(0,0)" filter="url(#soft)">
    <path d="M90 210 L90 90 C90 70 110 60 130 60 L190 60 C210 60 230 80 230 100 L230 200 C230 220 210 240 190 240 L130 240 C110 240 90 230 90 210 Z" fill="rgba(0,0,0,0.12)"/>
  </g>

  <text x="50%" y="56%" class="mono" font-size="120" text-anchor="middle" dominant-baseline="middle">DX</text>
  <circle cx="240" cy="60" r="10" fill="#00FFA3" opacity="0.95"/>
</svg>
