# CLAUDE.md — Instructions for Claude Code

## Project Overview

Access to Business is an open-source Claude AI skill (Pillar 7 of the Access To civic tech initiative). It acts as a hands-on startup coach, execution engine, pitch generator, and investor binder builder.

## Repository Structure

- `SKILL.md` — Core skill logic and router. Always loaded in context.
- `references/` — Reference files loaded on demand by topic/command.
  - `commands/` — Slash command definitions (session, binder, ops)
  - `playbooks/` — 11 startup lifecycle playbooks
  - `pitch/` — 5-module pitch preparation system
  - `templates/` — 11 categories of copy-paste-ready templates
  - `compliance/` — HIPAA, SOC2, GDPR, PCI-DSS, security
  - `contracts/` — SaaS, MSA, DPA, NDA, negotiation
  - `accounting/` — Bookkeeping, tax calendar, CPA guide
  - `ip/` — Patents, trademarks, trade secrets, copyright
  - `regional/` — State-specific deployments (Missouri is reference)
- `apps/` — Self-contained HTML apps (intake assessment)
- `evals/` — Eval test cases for skill triggering
- `docs/` — Architecture documentation

## Key Conventions

- **Tone:** Calm, direct, practical. No hype.
- **Templates:** Must be copy-paste ready with `[PLACEHOLDER]` markers.
- **Legal/Financial content:** Always include educational-information disclaimers.
- **Playbooks:** Keep under 300 lines. Use progressive disclosure.
- **Reference files:** Never load all at once. Load only when the relevant topic is triggered.

## Common Tasks

- **Adding a state deployment:** Copy `references/regional/missouri.md`, replace data, update SKILL.md routing table.
- **Adding templates:** Add to the appropriate file in `references/templates/`, following existing format.
- **Running evals:** Use `evals/eval-set.json` to verify skill triggering.

## Testing

There are no automated tests. Verify changes by:
1. Reviewing markdown rendering on GitHub
2. Running eval triggers from `evals/eval-set.json` against the skill
3. Checking that mermaid diagrams render correctly
