# CLAUDE.md — Instructions for Claude Code

## Project Overview

Access to Business is an open-source Claude AI skill (Pillar 7 of the Access To civic tech initiative). It acts as a hands-on startup coach, execution engine, pitch generator, and investor binder builder.

## Repository Structure

- `SKILL.md` — Core skill logic and router. Always loaded in context.
- `references/` — Reference files loaded on demand by topic/command.
  - `commands/` — Slash command definitions (session, binder, ops)
  - `playbooks/` — 21 startup playbooks (11 core + 10 specialized, with 8 advanced companions)
  - `pitch/` — 5-module pitch preparation system
  - `templates/` — 11 categories of copy-paste-ready templates
  - `compliance/` — HIPAA, SOC2, GDPR, PCI-DSS, security
  - `contracts/` — SaaS, MSA, DPA, NDA, negotiation
  - `accounting/` — Bookkeeping, tax calendar, CPA guide
  - `ip/` — Patents, trademarks, trade secrets, copyright
  - `advisor/` — Diagnostic frameworks, portfolio tools, session prep
  - `decisions/` — Decision flowcharts (should-i-raise, entity-type, build-vs-buy, when-to-hire)
  - `integrations/` — Stripe setup, Airtable starter bases
  - `regional/` — State-specific deployments (Missouri, California, Texas)
- `apps/` — Self-contained HTML apps (intake, pitch timer, runway calculator, unit economics)
- `evals/` — 80 eval test cases for skill triggering
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

CI runs automatically on push to `main` and on pull requests (`.github/workflows/validate.yml`). It checks:
1. JSON validity (MANIFEST.json, eval-set.json)
2. MANIFEST.json counts match actual files on disk
3. All file paths referenced in SKILL.md exist
4. Eval test case IDs are unique and well-formed
5. Playbook cross-references (markdown links between split files) resolve

Additionally, verify changes by:
1. Reviewing markdown rendering on GitHub
2. Running eval triggers from `evals/eval-set.json` against the skill
3. Checking that mermaid diagrams render correctly
