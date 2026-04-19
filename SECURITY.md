# Security Policy

## Reporting a Vulnerability

If you discover a security issue in Access to Business — for example, a template that could leak secrets, a prompt that could be exploited, or a skill behavior that poses risk to founders using it — please report it privately.

**Do not open a public GitHub issue for security vulnerabilities.**

Instead, contact the maintainer, [Doug DeVitre](https://github.com/dougdevitre), directly via a private GitHub message or through the contact information in his GitHub profile.

Include in your report:
- A clear description of the issue
- Steps to reproduce (prompt, command, or file path)
- Your assessment of the impact
- Any suggested remediation

## What to Expect

- **Acknowledgement** within 5 business days
- **Triage and assessment** within 14 business days
- **Coordinated disclosure** within 90 days of the initial report, or sooner if a fix is available

We follow a coordinated disclosure process: we ask reporters to give us a reasonable window to remediate before publicly disclosing, and we will credit reporters in the release notes unless anonymity is requested.

## Scope

In scope:
- Content in `SKILL.md`, `references/`, `apps/`, and `evals/`
- The GitHub Actions validation workflow
- Templates and playbooks that could expose users to legal, financial, or security risk if followed as written

Out of scope:
- Vulnerabilities in Claude.ai, Claude Code, or other Anthropic products (report those to [Anthropic's security team](https://www.anthropic.com/security))
- Issues in third-party services referenced by templates (e.g., Stripe, Airtable) — report those to the service owner

## Secrets and Credentials

If you find committed secrets (API keys, tokens, credentials) in the repository history, please report privately — **do not** open a public issue. Secrets will be rotated and the history rewritten as appropriate.
