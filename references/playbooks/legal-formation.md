# Legal & Formation Playbook

```mermaid
graph LR
    A[Choose Entity Type] --> B{Raising VC?}
    B -- Yes --> C[Delaware C-Corp]
    B -- No --> D[LLC]
    C --> E[File + EIN + Bank]
    D --> E
    E --> F[Operating / Equity Agreements]
    F --> G[Licenses & Compliance]
    style A fill:#2563eb,stroke:#1e40af,color:#fff
    style B fill:#d97706,stroke:#b45309,color:#fff
    style C fill:#7c3aed,stroke:#5b21b6,color:#fff
    style D fill:#7c3aed,stroke:#5b21b6,color:#fff
    style E fill:#2563eb,stroke:#1e40af,color:#fff
    style F fill:#059669,stroke:#047857,color:#fff
    style G fill:#059669,stroke:#047857,color:#fff
```

**Disclaimer:** This is educational context only — not legal advice. Always consult a licensed attorney for entity formation, equity, and compliance decisions.

---

## Entity Choice

### LLC vs C-Corp

| Factor | LLC | C-Corp (Delaware) |
|--------|-----|-------------------|
| VC fundable | ❌ (VCs typically won't invest) | ✅ |
| Pass-through taxes | ✅ | ❌ (double taxation) |
| QSBS eligibility | ❌ | ✅ |
| Self-employed tax | Higher | Lower at scale |
| Best for | Bootstrapped, lifestyle, services | VC-backed, high-growth |
| Complexity | Lower | Higher |

**Rule of thumb:** If you plan to raise venture capital, form a Delaware C-Corp. If you're bootstrapping or running a services business, Missouri LLC is simpler and cheaper.

---

## Missouri LLC Formation

1. Choose a business name → check availability at sos.mo.gov
2. File Articles of Organization → sos.mo.gov → $50 filing fee
3. Designate a Registered Agent (you, or a service ~$50/yr)
4. Apply for EIN → irs.gov/ein (free, takes 5 minutes online)
5. Open a business bank account (Mercury, Relay, or local bank)
6. Draft an Operating Agreement (not legally required in MO, but critical)
7. Apply for any required business licenses (varies by city/county)

---

## Delaware C-Corp Formation

Options:
- **Stripe Atlas** ($500, fastest) — incorporation + EIN + bank + stock issuance
- **Clerky** ($399+) — startup-optimized, attorney-reviewed docs
- **Gust Launch** (free) — basic formation
- **Attorney** — most control, most expensive ($1,500–$5,000+)

Steps after formation:
1. Issue founder stock (83(b) election required — see below)
2. Assign all IP to the company
3. Set up vesting agreements
4. Open bank account (Mercury recommended for startups)
5. File for EIN if not done through formation service

---

## Equity & Vesting

### Standard Founder Vesting
- **4 years total** with a **1-year cliff**
- Cliff: No stock vests until 12 months in; then 25% vests immediately
- Monthly vesting after cliff: 1/48 per month for remaining 36 months
- **Set this up BEFORE taking any outside money**

### 83(b) Election
- **File within 30 days of receiving restricted stock**
- Tells the IRS you want to be taxed now on the low early value (not later when it's worth more)
- Failure to file = massive tax bill when stock vests
- File with IRS + keep a copy + file with company records
- **This is one of the most costly mistakes founders make. Don't miss it.**

### Employee Equity (Options)
- Standard: 10–15% option pool reserved for employees
- Options vest on the same 4yr/1yr cliff schedule
- Strike price = FMV at grant date (set by 409A valuation)
- **Get a 409A valuation before issuing any options** (required for compliance)

---

## SAFE Note

**Simple Agreement for Future Equity** — not a loan, not equity yet.

Key terms to understand:
- **Valuation cap:** The cap on what valuation it converts at. Lower cap = better for investor.
- **Discount rate:** Converts at a discount to the next round (typically 15–25%)
- **Pro-rata rights:** Right to invest in future rounds to maintain ownership %
- **MFN clause:** If you offer better terms to future investors, early SAFE holders get those terms too

**Use YC's standard postmoney SAFE.** Available free at ycombinator.com/documents. Don't create custom terms early-stage — it spooks investors and costs legal fees.

---

## Convertible Note

Older instrument — a loan that converts to equity. Has:
- Interest rate (typically 5–8%)
- Maturity date (18–24 months)
- Conversion mechanics (cap + discount)

SAFE has largely replaced convertible notes for early-stage. Use SAFE unless investor specifically requests a note.

---

## Co-Founder Agreement Checklist

Before taking any money or writing any code together:

- [ ] Equity split (and rationale — written down)
- [ ] Vesting schedule for all founders
- [ ] IP assignment (all work done for the company belongs to the company)
- [ ] Decision-making authority (who decides what)
- [ ] What happens if a co-founder leaves (buyback rights)
- [ ] Compensation expectations (salary, deferred)
- [ ] Full-time commitment expectations
- [ ] Non-compete / non-solicit scope

**A handshake agreement is not enough. Put it in writing.**

---

## Intellectual Property Basics

- All founders must **assign IP** to the company in writing before the company takes money
- Any code, designs, or inventions created for the company belong to the company
- This is standard in every investor's due diligence checklist — missing IP assignments kill deals
- File provisional patent applications for novel inventions before public disclosure

---

## QSBS (Qualified Small Business Stock)

- **Up to $10 million** in federal capital gains tax exclusion
- Requires: C-Corp, issued at original issuance (not secondary), held 5+ years
- Company must have < $50M in assets at time of issuance
- **One of the most valuable tax benefits for early startup founders and investors**
- Missouri has no equivalent state QSBS benefit (as of 2025)

---

## Key Legal Resources

| Need | Resource |
|------|----------|
| Entity formation | Stripe Atlas, Clerky, sos.mo.gov |
| SAFE / term sheet templates | ycombinator.com/documents |
| Startup-friendly law firms | Cooley, Gunderson, Wilson Sonsini, Bryan Cave (St. Louis) |
| IP assignment templates | Clerky, NVCA model docs |
| 409A valuation | Carta, Pulley, Preferred Return |
| Cap table management | Carta (funded) or LTSE Equity (early stage, free) |
