# Full Case Example: B2B SaaS Mid-Market Expansion

## User prompt

> "Should our B2B SaaS company expand into the mid-market segment?"

## Response (Full Case mode)

### Step 1: Clarify (Hard Gate)

Before I structure this, I need to confirm three things:

1. **Decision-maker**: Who approves this -- CEO? Board? VP of Sales?
2. **Success metric**: What does "successful expansion" look like? Revenue target? Number of mid-market logos? Timeframe?
3. **Scope**: Are we evaluating (a) moving upmarket from SMB, (b) moving downmarket from enterprise, or (c) launching a new product for mid-market? And what's the budget envelope?

*User confirms: CEO decides. Success = $5M ARR from mid-market within 18 months. Currently SMB-focused ($15K ACV), mid-market defined as $50-200K ACV. Budget: can hire 5-8 people.*

### Step 2: Structure (MECE Issue Tree)

```
Should we expand into mid-market?
├── 1. Market Attractiveness
│   ├── 1a. Size: How large is the mid-market TAM for our category?
│   ├── 1b. Growth: Is mid-market spending growing faster than SMB?
│   └── 1c. Competition: Who serves mid-market today? How entrenched?
├── 2. Right to Win
│   ├── 2a. Product fit: Can our product serve mid-market needs without a rewrite?
│   ├── 2b. Sales motion: Do we know how to sell $50-200K deals?
│   └── 2c. Differentiation: What do we offer that incumbents don't?
├── 3. Economic Model
│   ├── 3a. Unit economics: LTV/CAC at mid-market ACV
│   ├── 3b. Investment: Upfront cost (product, sales, CS) to reach $5M ARR
│   └── 3c. Cannibalization: Does mid-market pull resources from profitable SMB?
└── 4. Execution Risk
    ├── 4a. Timeline: Can we ship mid-market features in 6 months?
    ├── 4b. Talent: Can we hire enterprise-capable AEs and SEs?
    └── 4c. Culture: Will a mid-market motion clash with our SMB DNA?
```

**Diagram description:** The issue tree would be rendered as an SVG with the root question at the top (amber border), four Level 1 branches in blue (Market Attractiveness, Right to Win, Economic Model, Execution Risk), and their sub-branches as leaf nodes. Branches 2a and 3a would be highlighted in amber as priority hypotheses.

### Step 3: Hypothesize

| # | Hypothesis | Kill test | Priority |
|---|-----------|-----------|----------|
| H1 | Mid-market TAM is >$500M and growing >15%/yr | Industry report or bottom-up sizing shows <$200M | High |
| H2 | Our product covers 70%+ of mid-market requirements today | Customer interviews reveal 3+ must-have features we lack | **Highest** |
| H3 | Mid-market LTV/CAC > 3x with 18-month payback | Financial model shows payback >24 months | High |
| H4 | We can hire 3 enterprise AEs within 6 months | Recruiting pipeline has <10 qualified candidates | Medium |

Lead with H2 -- if the product doesn't fit, nothing else matters.

### Step 4: Analyze

**H2 -- Product fit** (priority)
- [F] Current product handles workflow automation for teams of 5-20. Mid-market buyers typically have 50-200 users per account. [Source: product analytics, Q4 usage data]
- [F] Top 3 feature gaps from mid-market prospects who evaluated us in 2025: SSO/SAML, audit logs, role-based permissions. [Source: CRM loss-reason analysis, n=23 lost deals]
- [I] SSO and audit logs are 2-3 month engineering efforts each. RBAC is a deeper architectural change, estimated 4-6 months. [Derived from eng team estimates]
- [A] 70% of mid-market buyers would accept RBAC in v2 if SSO + audit ship in v1. Confidence: 55% -- this is the biggest unknown.

**H1 -- Market size**
- [F] Gartner sizes our category at $12B total, with mid-market representing ~30% = $3.6B. [Source: Gartner 2025 Market Guide]
- [I] At 0.15% penetration (conservative for a challenger), achievable market = $5.4M ARR. Aligns with the $5M target. [Derived from TAM x penetration benchmark]
- [F] Category growing 22% YoY overall; mid-market segment growing 28%. [Source: same Gartner report]

**H3 -- Unit economics**
- [F] Current SMB metrics: ACV $15K, CAC $8K, gross margin 78%, logo churn 18%/yr. [Source: finance team]
- [I] Mid-market ACV of $80K (midpoint) with estimated CAC of $40K (2 AE touches + SE + 90-day cycle) yields LTV/CAC of ~4.2x assuming 10% logo churn. [Derived from ACV assumption + industry benchmarks for mid-market churn]
- [A] 10% logo churn is achievable if we staff dedicated CSMs (1:15 ratio). Confidence: 65%.

**H4 -- Talent**
- [F] Current sales team: 12 SMB AEs, avg deal size $15K, 30-day cycle. Zero enterprise experience on the team. [Source: VP Sales]
- [A] We need 3 net-new AEs with enterprise backgrounds, not promoted SMB reps. Hiring timeline: 3-4 months. Confidence: 70%.

### Step 5: Synthesize (Pyramid Principle)

**BOTTOM LINE:** Yes, expand into mid-market -- but sequence it as a gated investment, not a big-bang launch.

**SO WHAT:**
1. **The market is there and growing** -- $3.6B mid-market TAM growing 28% YoY gives us a large, expanding target. $5M ARR requires only 0.15% penetration. [F]
2. **Product gap is closable but not trivial** -- SSO + audit logs (ship in 6 months) unlock 70% of buyers [I]. RBAC (4-6 months more) is needed for the remaining 30% [A, 55% confidence].
3. **Economics work at mid-market ACV** -- LTV/CAC of ~4.2x with $80K ACV and 10% churn [I]. Significantly better than SMB's 3.1x, but depends on hitting churn assumption.
4. **Execution requires new muscle** -- need enterprise AEs (not promoted SMB reps) and dedicated CSMs. This is a cultural shift, not just a hiring exercise [A, 70% confidence].

**RISKS & OPEN QUESTIONS:**
- **Product risk (highest):** RBAC confidence is only 55%. If mid-market buyers won't close without it, timeline extends 4-6 months and the 18-month ARR target is at risk. Mitigation: run 5 design-partner conversations in month 1 to validate.
- **Cannibalization risk:** Enterprise AEs are 3-4x more expensive than SMB reps. If mid-market ramp is slow, the burn rate hits SMB profitability. Mitigation: cap initial hire at 3 AEs; don't scale until 2 of 3 hit quota in Q1.
- **Culture risk:** SMB velocity culture (close in 30 days) will clash with 90-day enterprise cycles. Mid-market AEs may feel like second-class citizens if comp plans aren't redesigned.

**NEXT ACTIONS:**
1. **VP Product** -- commission RBAC scoping study, deliver go/no-go in 2 weeks
2. **VP Sales** -- begin recruiting 3 enterprise AEs immediately; target first hire in 8 weeks
3. **CEO** -- approve $400K bridge budget for mid-market pilot (3 AEs + 1 SE + SSO/audit eng sprint)
4. **VP Product + CEO** -- run 5 mid-market design-partner conversations in weeks 1-4 to validate RBAC phasing assumption

### Step 5b: Devil's Advocate

**Strongest counter-argument:** "You're a $15K ACV company trying to sell $80K deals. That's not a segment expansion -- it's a different business. Your sales motion, support model, product architecture, and culture all need to change. History says most SMB companies that try to move upmarket end up stuck in the middle: too expensive for SMB, too immature for mid-market."

**Why the recommendation holds:** The counter-argument is real -- which is exactly why this is a gated pilot, not a full pivot. The $400K bridge buys 6 months of signal. If 2 of 3 AEs close $50K+ deals with SSO-only product, we have proof. If they can't, we've lost $400K and learned something valuable. The asymmetry favors trying: the upside ($5M+ ARR at better unit economics) far exceeds the downside (one quarter of burn on a failed experiment).
