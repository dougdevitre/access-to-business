# Commands Directory

## Command Routing

```mermaid
graph TD
    USER[User types /command] --> ROUTER{Route by command type}

    ROUTER --> SESSION[Session & Flow\nsession-commands.md]
    ROUTER --> BINDER[Binder & Fundraising\nbinder-commands.md]
    ROUTER --> OPS[Ops Sales & Coaching\nops-commands.md]

    SESSION --> S1[/start]
    SESSION --> S2[/focus]
    SESSION --> S3[/sprint]
    SESSION --> S4[/recover /decide /energy /help]

    BINDER --> B1[/binder /score]
    BINDER --> B2[/pitch /deck]
    BINDER --> B3[/exec /ask /dataroom /update /simulate]

    OPS --> O1[/metrics /runway /burn /uniteconomics]
    OPS --> O2[/outreach /followup /objection /icp]
    OPS --> O3[/status /blockers /wins /next /pivot]

    style USER fill:#2563eb,stroke:#1e40af,color:#fff
    style ROUTER fill:#f59e0b,stroke:#d97706,color:#000
    style SESSION fill:#22c55e,stroke:#16a34a,color:#fff
    style BINDER fill:#7c3aed,stroke:#6d28d9,color:#fff
    style OPS fill:#3b82f6,stroke:#2563eb,color:#fff
```

## Files in This Directory

| File | Commands | Purpose |
|------|----------|---------|
| `session-commands.md` | `/start` `/focus` `/sprint` `/recover` `/decide` `/energy` `/help` | Session flow and founder energy management |
| `binder-commands.md` | `/binder` `/score` `/pitch` `/deck` `/exec` `/ask` `/dataroom` `/update` `/simulate` | Investor binder building and fundraising prep |
| `ops-commands.md` | `/metrics` `/runway` `/burn` `/uniteconomics` `/model` `/outreach` `/followup` `/objection` `/icp` `/position` `/status` `/blockers` `/wins` `/next` `/pivot` `/validate` `/hire` `/cofounder` `/proposal` | Operations, sales, and startup coaching |

## 35+ Commands Total

The skill provides over 35 slash commands organized into three groups. If unsure which file to load, start with `session-commands.md` and use `/help`.
