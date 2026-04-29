# Full Case Example: B2B SaaS Mid-Market Expansion

## User prompt

> "Should our B2B SaaS company expand into the mid-market segment?"

## Response (Full Case mode)

### Step 1: Context check

*Provisional assumptions [A] (correct any that are wrong and I'll restructure):*
- Decision-maker: CEO
- Success metric: $5M ARR from mid-market within 18 months
- Scope: moving upmarket from current SMB base ($15K ACV → $50–200K ACV); budget envelope ~5–8 hires

Proceeding on these.

### Step 2: Structure (MECE Issue Tree)

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 920 480" font-family="Inter, sans-serif">
  <rect width="920" height="480" fill="#0f172a"/>
  <rect x="340" y="20" width="240" height="50" rx="8" fill="#1e293b" stroke="#f59e0b" stroke-width="2"/>
  <text x="460" y="50" text-anchor="middle" font-size="13" font-weight="600" fill="#f8fafc">Should we expand into mid-market?</text>

  <line x1="460" y1="70" x2="120" y2="120" stroke="#475569"/>
  <line x1="460" y1="70" x2="350" y2="120" stroke="#475569"/>
  <line x1="460" y1="70" x2="580" y2="120" stroke="#475569"/>
  <line x1="460" y1="70" x2="800" y2="120" stroke="#475569"/>

  <rect x="20" y="120" width="200" height="40" rx="6" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="120" y="145" text-anchor="middle" font-size="11" fill="#93c5fd">1. Market attractiveness</text>
  <rect x="250" y="120" width="200" height="40" rx="6" fill="#1e293b" stroke="#f59e0b" stroke-width="1.5"/>
  <text x="350" y="145" text-anchor="middle" font-size="11" fill="#fcd34d">2. Right to win (priority)</text>
  <rect x="480" y="120" width="200" height="40" rx="6" fill="#1e293b" stroke="#f59e0b" stroke-width="1.5"/>
  <text x="580" y="145" text-anchor="middle" font-size="11" fill="#fcd34d">3. Economic model (priority)</text>
  <rect x="700" y="120" width="200" height="40" rx="6" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="800" y="145" text-anchor="middle" font-size="11" fill="#93c5fd">4. Execution risk</text>

  <text x="120" y="195" text-anchor="middle" font-size="10" fill="#cbd5e1">TAM · growth · competition</text>
  <text x="350" y="195" text-anchor="middle" font-size="10" fill="#cbd5e1">Product fit · sales motion · diff</text>
  <text x="580" y="195" text-anchor="middle" font-size="10" fill="#cbd5e1">LTV/CAC · investment · cannibalization</text>
  <text x="800" y="195" text-anchor="middle" font-size="10" fill="#cbd5e1">Timeline · talent · culture</text>

  <text x="460" y="250" text-anchor="middle" font-size="10" fill="#64748b">Amber border = priority branch · gray text = sub-questions</text>
</svg>
```

### Step 3: Hypothesize

| # | Hypothesis | Kill test | Priority |
|---|-----------|-----------|----------|
| H1 | Mid-market TAM is >$500M and growing >15%/yr | Industry report or bottom-up sizing shows <$200M | High |
| H2 | Our product covers 70%+ of mid-market requirements today | Customer interviews reveal 3+ must-have features we lack | **Highest** |
| H3 | Mid-market LTV/CAC > 3x with 18-month payback | Financial model shows payback >24 months | High |
| H4 | We can hire 3 enterprise AEs within 6 months | Recruiting pipeline has <10 qualified candidates | Medium |

Lead with H2 — if the product doesn't fit, nothing else matters.

### Step 4: Analyze

**H2 — Product fit** (priority)
- [F] Current product handles workflow automation for teams of 5–20. Mid-market buyers typically have 50–200 users per account. *(product analytics, Q4 usage data)*
- [F] Top 3 feature gaps from mid-market prospects who evaluated us in 2025: SSO/SAML, audit logs, role-based permissions. *(CRM loss-reason analysis, n=23 lost deals)*
- [I] SSO and audit logs are 2–3 month engineering efforts each. RBAC is a deeper architectural change, estimated 4–6 months. *(eng team estimates)*
- [A] 70% of mid-market buyers would accept RBAC in v2 if SSO + audit ship in v1. **Confidence: 55%** — biggest unknown.

**H1 — Market size**
- [F] Gartner sizes our category at $12B total, with mid-market representing ~30% = $3.6B. *(Gartner 2025 Market Guide)*
- [E] At 0.15% penetration (conservative for a challenger), achievable market = $5.4M ARR. Aligns with the $5M target. *(TAM × penetration benchmark)*
- [F] Category growing 22% YoY overall; mid-market segment growing 28%. *(same Gartner report)*

**H3 — Unit economics**
- [F] Current SMB metrics: ACV $15K, CAC $8K, gross margin 78%, logo churn 18%/yr. *(finance team)*
- [E] Mid-market ACV of $80K (midpoint) with estimated CAC of $40K (2 AE touches + SE + 90-day cycle) yields LTV/CAC of ~4.2x assuming 10% logo churn.
- [A] 10% logo churn is achievable if we staff dedicated CSMs (1:15 ratio). **Confidence: 65%.**

**H4 — Talent**
- [F] Current sales team: 12 SMB AEs, avg deal size $15K, 30-day cycle. Zero enterprise experience on the team. *(VP Sales)*
- [A] We need 3 net-new AEs with enterprise backgrounds, not promoted SMB reps. Hiring timeline: 3–4 months. **Confidence: 70%.**

### Step 5: Synthesize (Pyramid Principle)

**BOTTOM LINE:** Yes, expand into mid-market — but sequence it as a gated $400K pilot tied to product gates, not a big-bang launch.

**SUPPORTING ARGUMENTS:**
1. **Market is there and growing** — $3.6B mid-market TAM growing 28% YoY; $5M ARR requires only 0.15% penetration. *[F, Gartner 2025]*
2. **Product gap is closable** — SSO + audit logs (6 months) unlock 70% of buyers; RBAC (4–6 months more) unlocks the rest. *[I, derived from CRM loss-reason analysis n=23]*
3. **Economics work at mid-market ACV** — LTV/CAC ~4.2x at $80K ACV vs SMB's 3.1x today. *[E, 65% confidence on 10% churn assumption]*
4. **Execution requires new muscle, not promotion** — enterprise AEs and dedicated CSMs are a hiring exercise *and* a culture shift. *[A, 70% confidence]*

**RISKS:**
1. **Product gap on RBAC** — likelihood: M, impact: H, mitigation: run 5 design-partner conversations in month 1 to validate whether RBAC can ship in v2 or must be in v1.
2. **Cannibalization of SMB economics** — likelihood: M, impact: M, mitigation: cap initial hire at 3 AEs; don't scale until 2 of 3 hit quota in Q1.
3. **Culture clash** — likelihood: H, impact: M, mitigation: redesign comp plans for 90-day cycles; explicit "two motions" framing in all-hands.

**KILL CONDITIONS:**
1. **3+ must-have features missing** — if design-partner interviews surface a fourth blocker beyond SSO/audit/RBAC, recommendation flips to "delay 12 months and rebuild platform first."
2. **Enterprise AE pipeline <10 qualified candidates by week 8** — if we can't hire the muscle, the rest doesn't matter; flips to "delay" or "acquihire."
3. **Mid-market churn >15% in pilot cohort** — kills the $80K-ACV economics; flips to "stay SMB and raise prices."

**NEXT ACTIONS:**
1. **VP Product** — commission RBAC scoping study, deliver go/no-go in 2 weeks; success metric: scoping doc + eng cost estimate signed by CTO.
2. **VP Sales** — begin recruiting 3 enterprise AEs immediately; first hire in 8 weeks; success metric: 1 signed offer.
3. **CEO** — approve $400K bridge budget for mid-market pilot (3 AEs + 1 SE + SSO/audit eng sprint); success metric: budget allocated by end of week 1.
4. **VP Product + CEO** — run 5 mid-market design-partner conversations weeks 1–4; success metric: validated answer on whether RBAC must ship in v1.

**OPEN QUESTIONS:**
- Is the 10% mid-market churn assumption realistic for our category? Need 3 reference customers from comparable SaaS companies.
- Will SMB sales reps churn if they perceive mid-market as "the new path to comp"? Need turnover signal in months 1–3.
- What's the integration burden for mid-market buyers' existing identity providers (Okta, Azure AD)? Need pilot data.

### Step 5b: Devil's Advocate

**Strongest counter-argument:** "You're a $15K-ACV company trying to sell $80K deals. That's not a segment expansion — it's a different business. Sales motion, support model, product architecture, and culture all need to change. History says most SMB companies that try to move upmarket end up stuck in the middle: too expensive for SMB, too immature for mid-market."

**Why the recommendation still holds:** the counter-argument is exactly why this is a gated pilot, not a full pivot. The $400K bridge buys 6 months of signal across the three kill conditions above. The asymmetry favors trying: upside is $5M+ ARR at materially better unit economics; downside is one quarter of burn on a falsified experiment with three pre-committed kill points.
