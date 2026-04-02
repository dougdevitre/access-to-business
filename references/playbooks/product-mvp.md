# Product & MVP Playbook

## Core Rule
**Ship fast. Learn fast. Kill features that don't serve the core job.**  
The goal of an MVP is to learn, not to impress.

---

## MVP Principles

1. **An MVP is not a bad version of your product.** It's the minimum needed to test your riskiest assumption.
2. **Cut scope until it hurts, then cut more.** If you're not embarrassed by your MVP, you launched too late. (Reid Hoffman)
3. **Build for your first 10 customers, not your first 1,000.**
4. **Manual before automated.** Do it yourself before building software to do it.
5. **Feedback is the product.** Your job is to collect it.

---

## MVP Types (Pick the right one)

| Type | Description | Best For |
|------|-------------|----------|
| Concierge | You do it manually for the customer | Validating demand + process |
| Wizard of Oz | Looks automated, you do it manually | Testing UX without backend |
| Landing page | Describe solution, collect emails | Measuring interest |
| Prototype | Clickable mockup (Figma) | UX validation |
| Piecemeal | Stitch together existing tools | Fast delivery without custom build |
| Single feature | One core feature, nothing else | Focused validation |

---

## Feature Prioritization (ICE Framework)

Score each feature 1–10 on:
- **I**mpact — How much will this move the north star metric?
- **C**onfidence — How sure are we this will work?
- **E**ase — How fast/cheap can we build it?

`ICE Score = (Impact × Confidence × Ease) / 3`

Build highest-scoring features first.

---

## North Star Metric

Your north star metric is the **one number** that best captures value delivered to customers.

| Company Type | Possible North Star |
|-------------|---------------------|
| Marketplace | GMV, transactions |
| SaaS | MRR, WAU, activated users |
| Consumer | DAU, retention D30 |
| Social | Posts created, connections made |
| Productivity | Tasks completed, time saved |

**Choose one. Align the whole team to it. Review weekly.**

---

## Product Roadmap (Startup Format)

Don't build 12-month roadmaps. Build rolling 90-day plans.

```
NOW (this sprint):
- [Feature/fix 1]
- [Feature/fix 2]

NEXT (next 4 weeks):
- [Feature 3]
- [Feature 4]

LATER (90 days):
- [Big bet 1]
- [Big bet 2]

NOT DOING:
- [Thing people ask for but doesn't move NSM]
```

Review and update every 2 weeks.

---

## User Story Format

```
As a [user type],
I want to [action],
So that I can [outcome/benefit].

Acceptance Criteria:
- [ ] Given [context], when [action], then [result]
- [ ] Edge case: [X]
```

---

## Sprint Structure (2-week cycle)

| Day | Activity |
|-----|----------|
| Mon (Week 1) | Sprint planning — what ships by Friday of week 2? |
| Tue–Fri (Week 1) | Build |
| Mon (Week 2) | Mid-sprint check — cut scope if needed |
| Tue–Thu (Week 2) | Build + QA |
| Fri (Week 2) | Ship + demo + retro |

**Retro questions:**
1. What went well?
2. What slowed us down?
3. What do we change next sprint?

---

## Product Metrics to Track Weekly

| Metric | Why It Matters |
|--------|---------------|
| Activation rate | % of new users who complete core action |
| Retention (D7, D30) | Are users coming back? |
| Feature adoption | Are people using what you built? |
| Bug reports | Quality signal |
| NPS / CSAT | Satisfaction signal |
| Time to value | How fast do users get the first win? |

---

## Common Product Mistakes

| Mistake | Fix |
|---------|-----|
| Building what users say they want (not what they need) | Watch behavior, not just feedback |
| Too many features | Kill the bottom 30% of features quarterly |
| Shipping without talking to users | Minimum 2 customer calls per sprint |
| Optimizing before PMF | Focus on retention, not performance |
| Ignoring churn | Churn is the most honest signal you have |
| Building for edge cases | Build for the core 80% use case |

---

## Tools (Free / Low Cost Tier)

| Category | Tool |
|----------|------|
| Wireframing | Figma (free) |
| Project tracking | Linear, Notion, GitHub Projects |
| User feedback | Typeform, Tally |
| Analytics | Mixpanel (free tier), PostHog (open source) |
| Session replay | Hotjar, FullStory |
| Feature flags | Flagsmith (open source), LaunchDarkly |
| Error tracking | Sentry (free tier) |
