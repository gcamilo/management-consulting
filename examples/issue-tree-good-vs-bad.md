# Issue Tree: Good vs Bad

## Scenario

A mid-size European SaaS company ($40M ARR) is evaluating entry into the US market.

---

## BAD issue tree

```
Should we enter the US market?
├── Market opportunity
│   ├── Is the market big?
│   ├── Is it growing?
│   └── Are there customers?
├── Competition
│   ├── Who are the competitors?
│   └── Are they strong?
├── Risks
│   ├── What could go wrong?
│   └── Is it expensive?
└── Other considerations
    └── Anything else?
```

**What's wrong:**
- **Not MECE.** "Risks" overlaps with every other branch (competition is a risk, cost is a risk). "Other considerations" is a catch-all that signals incomplete thinking.
- **Too generic.** "Is the market big?" applies to any market entry anywhere. Nothing is specific to this company, this product, or the US.
- **No evidence coding.** No indication of what's known vs unknown.
- **No decision path.** Reading the tree doesn't tell you what analysis would actually resolve the question.

---

## GOOD issue tree

```
Should EuroSaaS enter the US market by Q1 2027?
│
├── 1. Is the US TAM large enough to justify the investment?
│   ├── 1a. US segment TAM for our ICP (mid-market logistics, 200-2000 employees)
│   │   └── [F] $2.1B (Gartner 2025), growing 14% CAGR
│   ├── 1b. Realistic SAM given current product-market fit
│   │   └── [I] ~$320M — based on EU win rates applied to US ICP density
│   └── 1c. Revenue target achievable within 24 months?
│       └── [A] $5M ARR target requires 120 customers @ $42K ACV (P=65%)
│
├── 2. Can we win against US incumbents?
│   ├── 2a. Incumbent positioning gaps
│   │   └── [F] Top 3 (Acme, Bolt, Crux) have no native EU compliance module
│   ├── 2b. Switching costs for target customers
│   │   └── [I] Medium — 6-month implementation, but contracts are mostly annual
│   └── 2c. Our differentiation durability (>18 months)
│       └── [A] EU compliance moat holds ~2 years before incumbents build it (P=55%)
│
├── 3. Do we have the right-to-win (capabilities + cost)?
│   ├── 3a. Required investment (GTM team, legal entity, localization)
│   │   └── [F] $2.8M first-year estimate (finance team model, Mar 2026)
│   ├── 3b. Opportunity cost — what EU growth do we forgo?
│   │   └── [I] ~$3M ARR from DACH expansion delayed 12 months
│   └── 3c. Funding runway supports the bet?
│       └── [F] 22 months runway at current burn; entry adds 4 months burn
│
└── 4. Can we execute the entry in time?
    ├── 4a. Hiring — US sales team ramp time
    │   └── [A] 6-month ramp; need Q3 2026 start to hit Q1 2027 (P=70%)
    ├── 4b. Legal/regulatory blockers
    │   └── [F] No federal license required; state-by-state data residency handled
    └── 4c. Partnership channel as accelerant?
        └── [I] 2 US resellers in late-stage discussions (LOI expected May 2026)
```

**What's right:**
- **MECE.** Four branches: market size, competitive position, capability/cost, execution. No overlaps, no gaps.
- **Specific.** Named competitors, dollar figures, timeframes, ICP definition.
- **Evidence-coded.** Every leaf tagged [F]act, [I]nference, or [A]ssumption with confidence.
- **Decision-driving.** Each branch resolves a necessary condition. If any branch fails, the answer is "no" or "not yet."
- **Prioritized.** Branch 1 (TAM) and Branch 3 (cost) are the kill tests — analyze those first.
