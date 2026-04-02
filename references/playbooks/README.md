# Playbooks Directory

## Startup Lifecycle Coverage

```mermaid
graph TD
    IDEA[Stage 0: Idea] --> VAL[validation.md\nCustomer Discovery]
    VAL --> MVP[product-mvp.md\nBuild & Ship]
    MVP --> LEGAL[legal-formation.md\nEntity & Equity]
    LEGAL --> GTM[gtm-sales.md\nGo-to-Market]
    GTM --> MKT[marketing-brand.md\nPositioning & Launch]
    MKT --> METRICS[metrics-finance.md\nBurn Runway Economics]
    METRICS --> TEAM[team-hiring.md\nFirst Hires]
    TEAM --> OPS[operations.md\nSOPs & Systems]
    OPS --> FUND[fundraising.md\nRound Planning]
    FUND --> BINDER[investor-binder.md\n17-Section Binder]
    BINDER --> RESIL[resilience.md\nFounder Psychology]

    RESIL -.-> IDEA

    style IDEA fill:#fbbf24,stroke:#d97706,color:#000
    style VAL fill:#fb923c,stroke:#ea580c,color:#000
    style MVP fill:#f87171,stroke:#dc2626,color:#fff
    style GTM fill:#2563eb,stroke:#1e40af,color:#fff
    style BINDER fill:#7c3aed,stroke:#6d28d9,color:#fff
    style FUND fill:#8b5cf6,stroke:#7c3aed,color:#fff
    style RESIL fill:#22c55e,stroke:#16a34a,color:#fff
```

## Files in This Directory

| File | Focus | Stage |
|------|-------|-------|
| `validation.md` | Customer discovery, assumption mapping, PMF signals | 0-1 |
| `product-mvp.md` | Roadmap, prioritization, shipping fast | 0-1 |
| `legal-formation.md` | Entity, equity, vesting, QSBS, 409A | 1-2 |
| `gtm-sales.md` | Outreach, pipeline, pricing, closing | 1-2 |
| `marketing-brand.md` | Positioning, content, SEO, launch | 1-3 |
| `metrics-finance.md` | Burn, runway, unit economics, financial model | 2-3 |
| `team-hiring.md` | First hire, co-founder, equity, culture | 2-3 |
| `operations.md` | SOPs, automation, tool stack, systems | 2-4 |
| `fundraising.md` | Fundraising strategy and round planning | 2-4 |
| `investor-binder.md` | Full 17-section binder build system + templates | 2-4 |
| `resilience.md` | Founder psychology, rejection, pivots, burnout | All |

## Loading Rule

Load only the playbook relevant to the founder's current stage and topic. Never load all playbooks at once.
