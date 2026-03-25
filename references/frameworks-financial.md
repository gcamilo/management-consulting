# Financial & Sizing Frameworks — Practitioner Reference

Five frameworks that flow naturally from diagnostic to communication: Profit Tree
(what is wrong?) → Revenue Tree (where is growth?) → TAM/SAM/SOM (how big is the
opportunity?) → Unit Economics (is each customer profitable?) → Waterfall/Bridge
(how do we explain the change?). Use them individually or in sequence for a complete
business analysis.

---

## 1. Profit Tree

**Solves:** Diagnosing *where* profit is being created or destroyed by decomposing it
into mathematical sub-components until you reach actionable operational levers.

**Does NOT solve:** *Why* the number changed (a revenue decline caused by a
competitor's patent does not appear in the tree), or whether the business model
itself is viable.

### When to Use

- "Why did profit decline?" — the classic profitability case
- When aggregate numbers mask opposing movements in sub-components
- When you need to prioritize which lever to fix first
- Comparing performance across time periods, segments, or competitors

**Skip it when:** The question is strategic ("Should we be in this business?") rather
than diagnostic, or you lack granular P&L data.

### Step-by-Step Workflow

1. **Start with the core equation.** Profit = Revenue - Costs. Do not skip this —
   confirm which branch is responsible before drilling down.

2. **Decompose Revenue** by business model:
   - **Product:** Revenue = Avg Price x Units Sold. Units = Customers x Units/Customer.
   - **Subscription:** Revenue = Subscribers x ARPU. Subscribers = New + Retained - Churned.
   - **Multi-product:** Revenue = Sum(Revenue per product line), each decomposed further.
   - **Segment** by channel, geography, or customer type when relevant.

3. **Decompose Costs.**
   - Variable: Cost/Unit x Volume. Break cost/unit into components (materials, labor,
     shipping, processing).
   - Fixed: Rent, salaries (non-production), depreciation, R&D, SG&A.
   - Alternative: COGS vs OpEx vs Non-operating. Choose the decomposition matching
     how the company actually tracks costs.

4. **Customize to the business.** A generic tree is a starting point, not a deliverable.
   An airline's cost tree (fuel, labor, aircraft lease, airport fees, maintenance) looks
   nothing like a SaaS company's (hosting, engineering, sales commissions, support).

5. **Populate with data.** For each leaf node, get actual numbers. Compare to:
   - Prior year (what changed?)
   - Budget/plan (where did we miss?)
   - Competitors/benchmarks (where are we over/under-performing?)

6. **Walk the tree top-down to identify root cause.** Revenue or Costs? If Costs,
   which category? Keep drilling until you reach an operational lever.

7. **Quantify the impact.** "If we fix this lever, how much profit improvement do we
   get?" Turns diagnosis into a prioritized action list.

### Good vs Bad Output

**Good:**
```
Company: Regional restaurant chain, 12 locations
Problem: Profit declined 22% YoY despite stable revenue

Revenue: $14.2M (flat YoY) — NOT the problem
  Avg check: $28 → $31 (+11%) — price increases working
  Covers (volume): 507K → 458K (-10%) — visits declining
    Lunch covers: -18% (remote work trend in region)
    Dinner covers: -3% (stable)

Costs: $12.8M → $13.5M (+5.5%) — PRIMARY PROBLEM
  Variable: $7.1M → $7.0M (-1.4%) — lower volume helped
    Food cost/cover: $9.80 → $10.40 (+6%) — commodity inflation
  Fixed: $5.7M → $6.5M (+14%) — ROOT CAUSE
    Rent: +3% (lease escalations, normal)
    Labor: +22% — BIGGEST DRIVER
      Added 3 sous chefs (+$180K)
      Overtime up 35% (staffing shortages)
      Minimum wage increase Q3 (+$95K annualized)
    Insurance: +18% (post-COVID adjustment)

Root cause: Fixed labor costs up $800K while revenue flat.
Impact: Right-sizing overtime and shifts recovers ~$400-500K → restores
~60% of lost profit.

Secondary: Lunch volume decline (-18%) is structural. Consider converting
underperforming lunch service to prep time, reducing labor further.
```

**Bad:**
```
Profits are down. Revenue is flat. Costs are up. Recommendation: Cut costs.
```

Why it fails: no decomposition past layer 1, no data, no identification of *which*
costs, "cut costs" is not actionable.

### Common Mistakes

1. **Using a generic tree without customization.** A textbook "Revenue - Costs" tree
   with no industry-specific decomposition signals template application, not thinking.

2. **Jumping to solutions before completing the tree.** Hearing "profits are down" and
   recommending cost cuts without confirming whether the problem is revenue-side.

3. **Staying at the aggregate.** Total revenue and total costs without segmenting by
   product, customer segment, or geography. The aggregate can mask one product line
   wildly profitable and another destroying value.

4. **Ignoring sales mix shifts.** Revenue can stay flat while profitability collapses
   if the company sells more low-margin products and fewer high-margin ones.

5. **Treating the tree as static.** Built once captures a snapshot. Value comes from
   comparing across time, segments, or competitors to find *what changed*.

### When It Breaks Down

- **Non-financial root causes.** The tree finds *which number* is wrong but not *why*.
  Competitor patents, regulatory changes, and cultural shifts do not appear in it.
- **Interdependencies between branches.** Revenue and costs are presented as
  independent, but cutting marketing (cost) reduces acquisition (revenue).
- **One-time vs structural.** A snapshot mixes a lawsuit settlement with labor
  inflation. Without time-series context, you cannot distinguish them.
- **Strategic questions masquerading as profitability questions.** "Why are profits
  declining?" might really be "Should we exit this business?"

### Best Combinations

- **Profit Tree + Waterfall/Bridge:** Tree is the analysis; waterfall is the
  communication format showing the "bridge" from last year's profit to this year's.
- **Profit Tree + Inversion:** Invert the tree: "What would guarantee costs increase
  and revenue decrease?" Check which conditions currently exist.
- **Profit Tree + Unit Economics:** Tree decomposes at company level; unit economics
  decomposes at per-customer level. Tree identifies the problem segment; unit
  economics diagnoses why.

---

## 2. Revenue Tree (Driver Tree / KPI Tree)

**Solves:** Mapping how revenue is generated, identifying the highest-leverage growth
levers, and aligning teams to the metrics they actually control.

**Does NOT solve:** Whether growth is profitable (pair with unit economics) or how
large the market is (pair with TAM/SAM/SOM).

### When to Use

- "Where is our revenue growth coming from?"
- Aligning team KPIs to a single North Star metric
- Diagnosing why growth stalled when the business seemed healthy
- Forecasting revenue from operational inputs

**Skip it when:** Revenue is not the primary concern (e.g., pure cost optimization),
or the business model is too early-stage to have stable driver relationships.

### Step-by-Step Workflow

1. **Choose the North Star metric** (root of the tree):
   - SaaS: ARR or MRR
   - E-commerce: GMV or Net Revenue
   - Marketplace: Take Rate x GMV
   - Consumer app: DAU x ARPDAU

2. **First-level decomposition** — multiplicative or additive:
   - `Revenue = Customers x ARPC`
   - `Revenue = Transactions x AOV`
   - `MRR = New MRR + Expansion MRR + Retained MRR - Churned MRR - Contraction MRR`

3. **Second-level decomposition:**
   ```
   New Customers = Organic + Paid + Referral + Partnerships
     Paid = Ad Spend / CAC
     Organic = SEO Traffic x Conversion Rate

   ARPC = Avg Price x Purchase Frequency x Avg Items/Order
   ```

4. **Continue until you reach operational levers.** Each leaf should be something a
   specific team directly influences:
   - Marketing controls ad spend and conversion rate
   - Product controls activation rate and feature adoption
   - Pricing controls average price
   - Customer success controls churn and expansion
   - Stop when further decomposition adds math but no operational insight.

5. **Add measures to each node:**
   - Current value
   - Prior period value (for delta analysis)
   - Target value
   - Sensitivity: "A 1% improvement in this lever produces $X revenue change"

6. **Identify the binding constraint.** Which leaf has the most improvement room
   *and* highest revenue sensitivity? That is the highest-leverage opportunity.

7. **Validate with data, not theory.** The tree structure is a hypothesis. If
   "SEO traffic x conversion rate" does not predict organic acquisition well,
   the tree is wrong.

### Good vs Bad Output

**Good:**
```
North Star: MRR ($420K/month)

├── New MRR: $65K/mo (+8% MoM)
│   ├── Inbound: 1,200 leads → 48 closed ($38K)
│   │   ├── Website: 45K visits x 2.7% lead rate
│   │   └── Close rate: 4% x $790 avg first-month
│   ├── Outbound: 800 prospects → 22 closed ($17K)
│   │   ├── 4 SDRs x 200 prospects/mo
│   │   └── 2.75% close rate x $780 avg
│   └── Partnerships: 5 referrals → $10K (lumpy)
│
├── Expansion MRR: $28K/mo (+12% MoM) ← fastest growing
│   ├── Seat expansion: $18K (2.3 seats/account/quarter)
│   └── Plan upgrades: $10K (15% Pro → Enterprise)
│
├── Retained MRR: $365K (87% gross retention)
│
└── Churned MRR: -$38K/mo ← PROBLEM
    ├── Voluntary: $25K (SMB, avg tenure 4.2 months)
    └── Involuntary: $13K (failed payments, expired cards)

Key finding: Involuntary churn ($13K/mo) is 34% of total churn.
Dunning emails + card updater could recover $8-10K/mo at near-zero cost.
This is the highest-leverage leaf node.

Second priority: SMB voluntary churn (4.2 mo tenure) suggests onboarding
or product-market fit issue in that segment.

Sensitivity:
- 1pt inbound close rate improvement (4% → 5%): +$9.5K MRR
- 1pt gross retention improvement (87% → 88%): +$4.2K MRR
- Fixing involuntary churn: +$8-10K MRR (one-time operational fix)
```

**Bad:**
```
Revenue = Customers x ARPU
Customers = 530
ARPU = $790
Revenue is growing. Need more customers.
```

Why it fails: no decomposition below layer 1, no segmentation, no churn or expansion
analysis, "need more customers" restates the math.

### Common Mistakes

1. **Violating MECE at first level.** If decomposition is "New Sales + Renewals +
   Upsells" but forgets downgrades and churn, branches do not sum to total.

2. **Decomposing beyond operational control.** "Google algorithm preference" is
   mathematically valid but operationally useless. Stop where a team can take action.

3. **Assuming multiplicative relationships are causal.** Revenue = Traffic x Conversion
   x AOV is a mathematical identity. Doubling traffic does not double revenue if new
   traffic has lower conversion.

4. **Ignoring trade-offs between branches.** Discounts boost volume but lower price.
   Aggressive paid acquisition may attract low-LTV customers who increase churn.

5. **Calendar aggregation masking cohort behavior.** A monthly tree mixes customers at
   different lifecycle stages. New-month-1 customers behave differently from 12-month
   retained. Without cohort segmentation, healthy averages mask deterioration.

### When It Breaks Down

- **Platform/network businesses.** Two-sided marketplaces have supply and demand
  drivers that interact. A simple tree cannot capture cross-side externalities.
- **Highly seasonal businesses.** Annual data masks seasonality. Use monthly trees
  with YoY same-month comparisons.
- **Post-hoc rationalization.** Revenue up, traffic up, conclude "SEO worked" — but
  traffic increase might be a competitor outage. Tree shows *what* changed, not *why*.
- **Confounding external factors.** No way to separate internal actions from economic
  cycle, regulation, or pandemic effects.

### Best Combinations

- **Revenue Tree + Unit Economics:** Tree shows where growth comes from; unit
  economics shows whether each vector is profitable. Growing tree with deteriorating
  unit economics = machine that burns more money as it scales.
- **Revenue Tree + Profit Tree:** Revenue tree expands one branch of the profit tree.
  Use revenue tree for growth diagnostics, profit tree for profitability.
- **Revenue Tree + TAM/SAM/SOM:** Revenue tree shows current performance; TAM/SAM/SOM
  shows the ceiling. Comparison reveals headroom in each branch.
- **Revenue Tree + Waterfall:** Identify which drivers changed, then present deltas
  as a waterfall showing how revenue walked from period A to B.

---

## 3. TAM / SAM / SOM

**Solves:** Estimating market size at three levels of realism — theoretical maximum,
what you can serve, and what you can realistically capture.

**Does NOT solve:** Whether you can profitably capture the market (pair with unit
economics), or how to capture it (that is strategy).

### When to Use

- Evaluating a new market entry, product launch, or investment opportunity
- Investor pitch decks (Series A+)
- Strategic planning: "How much runway does this market give us?"
- Comparing market attractiveness across geographies or segments

**Skip it when:** You are creating an entirely new category with no existing market
(the TAM does not exist yet), or the question is operational rather than strategic.

### Step-by-Step Workflow

1. **Define the market precisely in one sentence.** "Cloud-based accounting software
   sold to SMBs (10-200 employees) in North America." Vague definitions are the root
   cause of most TAM inflation.

2. **Choose your calculation approach:**
   - **Top-down:** Industry reports → apply filters. "US accounting software $12B
     (Gartner) → cloud 45% → SMB 30% → TAM = $1.62B."
   - **Bottom-up (preferred by sophisticated investors):** Unit economics. "650K SMBs
     with 10-200 employees x $2,400/yr ACV = $1.56B."
   - **Value-theory:** Total economic value if entire market adopted. Useful for new
     categories with no market data.
   - **Best practice:** Calculate BOTH top-down and bottom-up. If they diverge >2x,
     your assumptions are wrong.

3. **Calculate TAM.**
   `TAM = Total potential customers x Annual revenue per customer`
   Document every assumption.

4. **Calculate SAM.** Apply realistic constraints:
   - Geographic limitations (North America only)
   - Segment focus (SMB only, not enterprise)
   - Product scope (AP/AR only, not full ERP)
   - Distribution reach (online only, no field sales)
   `SAM = TAM x geographic filter x segment filter x product scope filter`

5. **Calculate SOM (hardest and most important).** Requires honest assessment of:
   - Current market share and growth trajectory
   - Competitive intensity
   - Sales capacity (reps x deals/quarter x ACV)
   - Win rate on qualified opportunities
   - Time frame (Year 1 vs Year 5)
   `SOM = SAM x realistic capture rate` — derived from pipeline model, NOT "we'll get
   1% of the market."

6. **Validate with triangulation:**
   - Comparable companies' revenue at similar stage
   - Customer survey data on willingness to pay
   - Bottom-up pipeline analysis (can sales actually close this much?)

7. **Present as a range, not a point estimate.** Low/base/high scenario with
   assumptions driving each.

### Good vs Bad Output

**Good:**
```
Product: AI contract review for mid-market legal departments

TAM (Top-down):
- US legal tech: $28B (Grand View Research 2025)
- Contract management: 12% → $3.4B
- AI-powered: 18% of contract mgmt → $612M

TAM (Bottom-up):
- 38K US companies, 500-5K employees, in-house legal
- Avg 2,400 contracts/yr reviewed
- Tool saves $22/contract in labor + error reduction
- WTP survey (n=120): median $45K/yr
- TAM = 38K x $45K = $1.71B

Reconciliation: Top-down ($612M) captures current AI market only;
bottom-up ($1.71B) includes manual-to-AI conversion. True TAM likely
$800M-$1.2B (some firms won't adopt AI for legal due to risk aversion).

SAM: $1.0B x 85% (English only) x 60% (commercial, not regulatory/IP)
     x 70% (mid-market, not enterprise needing custom integration)
     = $357M

SOM (Year 3):
- 45 current customers (0.12% of addressable)
- Win rate: 28% on qualified opps
- Sales capacity: 12 reps x 4 deals/quarter = 192 deals/yr
- Avg ACV: $52K (growing 15% annually)
- Year 3 SOM: ~$28-35M (pipeline model)
- Implies 8-10% of SAM, consistent with comparable ContractPodAI
  at ~$30M ARR at year 4
```

**Bad:**
```
TAM: The global legal services market is $1 trillion.
SAM: The US portion is $400 billion.
SOM: If we capture just 0.1%, that's $400 million.
This is a massive opportunity.
```

Why it fails: TAM is the entire legal industry, not contract review software. SAM is
just a geographic filter on an inflated number. SOM uses the "1% of a huge market"
fallacy with no bottoms-up justification. The numbers are meaningless.

### Common Mistakes

1. **The "trillion-dollar market" fallacy.** TAM as the broadest possible category.
   If you build a niche SaaS tool, your TAM is not "the global software market."

2. **The "1% fallacy" for SOM.** Sounds modest but skips the entire question of *how*
   you capture that share. SOM must be built bottom-up from pipeline and capacity.

3. **Treating TAM/SAM/SOM as static.** Markets evolve. New competitors, shifting
   preferences, technology changes. Update regularly.

4. **Ignoring the "do nothing" competitor.** The biggest competitor is often the
   customer's status quo — spreadsheets, manual processes, incumbent good-enough
   solutions. SOM must account for behavior change difficulty.

5. **Single-method reliance.** Top-down only or bottom-up only without cross-checking.
   Divergent results signal broken assumptions.

### When It Breaks Down

- **Category-creating products.** No existing market to size. The iPhone's TAM in 2006
  was not "the mobile phone market." TAM/SAM/SOM is for entering existing markets.
- **Platform businesses with indirect monetization.** Social networks monetize through
  ads, not through end-user spending. Sizing "the social media advertising market"
  is correct for Facebook but tells nothing about a new competitor's viability.
- **Investor pitch theater.** TAM/SAM/SOM has become ritual, producing numbers designed
  to impress rather than inform. Series B+ investors deeply discount top-down TAM and
  focus on bottom-up SOM backed by pipeline data.
- **Rapidly disrupting markets.** When technology reshapes a market (AI disrupting
  legal services, EVs disrupting auto), historical data poorly predicts future size.

### Best Combinations

- **TAM/SAM/SOM + Unit Economics:** TAM sizes the market; unit economics determines
  whether you can *profitably* capture it. Large SOM with negative unit economics is
  a trap. Small TAM with 10:1 LTV:CAC is a lifestyle business (may be fine).
- **TAM/SAM/SOM + Revenue Tree:** Revenue tree shows current go-to-market; TAM/SAM/SOM
  shows the ceiling. Reveals how much headroom exists per branch.
- **TAM/SAM/SOM + Second-Order Thinking:** "If we capture 10% of SAM, competitors
  respond. And then? Pricing pressure. And then? Must differentiate on features,
  changing cost structure."

---

## 4. Unit Economics (LTV / CAC)

**Solves:** Whether each customer generates more value than they cost to acquire.
The master question of business viability at the per-customer level.

**Does NOT solve:** Whether the market is large enough (pair with TAM), or where
company-level profitability problems live (pair with profit tree).

### When to Use

- Evaluating whether to scale a channel or business line
- Diagnosing why growth is not producing profit
- Investor due diligence on business model sustainability
- Comparing efficiency across customer segments or acquisition channels

**Skip it when:** You have <100 customers (data is not yet meaningful), or the business
model is fundamentally about network effects not captured in per-customer metrics.

### Step-by-Step Workflow

1. **Calculate fully-loaded CAC.**
   ```
   CAC = (Total Sales + Marketing Costs) / New Customers Acquired
   ```
   Fully-loaded means: all ad spend, sales team comp (salary + commission + benefits),
   marketing team comp, CRM/automation tools, content creation, events, agencies.
   **Do NOT include** product/engineering or customer success costs.
   **Segment by channel** — blended CAC hides that organic is $200 and outbound is
   $5,000. The marginal channel (the one you scale) is always the expensive one.

2. **Calculate LTV.**
   - **SaaS (simple):**
     `LTV = ARPA x Gross Margin / Monthly Churn Rate`
   - **SaaS (precise, discounted):**
     `LTV = Sum of (Monthly Gross Profit x Retention^n) / (1 + discount)^n`
   - **E-commerce:**
     `LTV = AOV x Purchase Frequency x Avg Lifespan x Gross Margin`

   **Critical:** Use **gross margin**, not revenue. LTV on revenue ignores cost of
   serving the customer, inflating by 15-40%. This is the difference between 3:1
   (healthy) and 2.1:1 (concerning).

3. **Calculate LTV:CAC ratio.**
   - **< 1:1** — Lose money on every customer. Unsustainable.
   - **1:1 to 3:1** — Not yet profitable or too close for comfort.
   - **3:1** — Healthy. Industry standard target.
   - **5:1+** — Very efficient or *under-investing in growth*.

4. **Calculate CAC Payback Period.**
   `Payback = CAC / (ARPA x Gross Margin)`
   Benchmark: <12 months SaaS, <6 months e-commerce. A 3:1 LTV:CAC with 24-month
   payback means the economics work *eventually* but cash flow is strained.

5. **Segment everything.** LTV, CAC, LTV:CAC by:
   - Customer segment (SMB vs mid-market vs enterprise)
   - Acquisition channel (paid vs organic vs outbound)
   - Cohort (Q1 vs Q3 — are newer cohorts better or worse?)
   - Product tier (free trial converts vs direct enterprise)

6. **Track cohort retention curves.** LTV depends on how long customers stay. A healthy
   business shows curves that flatten (core percentage stays forever). A sick business
   shows curves that never flatten.

7. **Monitor over time.** Rising CAC with flat LTV is a slow-moving crisis. Track
   monthly or quarterly.

### Good vs Bad Output

**Good:**
```
SaaS PM Tool, Series B

BLENDED:
  CAC: $1,840 (fully loaded: $720 ad + $680 sales comp + $440 overhead)
  LTV: $6,720 (ARPA $280/mo x 72% GM / 3.0% monthly churn)
  LTV:CAC: 3.65:1
  Payback: 9.1 months

BY CHANNEL:
                    CAC      LTV     LTV:CAC   Payback    Mix
  Organic/SEO      $420    $7,800    18.6:1     2.1 mo    22%
  Paid Search     $1,950   $5,200     2.7:1     9.7 mo    35%
  Outbound Sales  $3,400   $9,100     2.7:1    16.9 mo    28%
  Referral         $280    $8,200    29.3:1     1.4 mo    15%

KEY FINDINGS:
1. Blended 3.65 looks healthy, but paid search (35% of volume) is 2.7:1.
   Scaling paid further will deteriorate the blend.
2. Outbound has same ratio as paid but higher LTV ($9,100) — enterprise
   accounts worth the long payback IF cash runway supports it.
3. Organic + referral (37% of mix) at 18-29x — investing in SEO and
   referral has 5-10x better economics than scaling paid.
4. Q4 cohort: 4.2% monthly churn vs 2.8% for Q2 cohort. If this
   persists, LTV drops to $4,800, collapsing blended ratio to 2.6:1.

RECOMMENDATION: Shift $40K/mo from paid search to SEO content + referral
incentives. Investigate Q4 cohort churn (onboarding? different profile?).
```

**Bad:**
```
CAC: $500 (ad spend / signups)
LTV: $10,000 (revenue per customer over 3 years)
LTV:CAC = 20:1
We have amazing unit economics!
```

Why it fails: CAC excludes sales salaries and tools (probably 3-4x higher), LTV uses
revenue not gross profit (overstated ~30%), no channel segmentation, no cohort analysis,
no payback period. The "20:1" is a fantasy built on incomplete inputs.

### Common Mistakes

1. **Incomplete CAC.** Most common error. Only including ad spend, ignoring sales
   salaries, tools, agencies, events. Understates CAC by 2-4x.

2. **Revenue instead of gross profit for LTV.** At 70% margin, this overstates LTV
   by 43%.

3. **Projecting LTV from immature data.** Oldest customers are 12 months old but
   you model 36-month retention. Use conservative assumptions or capped LTV
   ("LTV over 24 months").

4. **Ignoring channel-level segmentation.** Blended CAC averages organic ($200) with
   outbound ($5,000). Blend looks fine, but the marginal channel you scale is the
   expensive one. *Marginal* LTV:CAC determines scaling profitability.

5. **Ignoring time value of money.** $6,000 LTV over 5 years at 10% discount rate is
   ~$4,500 in today's dollars. Matters for capital-intensive businesses.

### When It Breaks Down

- **Early-stage (<100 customers).** Retention curve does not exist. CAC is distorted
  by founder-led sales. Use as directional hypothesis, not evidence.
- **Land-and-expand models.** Month-1 revenue is not indicative of month-12. Simple
  LTV formulas dramatically understate enterprise expansion value.
- **Platform/marketplace businesses.** Per-customer metrics miss network effects. A
  customer bringing 5 referrals has LTV extending far beyond their own revenue.
- **Venture-subsidized growth.** Deliberately spending above-sustainable CAC to capture
  share (Uber/DoorDash model). LTV:CAC alone cannot distinguish rational strategy
  from delusion.

### Best Combinations

- **Unit Economics + Revenue Tree:** Revenue tree shows where growth comes from;
  unit economics shows whether each vector is profitable. Together: "Where should
  we invest the next dollar?"
- **Unit Economics + TAM/SAM/SOM:** TAM sizes the market; unit economics determines
  profitability of capture. Huge TAM + negative economics = trap.
- **Unit Economics + Profit Tree:** Profit tree operates at company level; unit
  economics at per-customer level. When profit tree shows margin problem, unit
  economics diagnoses whether it is CAC or LTV.
- **Unit Economics + Waterfall:** Show how LTV:CAC changed QoQ, decomposed: "CAC up
  0.4x (CPM inflation), LTV up 0.6x (lower churn), net: 3.2x → 3.4x."

---

## 5. Waterfall / Bridge Chart

**Solves:** Explaining *why* a number changed by decomposing the total change into
contributing factors. The definitive communication format for financial variance
analysis.

**Does NOT solve:** Root-cause diagnosis (use profit tree or revenue tree for that).
The waterfall presents findings; it does not discover them.

### When to Use

- Board presentations explaining revenue, profit, or margin changes
- Budget-to-actual variance analysis
- Year-over-year or quarter-over-quarter financial review
- Any time someone asks "why did this number change?"

**Skip it when:** The change has only 1-2 obvious drivers (just state them), or you
need to compare multiple entities side-by-side (grouped bar chart is better).

### Step-by-Step Workflow

1. **Define start and end values** (the "anchor bars"):
   - Last year's revenue → this year's revenue
   - Budget profit → actual profit
   - Q1 margin → Q2 margin

2. **Identify the drivers.** Common decompositions:

   **Revenue bridge:** volume effect, price effect, mix effect, currency effect, new
   product, discontinued product, acquisition/divestiture.

   **Profit bridge:** revenue change, COGS change (materials, labor, overhead), SG&A
   change, one-time items (restructuring, legal).

   **Cost bridge:** inflation/merit increases, new hires, attrition savings,
   restructuring, scope changes.

3. **Calculate each driver's impact.** Sum of all drivers must equal total change
   (Starting + All Drivers = Ending). If it does not balance, a driver is missing or
   miscalculated. This is a mathematical constraint.

4. **Order the drivers for storytelling:**
   - By narrative logic: revenue before cost, operational before financial
   - By magnitude: largest drivers first for "big moves" narrative
   - By controllability: internal actions before external factors
   Choose the ordering serving the audience and message.

5. **Color-code consistently.** Green = positive (increase), red = negative (decrease),
   neutral (blue/gray) = anchor bars. Do not change convention across slides.

6. **Add subtotals at logical breaks.** After all revenue drivers, after all cost
   drivers. Prevents audience losing track of cumulative effect.

7. **Annotate key drivers.** "Volume -$3.2M (lost Walmart contract)" is far more
   useful than a bare "-$3.2M" bar.

8. **Add a "so what?" statement.** One sentence: "Revenue grew $8M, driven by the new
   enterprise tier (+$5.2M), partially offset by SMB churn (-$2.1M)."

### Good vs Bad Output

**Good:**
```
FY2025 → FY2026 EBITDA Bridge ($M)

FY2025 EBITDA                                        $42.0M

Volume growth          +$8.2M   (new enterprise accounts)
Price increases        +$3.8M   (avg 6% across products)
Mix shift              -$2.1M   (more SMB, lower margin)
                       ─────────
Revenue impact         +$9.9M   SUBTOTAL

Raw material inflation -$5.4M   (steel +18% YoY)
Labor cost increase    -$2.8M   (wage inflation + new hires)
Operational efficiency +$3.1M   (automation project savings)
SG&A reduction         +$1.5M   (office consolidation)
                       ─────────
Cost impact            -$3.6M   SUBTOTAL

One-time items         -$1.2M   (restructuring charge)

FY2026 EBITDA                                        $47.1M

TAKEAWAY: EBITDA grew $5.1M (+12%), driven by volume and pricing
(+$12.0M), partially offset by commodity inflation (-$5.4M).
Automation savings ($3.1M) are the standout operational win —
expanding this program is highest-ROI for FY2027.
```

**Bad:**
```
2025: $42M
2026: $47M
Change: +$5M
Factors: revenue up, costs up, one-time charge.
```

Why it fails: no decomposition, no quantification of individual factors, no
sequencing, no "so what?" This is data description, not analysis.

### Common Mistakes

1. **Drivers do not sum to total.** If Starting + Drivers does not equal Ending, a
   driver is missing or miscalculated. Always verify the math.

2. **Too many drivers (>12-15).** Consolidate small ones into "Other." Highlight the
   5-8 most important, not an exhaustive ledger.

3. **Inconsistent color coding.** Green on one slide, blue on another. Pick a
   convention and enforce it across the deck.

4. **Misleading sequencing.** Showing gains before losses tells a "growth" story;
   losses first tells a "pressure" story. Be intentional and honest.

5. **No annotations on key drivers.** "Volume: -$3.2M" raises "*why?*" If you know,
   annotate. If you do not, flag it as "requires investigation."

### When It Breaks Down

- **Hiding volatility in net figures.** Revenue that swung $10M → $15M → $11M shows
  as a modest "+$1M" bar. The waterfall makes a wild ride look calm.
- **False precision in driver isolation.** When volume and price interact, separating
  their impacts requires assumptions. Different attribution methods give different
  bar sizes for the same data.
- **Comparing multiple waterfalls.** Five side-by-side waterfalls (one per BU) are
  chaotic. Use grouped bar charts for cross-entity comparison.
- **Treating the chart as self-explanatory.** A waterfall without a "so what?"
  forces the audience to do their own analysis.

### Best Combinations

- **Waterfall + Profit Tree:** Profit tree is the analytical engine; waterfall is the
  communication format. Always do the tree first, present the waterfall second.
- **Waterfall + Revenue Tree:** Revenue tree identifies which drivers changed; present
  the deltas as a waterfall showing how revenue walked from period A to B.
- **Waterfall + Unit Economics:** Show LTV:CAC changes over time decomposed by factor.
- **Waterfall + TAM/SAM/SOM:** "Market opportunity waterfall" showing TAM narrowing to
  SAM to SOM through each filter.
- **Waterfall + Pre-Mortem:** "Downside waterfall" showing profit if risks materialize:
  "Base $50M → supplier +20% (-$4M) → key customer lost (-$8M) → worst case $38M."

---

## Full-Stack Sequences

### "Why are we losing money?" (Profitability Diagnostic)

1. **Profit Tree** — find the root-cause branch
2. **Unit Economics** — validate at per-customer level
3. **Waterfall** — present the bridge to leadership

### "Where should we invest for growth?" (Growth Strategy)

1. **Revenue Tree** — map current drivers and highest-leverage levers
2. **TAM/SAM/SOM** — size the headroom per growth vector
3. **Unit Economics** — confirm profitability of the target channel
4. **Waterfall** — show projected revenue bridge under the plan

### "Should investors fund this?" (Investor Due Diligence)

1. **TAM/SAM/SOM** — market size at three levels of realism
2. **Unit Economics** — per-customer profitability and payback
3. **Revenue Tree** — growth driver breakdown with sensitivity
4. **Waterfall** — historical growth narrative and projected path

### Full Business Health Check

1. **Profit Tree** — company-level diagnosis
2. **Revenue Tree** — growth driver mapping
3. **Unit Economics** — per-customer validation
4. **TAM/SAM/SOM** — market ceiling and headroom
5. **Waterfall** — communicate all findings to the board
