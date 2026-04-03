# LLC vs C-Corp vs S-Corp

A structured decision flowchart to help you choose the right business entity for your situation.

## Decision Flowchart

```mermaid
graph TD
    START([What entity type<br/>should I choose?]) --> Q1{Are you raising or<br/>planning to raise<br/>venture capital?}

    Q1 -->|Yes| CCORP_DE[C-Corp<br/>Delaware]
    Q1 -->|No| Q2{How many<br/>founders/owners?}

    Q2 -->|Solo| Q3{Do you expect<br/>annual profits over<br/>$50K in year 1-2?}
    Q2 -->|2+| Q4{Will all owners<br/>be active in<br/>the business?}

    Q3 -->|Yes| Q5{Do you want to<br/>minimize self-employment<br/>tax?}
    Q3 -->|No| LLC_HOME[LLC<br/>Home State]

    Q5 -->|Yes| SCORP[S-Corp Election<br/>Home State]
    Q5 -->|No| LLC_HOME

    Q4 -->|Yes| Q6{Do you expect<br/>significant profits<br/>in years 1-2?}
    Q4 -->|No, some are passive| Q7{Are passive owners<br/>accredited investors?}

    Q6 -->|Yes| Q8{Will you need<br/>different share classes<br/>or complex equity splits?}
    Q6 -->|No| LLC_MULTI[Multi-Member LLC<br/>Home State]

    Q8 -->|Yes| CCORP_HOME[C-Corp<br/>Home State]
    Q8 -->|No| SCORP

    Q7 -->|Yes| CCORP_HOME
    Q7 -->|No| LLC_MULTI

    style CCORP_DE fill:#bbdefb,stroke:#1565c0,color:#0d47a1
    style CCORP_HOME fill:#bbdefb,stroke:#1565c0,color:#0d47a1
    style LLC_HOME fill:#c8e6c9,stroke:#2e7d32,color:#1b5e20
    style LLC_MULTI fill:#c8e6c9,stroke:#2e7d32,color:#1b5e20
    style SCORP fill:#fff9c4,stroke:#f9a825,color:#f57f17
```

## Comparison Table

| Factor | LLC | S-Corp | C-Corp |
|---|---|---|---|
| **Best for** | Solo founders, small teams, service businesses | Profitable small businesses wanting tax savings | VC-backed startups, companies planning to go public |
| **Taxation** | Pass-through (profits taxed on personal return) | Pass-through with salary/distribution split | Double taxation (corporate tax + dividend tax) |
| **Self-employment tax** | All profits subject to SE tax | Only salary subject to SE tax; distributions are not | Not applicable (you are an employee) |
| **Investor compatibility** | Difficult for institutional investors | Limited to 100 shareholders, US citizens only | Preferred by all investor types |
| **Equity flexibility** | Membership interest percentages | Single class of stock only | Multiple classes (common, preferred, etc.) |
| **Administrative burden** | Minimal | Moderate (payroll required) | High (board meetings, minutes, annual reports) |
| **Formation cost** | $50--$500 | $50--$500 + S-election filing | $300--$1,500 (Delaware: ~$400 + registered agent) |
| **Ongoing cost** | $0--$800/year (state fees) | $1,000--$3,000/year (payroll + filings) | $1,000--$5,000/year (Delaware franchise tax + filings) |

## End States Explained

### LLC (Home State)

The simplest and most flexible entity for most small businesses. An LLC provides liability protection without the administrative overhead of a corporation.

**Choose this when:**
- You are a solo founder or small team
- You are not raising institutional capital
- Your revenue is under $50K/year or you are pre-revenue
- You want maximum simplicity

**Key details:**
- Formed in your home state (where you live and operate)
- Taxed as a disregarded entity (solo) or partnership (multi-member)
- No requirement for payroll, board meetings, or corporate minutes
- Can always convert to a C-Corp later if you raise funding

### S-Corp (Home State)

An S-Corp is not a separate entity type. It is a tax election that an LLC or corporation can make. The primary benefit is reducing self-employment tax on profits above a reasonable salary.

**Choose this when:**
- Your business is consistently profitable ($50K+ annually)
- You want to split income between salary and distributions
- You have no plans to raise venture capital
- You are a US citizen or permanent resident

**Key details:**
- You must pay yourself a "reasonable salary" and run payroll
- Distributions above salary are not subject to self-employment tax
- Limited to 100 shareholders, all must be US persons
- Only one class of stock allowed
- The tax savings typically become meaningful at $50K+ in annual profit

**Example:** If your LLC earns $120K in profit, you pay ~15.3% self-employment tax on all of it (~$18,360). With an S-Corp election and a $70K salary, you pay SE tax only on the salary (~$10,710) and take the remaining $50K as a distribution. Savings: ~$7,650/year.

### C-Corp (Delaware)

The standard structure for venture-backed startups. Delaware is the default jurisdiction because of its well-established corporate law, specialized business court, and investor familiarity.

**Choose this when:**
- You are raising or plan to raise venture capital
- You need multiple classes of stock (common for founders, preferred for investors)
- You are building a company with the goal of a large exit or IPO
- You want to issue stock options through a formal equity incentive plan

**Key details:**
- Delaware formation, but you will also need to register as a foreign corporation in your home state
- Requires a registered agent in Delaware (~$100--$300/year)
- Delaware franchise tax ($400--$200K/year depending on structure)
- Annual board meetings and corporate minutes required
- Double taxation: corporate income taxed at 21%, dividends taxed again on personal returns
- The double taxation issue is largely irrelevant for startups reinvesting all revenue into growth

---

## Decision Points Explained

### Are you raising venture capital?

If yes, stop here. VCs require C-Corps (almost always Delaware) because they need preferred stock, pro-rata rights, and a familiar legal framework. Trying to raise VC into an LLC will waste months and legal fees.

### Do you expect significant profits early?

If your business will be profitable quickly (consulting, SaaS with early customers, e-commerce), an S-Corp election can save thousands in self-employment taxes. If you are burning cash and reinvesting everything, the S-Corp benefit does not apply.

### Will you need different share classes?

If you need to give different rights to different owners (voting vs non-voting, preferred returns, vesting schedules), a C-Corp provides the most flexibility. LLCs can do some of this via operating agreements, but it gets complex.

---

## Common Mistakes

1. **Incorporating in Delaware when you do not need to.** If you are not raising VC, Delaware adds cost and complexity for no benefit. Form in your home state.
2. **Skipping the operating agreement.** Even a single-member LLC needs an operating agreement. Without one, you risk losing your liability protection.
3. **Electing S-Corp too early.** If your business is not yet profitable, the payroll costs of an S-Corp outweigh the tax savings.
4. **Choosing C-Corp for the QSBS exclusion alone.** The Qualified Small Business Stock tax exclusion is valuable, but it has strict requirements. Do not structure your company around a tax benefit you may not qualify for.
5. **Not consulting a CPA.** Entity selection has significant tax implications. A one-hour consultation with a CPA ($150--$300) can save you thousands.

---

> **Disclaimer:** This flowchart is for educational purposes only. Entity selection depends on your specific tax situation, state laws, and business goals. Consult a qualified attorney and CPA before forming your business entity.
