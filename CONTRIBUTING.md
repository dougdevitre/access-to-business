# Contributing to Access to Business

Thank you for helping make startup coaching more accessible.

```mermaid
flowchart LR
    A["Fork Repo"] --> B["Edit Files"]
    B --> C["Open PR"]
    C --> D["Review"]
    D --> E["Merge"]

    style A fill:#4a90d9,stroke:#2c5f8a,color:#fff
    style B fill:#f5a623,stroke:#c47d10,color:#fff
    style C fill:#7b68ee,stroke:#5a4abf,color:#fff
    style D fill:#e67e22,stroke:#b35e0a,color:#fff
    style E fill:#27ae60,stroke:#1a7a42,color:#fff
```

## How to Contribute

### Report Issues
- Open a GitHub Issue with a clear description
- Include the command or playbook involved
- Describe expected vs. actual behavior

### Add a State Deployment
1. Fork the repo
2. Copy `references/regional/missouri.md` to `references/regional/[your-state].md`
3. Replace all Missouri-specific data with your state's ecosystem
4. Follow the template structure in `references/regional/README.md`
5. Open a PR with the title: `Add regional deployment: [State Name]`

### Improve Playbooks or Templates
1. Fork the repo
2. Edit the relevant file in `references/`
3. Keep the existing structure and formatting conventions
4. Open a PR describing what changed and why

### Add New Templates
1. Determine which template category the new template belongs to
2. Add it to the appropriate file in `references/templates/`
3. Follow the existing template format: title, when to use, the template, notes

### Add Decision Frameworks
1. Create a new file in `references/decisions/` (e.g., `when-to-pivot.md`)
2. Structure as a decision flowchart with clear criteria
3. Include a mermaid diagram showing the decision tree
4. Update the Decision Flowchart Routing table in `SKILL.md`

### Add Integrations Guides
1. Create a new file in `references/integrations/` (e.g., `hubspot-setup.md`)
2. Cover setup, configuration, and common startup use cases
3. Keep instructions step-by-step and tool-version-independent
4. Update the Integrations Routing table in `SKILL.md`

### Add Advisor Tools
1. Add to the appropriate file in `references/advisor/`
2. Focus on diagnostic frameworks, session prep, or portfolio tracking
3. Update the Advisor & Investor Toolkit Routing table in `SKILL.md`

## Style Guidelines

- **Tone:** Calm, direct, practical. No hype.
- **Format:** Use the Task Response Format from SKILL.md for executable content
- **Length:** Keep playbooks under 300 lines. Use progressive disclosure.
- **Templates:** Must be copy-paste ready with clear `[PLACEHOLDER]` markers
- **Legal/Financial:** Always include educational-information disclaimers. Never present as advice.

## Code of Conduct

Be respectful, constructive, and founder-friendly. This project exists to help people
build businesses — contributions should reflect that mission.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
