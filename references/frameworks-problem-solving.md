# Problem-Solving Frameworks: Practitioner Reference

Synthesized from multiple research sources. No textbook definitions -- only workflow, judgment calls, and concrete examples with numbers.

---

## 1. MECE (Mutually Exclusive, Collectively Exhaustive)

### When to Use

- Decomposing any problem, market, cost structure, or population into non-overlapping, gap-free buckets
- Quality-checking every level of an Issue Tree, Hypothesis Tree, or Pyramid grouping
- Structuring a data request ("give me revenue by X") so nothing is double-counted or missing

MECE is not a standalone framework. It is the quality gate applied inside every other framework here.

### Step-by-Step Workflow

**Step 1 -- Define the universe (5 min).** Write down exactly what you are decomposing. "All sources of revenue for Company X" is decomposable. "Things that matter" is not.

**Step 2 -- Pick ONE decomposition logic.**

| Logic | How it works | Strength |
|-------|-------------|----------|
| **Algebraic** | Use an equation: Profit = Revenue - Cost | Provably MECE. Strongest. |
| **Process** | Sequential steps: Awareness > Consideration > Purchase > Retention | Strong for funnels, operations |
| **Dichotomy** | Two opposing halves: Internal vs. External, New vs. Existing | Clean and fast |
| **Framework** | Known structure: Porter's 5 Forces, 4Ps | Weakest -- trusting someone else's decomposition |

Always prefer algebraic when an equation exists. Revenue = Price x Volume is inarguable.

**Step 3 -- Draft 3-5 categories.** Two is fine for a dichotomy. Five is the practical ceiling. Six or more means you need a higher grouping level.

**Step 4 -- Stress-test for ME.** For every pair, ask: "Can a single data point belong in both?" If yes, redraw or merge.

**Step 5 -- Stress-test for CE.** Ask: "Is there a plausible item that fits nowhere?" An "Other" bucket is acceptable for minor residuals (< 5% of total), never for important items.

**Step 6 -- Iterate (10-15 min).** The first cut is rarely right. If you cannot explain the grouping in one sentence, it is not clean.

### Good vs. Bad Output

**Good -- Revenue decomposition for a retail chain:**
```
Total Revenue ($2.1B)
 +-- In-store sales ($1.5B) -- all POS transactions at physical locations
 +-- E-commerce sales ($480M) -- all website/app transactions
 +-- Wholesale/licensing ($120M) -- all B2B revenue
```
ME: A transaction occurs in exactly one channel. CE: Every revenue dollar maps to one bucket.

**Bad -- Same company:**
```
Total Revenue
 +-- Digital sales
 +-- Retail sales
 +-- B2B sales
 +-- Marketing-driven sales
```
"Digital sales" overlaps with "B2B" (online B2B orders double-counted). "Marketing-driven sales" overlaps with everything. Licensing income fits nowhere.

### Common Mistakes

1. **Hidden overlaps that look clean.** "Customer Acquisition" and "Marketing Spend" as siblings -- marketing spend drives acquisition, so they are causally nested, not parallel.
2. **Boiling the ocean for CE.** Collectively exhaustive does not mean every edge case. 80/20 applies.
3. **Forcing a MECE framework that does not match the problem.** A geography split is useless when the problem is product quality.
4. **Over-segmentation.** 8-12 categories at one level means you failed to group. Step back.
5. **Confusing structure with insight.** A perfect MECE tree with no analysis inside each bucket is an empty scaffold.

### When It Breaks Down

- **Highly interdependent systems with feedback loops** -- decomposition creates an illusion of independence. Use MECE to organize the work, accept cross-cutting dependencies in reality.
- **Creative brainstorming** -- rigid ME thinking suppresses lateral connections. Apply MECE after idea generation, not during.
- **Wicked problems with contested definitions** -- if stakeholders disagree on the "universe," MECE is premature.

### Best Combinations

MECE + Issue Tree (quality gate at every node), MECE + Pyramid Principle (every argument group must be MECE), MECE + 7-Step Step 2 (disaggregation IS MECE decomposition).

---

## 2. Issue Tree

### When to Use

- Map ALL possible causes (diagnostic tree) or ALL possible solutions (solution tree)
- Problem is complex enough that brainstorming produces a flat, overlapping list
- Need to assign parallel workstreams to a team -- each branch becomes a workstream
- Do not yet have a strong hypothesis and need open exploration

Rule: diagnose before you solve. Build the Why tree first, then a How tree for the top causes.

### Step-by-Step Workflow

**Step 1 -- Write the root question (5-10 min).** Specific and clear. "Why has operating profit declined 15% over the last two quarters?" -- not "Profit is bad." The question type determines tree type:

| Type | Root question form | Purpose |
|------|-------------------|---------|
| **Diagnostic (Why)** | "Why is X happening?" | Identify root causes |
| **Solution (How)** | "How can we achieve X?" | Identify interventions |

**Step 2 -- Generate Level 1 branches (15-30 min).** 3-5 sub-questions, MECE. Use algebraic logic when possible.

```
Why has operating profit declined 15%?
 +-- Have revenues decreased?
 +-- Have costs increased?
 +-- Has the product/channel mix shifted unfavorably?
```

**Step 3 -- Decompose each branch (30-60 min per branch).** Keep going until each leaf is answerable by a single data pull.

```
Have revenues decreased?
 +-- Has volume decreased?
 |    +-- Fewer new customers? (data: acquisition funnel by month)
 |    +-- Higher churn? (data: cohort retention curves)
 +-- Has price/unit decreased?
      +-- Explicit price cuts? (data: pricing log vs. prior year)
      +-- Shift toward lower-priced SKUs? (data: mix analysis by tier)
```

**Step 4 -- Assign each leaf to an analysis.** What data, who runs it, by when.

**Step 5 -- Validate with stakeholders.** Confirm nothing missing (CE), no overlaps (ME).

**Step 6 -- Prune as data comes in.** Mark dead branches, reallocate to live ones.

### Good vs. Bad Output

**Good -- SaaS churn diagnostic:**
```
Why is monthly churn above 5%?
 +-- Product-market fit issues
 |    +-- Core feature gaps vs. competitors? (compare feature matrix)
 |    +-- Wrong target segment? (churned vs. retained firmographics)
 +-- Onboarding failures
 |    +-- Time-to-value > 14 days? (activation milestone timing)
 |    +-- Setup complexity? (support ticket analysis)
 +-- Pricing/value perception
 |    +-- Price > perceived value? (win/loss survey)
 |    +-- Competitor undercut? (competitive price audit)
 +-- Customer success gaps
      +-- Support response > 4hr SLA? (ticket response time)
      +-- Proactive engagement insufficient? (CSM touch frequency vs. churn)
```

**Bad -- Same problem:**
```
Why is churn above 5%?
 +-- Product issues          (too vague)
 +-- Customer dissatisfaction (overlaps with everything -- it's an outcome, not a cause)
 +-- Competitors are better   (overlaps with product and pricing)
 +-- Bad onboarding / Support is slow / Too expensive / Wrong marketing targets
```
Flat list, no hierarchy, not actionable, not MECE.

### Common Mistakes

1. **Random listing instead of structured decomposition.** Pick decomposition logic first, then fill in.
2. **The aggregator fallacy.** "Revenue declined" is the symptom restated. Decompose into WHY.
3. **Mixing diagnostic and solution branches.** "Hire more salespeople" inside a "Why are sales declining?" tree skips diagnosis.
4. **Skipping levels.** Jumping from "Why did profit decline?" to "Is it the new CRM system?" misses intermediate causes.
5. **Building once, never updating.** Prune ruled-out branches, expand promising ones as data arrives.

### When It Breaks Down

- **Feedback loops** -- pricing affects volume affects costs affects pricing. Supplement with causal loop diagrams.
- **Contested problem definitions** -- use SCQA to align on the root question first.
- **Single dominant cause** -- if 95% of the issue is one factor, a simple root-cause chain suffices.

### Best Combinations

Issue Tree + MECE (quality gate), Issue Tree then Hypothesis Tree (the canonical McKinsey/BCG workflow: map all causes, then hypothesize about the most likely), Issue Tree + SCQA (SCQA's Question becomes the tree's root), Issue Tree + 7-Step Step 2 (the tree IS the disaggregation).

---

## 3. Hypothesis Tree

### When to Use

- You have enough domain knowledge to form a reasonable initial hypothesis
- Need to move fast -- hypothesis-driven is 2-3x faster than open exploration when the hypothesis is good
- The problem likely has a dominant cause and you want to confirm or kill it quickly
- Need to prioritize scarce analytical resources on riskiest assumptions first

Critical prerequisite: a reasonable initial hypothesis. If you are entering a new domain, use an Issue Tree first.

### Step-by-Step Workflow

**Step 1 -- Define the problem as a question.** Same as Issue Tree.

**Step 2 -- Form the initial hypothesis.** Informed by experience, analogies, initial data.
Example: "Airline Inc. can achieve $400M in savings primarily through fleet optimization ($250M) and crew scheduling ($150M)."

**Step 3 -- Decompose: "What must be true?"** 3-5 conditions that must ALL hold.

```
Hypothesis: Fleet + crew = $400M savings
 +-- Fleet optimization can yield >= $250M
 +-- Crew scheduling can yield >= $150M
 +-- Implementation is feasible within 2 years
```

**Step 4 -- Continue decomposing each condition.**
```
Fleet optimization >= $250M
 +-- Current fleet has >= 15% utilization inefficiency
 +-- Retiring older aircraft saves >= $100M/yr in maintenance
 +-- Route optimization from right-sizing saves >= $150M/yr
```

**Step 5 -- Design falsification tests.** Define what would PROVE IT WRONG before looking at data.

| Leaf hypothesis | Falsification test | Kill threshold |
|----------------|-------------------|----------------|
| Fleet >= 15% utilization gap | Block hours/aircraft vs. industry benchmark | Gap < 5% = branch dies |
| Retiring planes saves >= $100M | Maintenance cost by aircraft age cohort | Delta < $60M = insufficient |
| Crew scheduling >= $150M | Overtime + deadhead cost vs. optimal schedule | Gap < $80M = need alternate |

**Step 6 -- Test riskiest assumptions first.** Prioritize by: what collapses the entire hypothesis if false, AND what is cheapest to test.

**Step 7 -- Update or pivot.** If falsified: modify scope, pivot entirely, or decompose the failed branch further. Do NOT ignore falsifying data.

### Good vs. Bad Output

**Good -- Declining retail sales:**
```
Hypothesis: Sales decline driven by supply chain disruption
 +-- Stockout rate increased significantly
 |    Test: Stockout % this quarter vs. prior 4 quarters
 |    Kill if: change < 2 percentage points
 +-- Stockouts = lost sales, not delayed sales
 |    Test: Do orders rebound after restock?
 |    Kill if: > 70% reappear within 2 weeks
 +-- Supply issues are within our control
      +-- Supplier capacity declined (delivery data + utilization reports)
      +-- Demand forecasting deteriorated (MAPE trend over 6 quarters)
```

**Bad -- Same problem:**
```
Hypothesis: We need to sell more
 +-- Marketing is not working / Sales team needs training / Product outdated / Competition tough
```
"We need to sell more" restates the problem. No falsification tests. No "must be true" logic.

### Common Mistakes

1. **Confirmation bias (#1 killer).** Define falsification tests BEFORE looking at data. Write: "I will abandon this if X."
2. **Treating hypothesis as fact.** It is a working assumption, not a conclusion.
3. **Poorly formed hypothesis.** "Things are bad because of competition" is not testable. "Revenue declined 12% because Competitor X captured $8M of mid-market" is.
4. **Testing easy branches first.** Prioritize by "what kills the hypothesis fastest?" not "what data do I have?"
5. **Not pivoting when evidence demands it.** Sunk cost fallacy. Three falsified conditions = pivot.

### When It Breaks Down

- **Insufficient domain knowledge** -- a bad hypothesis wastes time testing the wrong thing. Use Issue Tree instead.
- **Multi-causal problems** -- if 5 factors each contribute 15-25%, no single hypothesis captures it.
- **Politically sensitive environments** -- a hypothesis can feel like an accusation. Open-question framing is safer.
- **Rapidly changing environments** -- hypothesis goes stale before validation. Use rapid experimentation.

### Best Combinations

Issue Tree first then Hypothesis Tree (canonical workflow), Hypothesis Tree + Pyramid (validated hypothesis = governing thought, validated conditions = supporting arguments), Hypothesis Tree + 7-Step Steps 3-5.

---

## 4. 7-Step Problem Solving (McKinsey)

### When to Use

- Complex, multi-week problems requiring team coordination
- High-stakes decisions where rigor matters more than speed
- Root cause genuinely unknown, multiple parallel workstreams needed

Do NOT use for decisions needed in hours. Use SCQA + Hypothesis + Pyramid instead.

### Step-by-Step Workflow

**Step 1 -- DEFINE the problem (20-30% of upfront time).**

| Element | Example |
|---------|---------|
| **Question** | "How can RetailCo increase same-store revenue by 8% within 18 months?" |
| **Context** | "Foot traffic declining 3% YoY. E-commerce growing 22%. New CEO." |
| **Success criteria** | "8% revenue lift, 18 months, headcount increase < 5%" |
| **Scope** | "In: pricing, assortment, format. Out: M&A, new stores." |
| **Stakeholders** | "CEO decides. CFO requires < 2yr payback. Ops VP veto on staffing." |

Must be SMART: Specific, Measurable, Action-oriented, Relevant, Time-bound.

**Step 2 -- DISAGGREGATE.** Build an Issue Tree. Every branch MECE. Use algebraic decomposition (Revenue = Traffic x Conversion x AOV).

**Step 3 -- PRIORITIZE.** Impact x Ability to influence. 80/20: 20% of branches drive 80% of outcome. Form hypotheses on top branches.

**Step 4 -- WORKPLAN.**

| Workstream | Hypothesis | Analysis | Owner | Deadline |
|-----------|-----------|---------|-------|----------|
| Pricing | "8-12% below market on key categories" | Benchmark top 50 SKUs vs. 3 competitors | Analyst A | Day 5 |
| Conversion | "Checkout friction loses 15% of shoppers" | Entry > browse > try > buy funnel | Analyst B | Day 7 |

Critical rule: describe the output slide/table BEFORE starting. If you cannot, you do not understand the analysis.

**Step 5 -- ANALYZE.** Execute workplan. Test hypotheses. Document supported/falsified. Distinguish correlation from causation.

**Step 6 -- SYNTHESIZE.** Pyramid Principle: governing thought + 3-4 supporting arguments + evidence. "So what?" test: every finding must connect to the recommendation or get cut.

**Step 7 -- COMMUNICATE.** SCQA (introduction) + Pyramid (body). Lead with the answer. Include action plan: what, who, when, expected impact. Anticipate objections.

### Good vs. Bad Output

**Good problem statement:** "How can MedTech reduce development cycle from 36 to 24 months for Class II devices, maintaining 85%+ FDA approval, within 2 years?"

**Bad:** "MedTech needs to innovate faster." (Not a question. Not specific. Not measurable.)

**Good disaggregation:**
```
Reduce dev cycle 36 --> 24 months
 +-- Pre-clinical (12mo): parallelize testing? simulation vs. physical prototyping?
 +-- Regulatory prep (10mo): pre-submission FDA meetings? modular submissions?
 +-- Manufacturing scale-up (14mo): design for manufacturability? dual-source components?
```

**Bad:** "Hire more engineers / Use AI / Copy competitors / Spend more on R&D" -- solution list, not disaggregation. Skips diagnosis.

### Common Mistakes

1. **Rushing past problem definition.** Weak statement guarantees misaligned analysis and scope creep.
2. **Reusing old templates.** A manufacturing cost tree will not work for SaaS. Build from the problem.
3. **Letting hierarchy dominate.** If the partner's hypothesis is never challenged, the team converges on the boss's pet theory.
4. **Analysis without synthesis.** 50 slides without "So what?" is the most common junior failure.
5. **Recommendations without action plans.** "Invest in digital" is not actionable. Specify actions, owners, timeline, expected impact.

### When It Breaks Down

- **Speed > rigor** -- for a 2-hour decision, use SCQA + Hypothesis + Pyramid.
- **Genuinely novel problems** -- use iterative experimentation (build-measure-learn).
- **Politics > analytics** -- supplement with stakeholder mapping and change management.
- **Data does not exist** -- scenario planning and expert judgment replace hypothesis testing.

### Best Combinations

7-Step uses ALL other frameworks: Issue Tree (Step 2), MECE (Step 2), Hypothesis Tree (Steps 3-5), Pyramid (Step 6), SCQA (Step 7). It is the meta-framework.

---

## 5. Pyramid Principle (Minto)

### When to Use

- Presenting findings, recommendations, or analysis to decision-makers
- Writing memos, emails, or decks where the audience must act
- Any situation where the audience's time is scarce

The Pyramid is a COMMUNICATION tool, not a thinking tool. Think bottom-up, present top-down.

### Step-by-Step Workflow

**Step 1 -- Start with the answer (Governing Thought).** One sentence. "RetailCo should invest $5M in dynamic pricing to capture $40M in annual revenue upside."

**Step 2 -- 3-4 supporting arguments.** Each must directly support the conclusion. If interesting but irrelevant, cut it.
```
Invest $5M for $40M upside
 +-- $40M left on the table due to static pricing (elasticity analysis: 12% uplift on top 200 SKUs)
 +-- Technology proven in comparable retailers (Competitor A: 9% lift Year 1)
 +-- $5M over 18 months, payback < 2 years (our pilot: 7% lift in 3 stores over 6 months)
```

**Step 3 -- Evidence under each argument.** Data, benchmarks, pilot results.

**Step 4 -- Order each group by one logic:**

| Order | Use when | Example |
|-------|----------|---------|
| **Time** | Steps, cause-effect | "Pilot, then scale, then optimize" |
| **Structural** | Parts of a whole | "North America 60%, Europe 30%, Asia 10%" |
| **Degree** | Ranking | "Pricing 60%, assortment 25%, layout 15%" |

**Step 5 -- Inductive at top (easier to absorb), deductive at bottom (rigorous proof).**

**Step 6 -- "So what?" test at every level.** If you cannot explain why a point matters to the recommendation, cut it.

**Step 7 -- Present top-down.** Audience hears the answer first, supporting logic second, evidence only on drill-down.

### Good vs. Bad Output

**Good:** "Consolidate from 3 DCs to 2, saving $12M/year. (1) Northeast DC at 40% capacity, below breakeven. (2) Consolidation feasible -- logistics sim shows < 0.5 day delivery impact. (3) Net $12M savings by Year 2 after closure costs."

**Bad:** "We analyzed the Northeast DC. Built 2008. 200K sq ft. 40% utilization. Also analyzed Midwest at 75% and Southeast at 68%. Ran 47 scenarios... [three paragraphs later] ...therefore consolidate to 2." Recommendation buried. Executive loses patience.

### Common Mistakes

1. **Burying the lead.** Starting with background or methodology. Lead with the answer. Always.
2. **Arguments that do not support the governing thought.** "Market grew 5%" is interesting but irrelevant -- appendix.
3. **Non-MECE groupings.** Overlapping arguments or missing a key objection.
4. **Overloading with data.** Most audiences need Level 1 + Level 2. Level 3 is drill-down only.
5. **Lists without internal logic.** Unordered "key findings" = data dump.

### When It Breaks Down

- **Exploratory conversations** -- leading with an answer during brainstorming shuts down alternatives.
- **Hostile audiences** -- lead with evidence instead, earn the right to state the conclusion. Minto acknowledged this.
- **Nuanced "it depends" situations** -- forced single governing thought can mislead. Present trade-offs honestly.
- **Technical audiences wanting evidence first** -- engineers prefer bottom-up. Read the room.

### Best Combinations

Pyramid + SCQA (SCQA = introduction on-ramp, Pyramid = body highway), Pyramid + MECE (every argument group), Pyramid + 7-Step Step 6 (the Pyramid IS the synthesis), Pyramid + Hypothesis Tree (validated hypothesis = governing thought).

---

## 6. SCQA (Situation-Complication-Question-Answer)

### When to Use

- Opening a presentation, memo, or proposal where you need to build a case
- Defining a problem statement (feeds directly into 7-Step Step 1)
- Any communication where the audience needs WHY before WHAT

Do NOT use for simple status updates, yes/no answers, or routine messages.

### Step-by-Step Workflow

**Step 1 -- SITUATION (1-3 sentences).** Shared context the audience already knows. Non-controversial. No new information.
> "MedTech has led Class II cardiac devices for a decade, 35% share, 90%+ FDA approval rates."

**Step 2 -- COMPLICATION.** What changed. Specific, with numbers. Creates urgency.
> "Development cycle lengthened to 36 months -- 50% longer than two fastest competitors -- missing two launch windows, losing 4 points of share."

**Step 3 -- QUESTION.** Arises naturally from the complication. Must be directly answerable. Match scope to complication.
> "How can MedTech cut cycle to 24 months while maintaining FDA track record?"

**Step 4 -- ANSWER (1-3 sentences).** Becomes the Pyramid's governing thought.
> "Parallelize pre-clinical testing, adopt modular regulatory submissions, design for manufacturability from Day 1."

### Good vs. Bad Output

**Good -- Board presentation:**
> **S:** "Dell led computer systems for 20 years via direct-to-consumer cost advantage."
> **C:** "Lenovo and Huawei now undercut Dell's price by 15-20%, eroding core PC margins."
> **Q:** "How can Dell compete when hardware cost is no longer its advantage?"
> **A:** "Double down on services -- managed IT, cloud, cybersecurity -- ceding lowest-cost hardware, building higher-margin sticky revenue."

**Bad:** S: "Tech is changing." C: "Dell has challenges." Q: "What should Dell do?" A: "Innovate and be competitive." Every element fails to add information.

**Good -- Internal email:**
> **S:** "Q3 target: 45 new enterprise accounts. 6 weeks left."
> **C:** "18 closed, pipeline shows 22 at Stage 3+. Risk of missing by 15-20%."
> **Q:** "What can we do in 6 weeks to close the gap?"
> **A:** "(1) Accelerate 8 Stage 2 deals via exec-to-exec outreach. (2) Q3-only pricing incentive for deals > $100K. (3) Reassign 2 SDRs to pipeline acceleration."

### Common Mistakes

1. **Complication too vague or too grandiose.** "The world is changing" -- not a complication. "Climate change threatens all business" -- dwarfs any answer.
2. **Scale mismatch.** $500M complication, $2M answer = credibility gap.
3. **Situation too long or teaches new information.** Only shared context.
4. **Skipping the Complication.** No tension = no urgency = "Why should I care?"
5. **Forcing SCQA on everything.** Quick Slack messages do not need it.

### When It Breaks Down

- **Simple, low-stakes comms** -- brevity beats structure.
- **No genuine complication** -- use SQA (Situation-Question-Answer) for neutral/positive updates.
- **Audience does not share the Situation** -- need more setup in cross-functional contexts.

### Best Combinations

SCQA + Pyramid (the canonical pair: SCQA introduces, Pyramid delivers), SCQA + Issue Tree (the Question = tree root), SCQA + 7-Step Step 1 (S = context, C = problem, Q = basic question, A = initial hypothesis).

---

## 7. Quick Reference

### By Situation

| You are here | Use | Supporting |
|-------------|-----|-----------|
| "I do not understand the problem" | SCQA | -- |
| "I need to map all possible causes" | Issue Tree | MECE |
| "I have a theory to test" | Hypothesis Tree | MECE |
| "Complex problem, end-to-end" | 7-Step | All five |
| "I need to present findings" | Pyramid | SCQA + MECE |
| "I need a compelling memo" | SCQA | Pyramid |

### By Time Available

| Time | Approach |
|------|----------|
| 2-hour meeting | SCQA + Hypothesis + Pyramid |
| 1-week sprint | Issue Tree + Hypothesis Tree + Pyramid |
| 2-month engagement | Full 7-Step |

### End-to-End Workflow

```
DEFINE  (SCQA + Problem Statement)  -->  clear, SMART problem
STRUCTURE  (Issue Tree + MECE)      -->  complete map of sub-questions
PRIORITIZE  (Hypothesis Tree)       -->  testable hypotheses + falsification
ANALYZE  (Workplan + data)          -->  validated/falsified with evidence
COMMUNICATE  (Pyramid + SCQA)       -->  answer-first recommendation
```

### Anti-Patterns

1. **Pyramid during analysis** -- think bottom-up, present top-down. Using Pyramid to analyze = confirmation bias.
2. **Issue Tree without a problem statement** -- a solution in search of a problem. SCQA first.
3. **MECE as end in itself** -- relevance > structural purity.
4. **7-Step when speed matters** -- SCQA + Hypothesis + Pyramid for a 2-hour decision.
5. **Hypothesis Tree in a new domain** -- bad hypothesis wastes more time than open exploration. Issue Tree first.
6. **Bottom-up to executives** -- they want answers. Pyramid. Reserve bottom-up for technical audiences.
