# Should I Raise Funding?

A structured decision flowchart to help you determine whether to bootstrap, raise a small round, or pursue a full venture raise.

## Decision Flowchart

```mermaid
graph TD
    START([Do you need external capital?]) --> Q1{Do you need capital<br/>to grow?}

    Q1 -->|No| Q1A{Are you profitable<br/>or close to it?}
    Q1A -->|Yes| BOOTSTRAP[Bootstrap]
    Q1A -->|No| Q1B{Can you get to<br/>revenue quickly?}
    Q1B -->|Yes| BOOTSTRAP
    Q1B -->|No| Q2

    Q1 -->|Yes| Q2{Can you bootstrap<br/>with revenue or savings?}

    Q2 -->|Yes, comfortably| Q2A{Would capital<br/>accelerate your timeline<br/>by 6+ months?}
    Q2A -->|No| BOOTSTRAP
    Q2A -->|Yes| Q3

    Q2 -->|No| Q3{Is your market<br/>winner-take-all?}

    Q3 -->|Yes| Q4{Do you have<br/>meaningful traction?}
    Q3 -->|No| Q3A{Can you start smaller<br/>and self-fund the MVP?}
    Q3A -->|Yes| BOOTSTRAP
    Q3A -->|No| Q5A

    Q4 -->|Yes| Q5{Are you ready<br/>for dilution and<br/>loss of control?}
    Q4 -->|No| NOTREADY[Not Ready Yet]

    Q5 -->|Yes| Q6{Do you need<br/>more than $500K?}
    Q5 -->|No| Q5A{Would a smaller check<br/>from angels solve<br/>your problem?}

    Q5A -->|Yes| SMALL[Raise a Small Round]
    Q5A -->|No| NOTREADY

    Q6 -->|Yes| FULL[Raise a Full Round]
    Q6 -->|No| SMALL

    style BOOTSTRAP fill:#c8e6c9,stroke:#2e7d32,color:#1b5e20
    style SMALL fill:#fff9c4,stroke:#f9a825,color:#f57f17
    style FULL fill:#bbdefb,stroke:#1565c0,color:#0d47a1
    style NOTREADY fill:#ffcdd2,stroke:#c62828,color:#b71c1c
```

## End States

### Bootstrap
You do not need outside capital right now. This is the strongest position to be in. You retain full ownership, full control, and can move at your own pace. Most successful small businesses never raise a dollar of outside funding.

### Raise a Small Round
An angel round or pre-seed of $50K--$500K from angels, friends-and-family, or a small fund. This gives you runway to prove your concept without the overhead of institutional investors. Typical dilution: 5--15%.

### Raise a Full Round
A seed or Series A from institutional investors ($500K--$5M+). This path makes sense when you have traction, a large market, and need significant capital to capture it. Typical dilution: 15--25% per round.

### Not Ready Yet
You are not in a position to raise effectively. Investors will either say no or offer bad terms. Focus on building traction first, then revisit.

---

## Decision Points Explained

### Do you need capital to grow?

Be honest. Many founders assume they need money when what they actually need is customers. Capital is necessary when:
- You need to build something before you can sell it (hardware, regulated industries)
- Customer acquisition requires significant upfront spend
- You need to hire specialized talent to build the product

Capital is not necessary when:
- You can sell a service first and build the product later
- Your MVP can be built nights-and-weekends
- You are pre-idea and just want a salary

### Can you bootstrap with revenue or savings?

Bootstrapping means funding the business from personal savings, revenue, or a day job. This is viable when:
- You have 6--12 months of personal runway
- You can generate revenue within 3--6 months
- Your burn rate is low (solo founder or small team)

Bootstrapping is not viable when:
- You would go into significant personal debt
- The product requires a large team before generating any revenue
- Your personal financial situation cannot absorb the risk

### Is your market winner-take-all?

Winner-take-all markets have strong network effects or high switching costs. Examples: marketplaces, social networks, infrastructure platforms. In these markets, the first company to reach scale often captures most of the value.

If your market is not winner-take-all, you can grow at a sustainable pace and still build a valuable business. Most markets are not winner-take-all, despite what pitch decks claim.

### Do you have meaningful traction?

Traction means evidence that people want what you are building. This varies by stage:
- **Pre-seed:** Waitlist signups, letters of intent, pilot customers
- **Seed:** Revenue (even small), active users, retention metrics
- **Series A:** Consistent month-over-month growth, clear unit economics

Without traction, you are asking investors to bet on an idea. Some will, but the terms will be worse and the process will be harder.

### Are you ready for dilution and loss of control?

Raising money means selling part of your company. Understand what you are giving up:
- **Equity:** 15--25% per round, compounding over multiple rounds
- **Control:** Board seats, investor approval rights, information obligations
- **Optionality:** Investors expect a large outcome; a $5M exit that would be life-changing for you may be a failure for them

If you are building a lifestyle business or a company you want to run for decades, venture capital is likely the wrong tool.

---

## Common Mistakes

1. **Raising because everyone else is.** Fundraising is not a milestone. It is a tool.
2. **Raising too early.** Pre-traction raises mean maximum dilution for minimum leverage.
3. **Raising too much.** More money means higher expectations and a higher bar for the next round.
4. **Raising too little.** Under-funding leads to desperate follow-on raises at bad terms.
5. **Ignoring alternatives.** Revenue-based financing, SBA loans, grants, and accelerators are all options that do not require equity dilution.

---

> **Disclaimer:** This flowchart is for educational purposes only. Fundraising decisions depend on your specific circumstances. Consult a qualified attorney and financial advisor before making financing decisions.
