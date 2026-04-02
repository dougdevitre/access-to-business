# Access to Business

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](CHANGELOG.md)
[![Pillar](https://img.shields.io/badge/Access%20To-Pillar%207-purple.svg)](https://github.com/dougdevitre)

**AI-powered startup coach, execution engine, pitch generator, and investor binder builder.**

Part of the [Access To](https://github.com/dougdevitre) open-source civic tech initiative.

> [Getting Started Guide](GETTING_STARTED.md) | [Architecture](docs/architecture.md) | [Contributing](CONTRIBUTING.md) | [Changelog](CHANGELOG.md)

---

## What It Does

Access to Business is a Claude AI skill that acts as a hands-on startup coach. It doesn't just advise — it builds with you. Every session ends with something shipped: a draft, a template, a pitch, a metric, a decision.

**For founders at any stage:**
- **Stage 0 (Idea):** Validate before building
- **Stage 1 (Pre-Revenue):** Get your first 10 customers
- **Stage 2 (Early Revenue):** Build repeatability
- **Stage 3 (Growth):** Systems, capital, and scale
- **Stage 4 (Scaling):** Efficiency and team

## Architecture

```mermaid
graph TD
    A[Access to Business] --> B[Execution Coaching]
    A --> C[Investor Binder]
    A --> D[Pitch Generator]
    A --> E[Financial Tools]
    A --> F[Sales & GTM]
    A --> G[Legal & Compliance]
    A --> H[Templates Library]
    A --> I[Regional Ecosystems]

    B --> B1["/start /focus /sprint /recover"]
    C --> C1[17-Section Binder + Scoring]
    D --> D1[Scripts / Deck / One-Sheets / Copy]
    E --> E1[Burn Rate / Runway / Unit Economics]
    F --> F1[Outreach / ICP / Pipeline]
    G --> G1[Formation / Contracts / HIPAA / SOC2]
    H --> H1[100+ Templates across 11 Categories]
    I --> I1[State-Specific Resources]

    style A fill:#2563eb,stroke:#1e40af,color:#fff
    style B fill:#7c3aed,stroke:#6d28d9,color:#fff
    style C fill:#7c3aed,stroke:#6d28d9,color:#fff
    style D fill:#7c3aed,stroke:#6d28d9,color:#fff
    style E fill:#7c3aed,stroke:#6d28d9,color:#fff
    style F fill:#7c3aed,stroke:#6d28d9,color:#fff
    style G fill:#7c3aed,stroke:#6d28d9,color:#fff
    style H fill:#7c3aed,stroke:#6d28d9,color:#fff
    style I fill:#7c3aed,stroke:#6d28d9,color:#fff
```

## Startup Stage Progression

```mermaid
graph LR
    S0[Stage 0\nIdea] --> S1[Stage 1\nPre-Revenue]
    S1 --> S2[Stage 2\nEarly Revenue]
    S2 --> S3[Stage 3\nGrowth]
    S3 --> S4[Stage 4\nScaling]

    S0 -.- V[Validate before building]
    S1 -.- C[Get first 10 customers]
    S2 -.- R[Build repeatability]
    S3 -.- G[Systems capital scale]
    S4 -.- E[Efficiency and team]

    style S0 fill:#fbbf24,stroke:#d97706,color:#000
    style S1 fill:#fb923c,stroke:#ea580c,color:#000
    style S2 fill:#f87171,stroke:#dc2626,color:#fff
    style S3 fill:#a78bfa,stroke:#7c3aed,color:#fff
    style S4 fill:#2563eb,stroke:#1e40af,color:#fff
```

## Repository Structure

```mermaid
graph TD
    ROOT[access-to-business] --> SKILL[SKILL.md\nRouter + Core Logic]
    ROOT --> README_F[README.md]
    ROOT --> REF[references]
    ROOT --> APPS[apps]
    ROOT --> EVALS[evals]

    REF --> CMD[commands]
    REF --> PB[playbooks]
    REF --> PT[pitch]
    REF --> TMP[templates]
    REF --> CMP[compliance]
    REF --> CTR[contracts]
    REF --> ACC[accounting]
    REF --> IP_D[ip]
    REF --> RGN[regional]

    CMD --> CMD1[session / binder / ops]
    PB --> PB1[11 startup playbooks]
    PT --> PT1[5 pitch modules]
    TMP --> TMP1[11 template categories]
    CMP --> CMP1[HIPAA / SOC2 / GDPR / PCI]
    CTR --> CTR1[SaaS / MSA / DPA / NDA]
    ACC --> ACC1[Bookkeeping / Tax / CPA]
    IP_D --> IP1[Patents / TM / Trade Secrets]
    RGN --> RGN1[Missouri + state template]

    style ROOT fill:#2563eb,stroke:#1e40af,color:#fff
    style REF fill:#7c3aed,stroke:#6d28d9,color:#fff
```

## Key Capabilities

| Area | What You Get |
|------|-------------|
| **Execution Coaching** | Slash commands (`/start`, `/focus`, `/sprint`, `/recover`) that keep you moving |
| **Investor Binder** | Full 17-section binder build system with scoring and templates |
| **Pitch Generator** | Verbal pitch scripts, deck design system, one-sheets, marketing copy |
| **Financial Tools** | Burn rate, runway, unit economics, financial model scaffolding |
| **Sales & GTM** | Cold outreach, ICP builder, objection handling, pipeline management |
| **Legal & Compliance** | Entity formation guides, contract templates, HIPAA/SOC2/GDPR frameworks |
| **Templates** | 100+ copy-paste-ready templates across 11 categories |
| **Regional Ecosystems** | State-specific accelerators, grants, legal resources, formation guides |

## Install

### Claude.ai (Recommended)
1. Download the latest `.skill` file from [Releases](https://github.com/dougdevitre/access-to-business/releases)
2. Go to **Claude.ai → Settings → Skills**
3. Upload the `.skill` file

### Manual
1. Clone this repo into your Claude skill directory
2. The `SKILL.md` file will be automatically detected

## Quick Start

Just type one of these to get started:
- `/start` — Full onboarding
- `/help` — See all commands
- `/focus [topic]` — Lock into one task
- `/sprint [topic]` — 60-min deep work session
- `/binder` — Start building your investor binder
- `/pitch` — Draft your pitch

## The Access To Family

| Pillar | Repo | Focus |
|--------|------|-------|
| 1 | [access-to-justice](https://github.com/dougdevitre/access-to-justice) | Legal aid navigation |
| 2 | [access-to-education](https://github.com/dougdevitre/access-to-education) | K-12 standards & educator tools |
| 3 | [access-to-housing](https://github.com/dougdevitre/access-to-housing) | Real estate intelligence |
| 4 | [access-to-services](https://github.com/dougdevitre/access-to-services) | Social services navigation |
| 5 | [access-to-peace](https://github.com/dougdevitre/access-to-peace) | Conflict resolution |
| 6 | [access-to-safety](https://github.com/dougdevitre/access-to-safety) | Domestic violence resources |
| **7** | **access-to-business** | **Startup coaching & execution** |

## State Deployment

This skill is designed for state-level deployment. Missouri is the reference implementation.

To deploy for your state:
1. Copy `references/regional/missouri.md`
2. Replace with your state's ecosystem data
3. Submit a PR

See `references/regional/README.md` for the full guide.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT — see [LICENSE](LICENSE) for details.

---

**Built by [Doug DeVitre](https://github.com/dougdevitre) | Part of the Access To Initiative**
