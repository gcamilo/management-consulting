# Decision Frameworks — Practitioner Reference

Five frameworks for different failure modes in decision-making. Each solves a specific
problem: unclear ownership, poor option comparison, hidden risk, missed consequences,
or avoidable failure. The strongest practice is sequencing the right ones for the
actual bottleneck.

---

## 1. RAPID (Bain & Company)

**Solves:** Unclear ownership, decision paralysis, diffused accountability across
multi-stakeholder organizations.

**Does NOT solve:** Strategy quality, analytical rigor, or execution planning.
RAPID clarifies *who* owns each part of the decision — not *how* to analyze it.

### When to Use

- Multiple teams or functions have a stake in a decision
- Decisions stall in "alignment" loops with no clear owner
- Previous decisions got relitigated because roles were ambiguous
- Stakes are high AND interdependence across teams is high

**Skip it when:** The decision is easily reversible, speed-critical (hours not days),
or involves fewer than 3 stakeholders.

### Step-by-Step Workflow

1. **Frame the decision in one sentence.** "Should we migrate the data platform from
   on-prem to AWS?" not "Cloud strategy." Vague framing is the #1 source of downstream
   confusion.

2. **Assign five roles to named individuals (not teams).**
   - **R (Recommend):** Owns the analysis, gathers input, brings a written
     recommendation. One person. Aligns with D upfront on criteria and timing.
   - **I (Input):** Subject-matter experts who provide data and constraints.
     Time-boxed contributions. No veto rights. Define "silence = no objection."
   - **A (Agree):** 2-3 people max with true veto authority on documented,
     specific grounds ("violates SOC2," "exceeds $2M budget"). Not preference.
   - **D (Decide):** One person who makes the final call. Single D is the keystone.
   - **P (Perform):** Implementation owner. Plans, resources, delivers, reports outcomes.

3. **Document the RAPID chart** and circulate before work begins. Simple table:
   Decision | R | I | A | D | P, with veto criteria and deadlines.

4. **R gathers I contributions** with deadlines. Set SLAs — if I roles do not respond
   within the timeframe, silence counts as no objection.

5. **R presents to A for sign-off.** A can only block on pre-agreed criteria. If A
   objects, R revises and resubmits.

6. **R presents final recommendation to D.** D decides publicly, with rationale
   documented.

7. **D hands to P.** P converts the decision into actions, owners, milestones.

8. **Document rationale and assumptions.** Record *why* the decision was made so the
   team can revisit intelligently later.

9. **Review after implementation.** Separate bad process from bad outcomes caused by
   uncertainty.

### Good vs Bad Output

**Good:**
```
Decision: Should we migrate the data platform from on-prem to AWS?

R: VP Engineering (Sarah) — owns analysis, vendor comparison, cost model
I: Security (compliance input), Finance (budget input), Ops (migration risk)
A: CISO (vetoes if SOC2 gap > 6 months), CFO (vetoes if 3-year TCO > $2M)
D: CTO (final call)
P: Platform team lead (executes migration)

Timeline: I inputs due March 10, A sign-off by March 17, D decision by March 20.
Rationale: expected payback in 11 months; main risk is onboarding friction.
Assumptions: CAC under $900, support contacts under 0.6/account/month.
```

**Bad:**
```
Decision: Cloud migration
R: Engineering team
A: Leadership team
D: CTO and CEO (co-decide)
P: Everyone
No veto criteria. No deadlines. No individual names.
```

Why it fails: team names instead of individuals, two Deciders (guaranteed deadlock),
no veto criteria for A, "everyone" for P means no accountability.

### Common Mistakes

1. **Multiple Deciders.** Co-D's produce deadlock. If you cannot agree on one D, you
   have a governance problem RAPID cannot solve — escalate it.

2. **Agree sprawl.** Everyone wants veto power. Six A-holders balloon cycle time. Move
   most to I; limit A to 2-3 roles with explicit veto grounds.

3. **Treating I as A.** Teams accidentally create too many veto points. Input should
   improve decision quality, not become shadow approvals.

4. **No SLAs for Input.** When I roles do not respond, decisions stall. Time-box and
   enforce "silence = no objection."

5. **Using RAPID for trivial decisions.** RAPID adds overhead. "Which conference room?"
   does not need a governance framework.

### When It Breaks Down

- **Speed-critical decisions.** Multi-step process is too slow for crisis response.
  Use commander's intent instead.
- **Flat/consensus cultures.** If no one will be the single D, or a hidden veto
  overrides the D, RAPID becomes theater.
- **Highly reversible decisions.** Low reversal cost means RAPID overhead is not
  justified. Bias to action instead.
- **Shadow power structures.** An executive who is formally I but informally overrides
  D negates the framework entirely.
- **Rapid iteration environments.** Formal role assignment is too heavy when decisions
  are decentralized and change daily.

### Best Combinations

- **RAPID + Decision Matrix:** RAPID defines *who* decides; the matrix structures the
  analysis that R presents to D.
- **RAPID + Pre-Mortem:** After D decides, run a pre-mortem with P and I to
  stress-test the implementation plan.
- **RAPID + Inversion:** Use inversion to test whether the recommendation creates
  obvious failure modes before the D commits.

---

## 2. Decision Matrix (Weighted Scoring)

**Solves:** Making tradeoffs visible when choosing between concrete options. Forces
explicit criteria, weights, and scores instead of arguing from gut feel.

**Does NOT solve:** Strategy formulation, values-based choices, or decisions where
options are too ambiguous to compare.

### When to Use

- 3-7 concrete, comparable options exist
- Multiple stakeholders disagree on what matters
- You need an audit trail for why a choice was made
- The decision is significant enough to justify 2-4 hours of structured analysis

**Skip it when:** Options are not mature enough to compare, the decision is binary
(go/no-go), or the most important variables are deeply uncertain.

### Step-by-Step Workflow

1. **Define the decision and list all viable options.** Include "do nothing" as
   baseline if relevant. Fewer than 3 options means the matrix is unnecessary; more
   than 7 becomes unwieldy.

2. **Identify 4-8 evaluation criteria.** Each must be relevant, measurable (even
   qualitatively), and independent from the others. Audit for double-counting:
   "ease of use" and "training time" measure the same thing.

3. **Assign weights BEFORE scoring.** This is critical — weights must be locked before
   anyone evaluates options to prevent reverse-engineering. Weights sum to 100%.
   Methods:
   - **Direct allocation:** Distribute 100 points across criteria.
   - **Pairwise comparison:** Compare each criterion against every other; count wins.
   - **Swing weighting:** "If I could move one criterion from worst to best, which
     would I swing first?"

4. **Score one criterion at a time across all options** (not one option across all
   criteria). This reduces halo effects. Use a consistent scale (1-5). Align on what
   each score means — what makes something a 5 on "speed to implement"?

5. **Calculate weighted scores.** For each option: sum of (score x weight).

6. **Sensitivity analysis.** Change the top 2-3 weights by +/-20%. If the winner
   flips with small shifts, the decision is fragile.

7. **Inspect, do not obey blindly.** Check:
   - Is the winner strong across the board, or does it win on one dominant criterion?
   - Does any option have a fatal flaw (score of 1 on a critical criterion) that the
     aggregate masks?
   - Should any non-quantified factor (cultural fit, regulatory uncertainty) override?

### Good vs Bad Output

**Good:**
```
CRM selection for 250-person services firm. Weights locked before scoring.

                    Weight   Salesforce   HubSpot   Pipedrive
Integration depth    30%       4 (1.2)    3 (0.9)    2 (0.6)
Total cost (3yr)     25%       2 (0.5)    4 (1.0)    5 (1.25)
Ease of adoption     20%       3 (0.6)    5 (1.0)    4 (0.8)
Reporting quality    15%       5 (0.75)   3 (0.45)   2 (0.3)
Vendor stability     10%       5 (0.5)    4 (0.4)    3 (0.3)
                             --------   --------   --------
TOTAL                          3.55       3.75       3.25

Sensitivity: If Integration drops to 20% and Cost rises to 35%, HubSpot
still wins (3.85 vs 3.35). Decision is robust.

Note: Pipedrive scored highest on cost but has a fatal flaw on integration
(score 2) that our API-heavy architecture cannot tolerate.
```

**Bad:**
```
              Salesforce   HubSpot   Pipedrive
Features         8           7          6
Price            5           8          9
Support          7           7          6
TOTAL           20          22         21
Winner: HubSpot
```

Why it fails: no weights, vague criteria ("features"), no score definitions, no
sensitivity analysis, no interpretation.

### Common Mistakes

1. **Setting weights after scoring.** People unconsciously shift weights toward their
   preferred option. Always lock weights before anyone sees scores.

2. **Correlated criteria that double-count.** Having both "ease of use" and "training
   time" inflates usability's influence. Audit criteria for independence.

3. **Too many low-impact criteria.** 15 criteria where 10 are minor dilutes the 3-4
   that actually matter. Many small criteria can collectively outweigh a single
   critical one, producing a mathematically "correct" but practically wrong answer.

4. **Scoring options one at a time.** Scoring all criteria for Option A before Option B
   creates halo effects. Score horizontally (one criterion across all options).

5. **Treating the output as the answer.** The matrix is a structured conversation
   starter. If the result contradicts strong intuition from experienced stakeholders,
   examine the criteria and weights.

### When It Breaks Down

- **Incommensurable criteria.** Binary/existential factors ("Is this legal?") forced
  onto a 1-5 scale create false equivalence. Handle pass/fail criteria as screening
  filters *before* the matrix.
- **Strategic or values-based decisions.** "Should we pivot the company?" is not a
  weighted-scoring problem. The criteria are uncertain, interdependent, and emotional.
- **Deliberate manipulation.** Because the framework *looks* scientific, a bad actor
  can rig criteria, weights, or rubrics. Have multiple people validate weights.
- **Missing the fatal flaw.** An option scoring 1/5 on a mission-critical criterion
  but 5/5 on everything else has a high total. The matrix hides this unless you check
  minimum thresholds.

### Best Combinations

- **Decision Matrix + Pre-Mortem:** Matrix selects the winner; pre-mortem identifies
  failure modes the criteria may have missed.
- **Decision Matrix + RAPID:** RAPID defines who sets criteria (D), who scores (I),
  and who recommends (R). Prevents one person from controlling the whole matrix.
- **Decision Matrix + Second-Order Thinking:** After scoring, apply "and then what?"
  to the top 2 options. If #1's downstream consequences are worse, revisit criteria.

---

## 3. Pre-Mortem (Gary Klein)

**Solves:** Surfacing risks that normal planning suppresses because people do not want
to sound negative or disloyal. Research shows prospective hindsight increases risk
identification accuracy by ~30%.

**Does NOT solve:** Unknown unknowns, risks no one on the team can imagine, or
strategy quality.

### When to Use

- Before committing to a plan with significant investment or irreversibility
- When team cohesion or leadership authority might suppress dissent
- At project kickoff, and again at major stage gates
- When the plan "feels" too smooth — everything working perfectly is a warning sign

**Skip it when:** The initiative is too vague to imagine realistic failure, or the
team lacks enough context to generate specific risks.

### Step-by-Step Workflow

1. **Assemble the full project team.** Include all key contributors, not just
   leadership. Cognitive diversity is the entire point.

2. **Present the plan briefly.** Everyone must understand what "success" looks like
   before imagining failure. Timeline, milestones, success criteria.

3. **Set the scene (the "crystal ball" moment).** Facilitator says: *"It is 6 months
   from now. This project has failed catastrophically — not a minor setback, a
   disaster. People are not talking to each other. We wish we had never started.
   Your job: explain why it failed."* The dramatic framing gives permission to name
   fears.

4. **Individual silent writing (3 minutes, strict).** Each person writes reasons for
   failure. **Silent and individual** — no discussion, no looking at others' lists.
   This prevents anchoring and groupthink. Time pressure forces gut-level intuitions.

5. **Round-robin sharing.** Each person shares ONE item. Facilitator records on
   whiteboard. Continue cycling until all lists exhausted. Rules:
   - No debating or dismissing during sharing.
   - No "that's the same as X" — capture everything, deduplicate later.
   - Probe vague items: "Can you make that more specific?"
   - Most junior person shares first (prevents senior anchoring).

6. **Cluster and prioritize.** Group related items. Vote on top 5-7 risks by
   likelihood and impact. For each: assign owner, mitigation action, leading
   indicator, deadline.

7. **Integrate into the project plan.** Top risks become tracked items with review
   dates. Not a one-time exercise.

8. **Re-run every 3-4 months.** New information changes the risk landscape.

### Good vs Bad Output

**Good:**
```
Project: Launch mobile banking app by Q3

1. REGULATORY DELAY (8 votes)
   Fear: State regulators require 90-day review; we assumed 30 days.
   Owner: Legal (Maria)
   Mitigation: Submit pre-filing Week 2; parallel-path top 3 states.
   Leading indicator: No pre-filing response by Week 4.

2. THIRD-PARTY API INSTABILITY (7 votes)
   Fear: Payment processor's sandbox works but production has different
   rate limits we haven't tested.
   Owner: Platform architect (James)
   Mitigation: Load test against production-equivalent by March 15.
   Leading indicator: Rate limit errors in staging above 100 req/s.

3. INTERNAL TALENT GAP (6 votes)
   Fear: Two senior iOS devs are on other projects through May;
   "available" but no written commitment.
   Owner: Engineering manager (Priya)
   Mitigation: Get written commitment by Friday or begin contractor search.
   Leading indicator: No commitment email by EOW.
```

**Bad:**
```
Risks:
- Things might go wrong with the technology
- Team might not work well together
- Budget could be an issue
- Competition
- Market timing
Action: PM will keep an eye on these.
```

Why it fails: vague risks, no owners, no mitigations, "keep an eye on it" is magical
thinking.

### Common Mistakes

1. **Discussion during silent writing.** The moment someone speaks, they anchor the
   room. Enforce silence for the full 3 minutes.

2. **Senior leader shares first.** Sets the frame. Randomize order or have the most
   junior go first.

3. **Treating it as one-time.** A kickoff pre-mortem that never gets revisited is
   check-the-box ritual. Risks evolve.

4. **Self-serving attribution.** Participants blame external factors ("market shifted")
   not internal ones ("our planning was inadequate"). Facilitator should prompt:
   "Now imagine the failure was entirely our fault — what did *we* do wrong?"

5. **No follow-through.** Great risk list filed in a shared drive where no one looks.
   Every top risk needs an owner, a mitigation, a deadline, and a review mechanism.

### When It Breaks Down

- **Low psychological safety.** Fear of punishment produces sanitized, politically safe
  risks. The output looks complete but misses actual threats.
- **Homogeneous teams.** Same backgrounds surface same blind spots. Works best with
  cognitively diverse groups.
- **Black swans.** Pre-mortems surface risks people can *imagine*. Cannot surface
  truly novel risks. Creates false sense of completeness.
- **Overconfidence in mitigation.** Having mitigations on paper creates false security
  when the mitigations are untested or underfunded.

### Best Combinations

- **Pre-Mortem + Inversion:** Inversion asks "what would guarantee failure?" at a
  strategic level. Pre-mortem operationalizes it with a structured group process,
  owners, and mitigations.
- **Pre-Mortem + Second-Order Thinking:** After identifying top risks, map cascades.
  A regulatory delay doesn't just push the timeline — it triggers contractual
  penalties, then cash flow issues, then a hiring freeze.
- **Pre-Mortem + Decision Matrix:** Run the pre-mortem *before* finalizing matrix
  criteria. Risks often reveal criteria the matrix was missing.

---

## 4. Second-Order Thinking (Howard Marks)

**Solves:** Decisions where first-order benefits are obvious but downstream
consequences are easy to miss. Forces "and then what?" past the immediate reaction.

**Does NOT solve:** Novel situations with no historical precedent, or decisions
requiring speed over depth.

### When to Use

- Policy changes, pricing changes, org restructuring — anything with cascading effects
- When the first-order analysis looks too clean (all upside, no downside)
- When multiple stakeholders will *react* to the decision (customers, competitors,
  employees, regulators) and their reactions create further consequences
- Long time horizons where delayed effects dominate

**Skip it when:** Immediate crisis requires action, or the decision is easily
reversible.

### Step-by-Step Workflow

1. **State the decision clearly.** Write it down. "We will raise prices by 15%."
   "We will mandate return-to-office 5 days/week."

2. **Map first-order consequences.** All direct, immediate effects. These are what
   most people stop at.

3. **For each first-order effect, ask "And then what?"** Generate second-order effects:
   - "Revenue per unit increases → Some price-sensitive customers churn."
   - "Revenue per unit increases → Competitors see margin opportunity, enter market."

4. **Push to third order for highest-impact chains only.** Not every branch needs depth:
   - "Price-sensitive customers churn → They tell others, word-of-mouth turns
     negative → Customer acquisition cost rises."

5. **Apply the 10/10/10 filter:**
   - **10 minutes:** Immediate reaction?
   - **10 months:** Medium-term adjustment?
   - **10 years:** Structural/permanent change?

6. **Map stakeholder reactions.** How will customers, competitors, employees,
   regulators react? Their reactions create further consequences and feedback loops.

7. **Identify opposing desirabilities.** Flag decisions where first-order and
   second-order effects have *opposite* valence — feels good now, causes pain later.
   These are traps.

8. **Assign rough probabilities.** "Top performers leave" might be 70% likely;
   "competitors poach them specifically for our IP" might be 15%. Do not weight them
   equally.

9. **Decide with the full map in view.** The goal is not to avoid all second-order
   effects (impossible) but to decide with eyes open.

### Good vs Bad Output

**Good:**
```
Decision: Mandate return-to-office 5 days/week.

FIRST ORDER:
- More in-person collaboration (+)
- Better visibility of employee work (+)
- Employees unhappy about lost flexibility (-)

SECOND ORDER:
- Unhappy employees → top performers (who have options) leave first
  → talent quality declines → remaining team less productive
  (net negative even with more "visibility")
- Top performers leave → competitors hire them with remote offers
  → competitor capability increases, ours decreases
- More in-person → open-plan means more interruptions → deep work
  decreases → complex project velocity drops
- Mandate signals distrust → remaining employees disengage, do
  minimum viable work → "presence" increases but output decreases

THIRD ORDER:
- Talent exodus + disengagement → next product cycle slips → revenue
  target missed → pressure to cut costs → layoffs → further exodus
  (doom loop)

10/10/10:
- 10 minutes: Leadership feels good, "culture is back"
- 10 months: Regrettable attrition at 18% (vs 8% baseline)
- 10 years: Company known as rigid employer, structural hiring disadvantage

OPPOSING DESIRABILITIES: First-order feels productive; second-order is
destructive. Classic trap.

DECISION IMPLICATION: Keep flexibility; add 2-3 structured in-person
days for collaboration without mandating full return.
```

**Bad:**
```
Decision: Return to office.
Pros: Better collaboration, culture.
Cons: Some people won't like it.
Conclusion: Benefits outweigh costs.
```

Why it fails: only first-order effects, no "and then what?", no stakeholder reactions,
no time horizons, no opposing desirabilities. Indistinguishable from a pros/cons list.

### Common Mistakes

1. **Stopping at first order and calling it analysis.** If your analysis fits in a
   bullet list with no chains, you have not done second-order thinking.

2. **Treating all second-order effects as equally likely.** Assign rough probabilities.
   Not all cascades are probable.

3. **Only mapping negative effects.** Positive cascades exist too. A price increase
   might cause churn *and* signal quality to a premium segment.

4. **Analysis paralysis.** You can always ask "and then what?" one more time. Practical
   limit is 2-3 orders, going deeper only for highest-impact chains.

5. **Skipping incentives and adaptation.** People change behavior in response to rules,
   targets, and pricing. Model the reaction, not just the first effect.

### When It Breaks Down

- **Genuinely novel situations.** No historical precedent means second-order effects
  are speculative. May be worse than admitting ignorance.
- **Complex adaptive systems.** Markets, ecosystems, geopolitics — effects are
  non-linear and unpredictable. The map looks confident but the territory is chaotic.
- **Chesterton's Fence.** You map consequences of *changing* something without
  understanding what the *current* arrangement manages. Cannot reason about change
  without understanding the status quo.
- **Confirmation bias in chain construction.** People build cascades supporting their
  pre-existing position. Counter: assign someone to build the cascade for the
  opposing decision.

### Best Combinations

- **Second-Order + Inversion:** Inversion identifies what would guarantee failure.
  Second-order thinking maps *how* a good-looking decision cascades into that failure.
- **Second-Order + Pre-Mortem:** Pre-mortem generates risks; second-order thinking
  maps the cascade from each risk to downstream impacts.
- **Second-Order + Decision Matrix:** Matrix for structured choice, second-order
  thinking for causal stress-testing of the top 2 options.

---

## 5. Inversion (Munger / Jacobi)

**Solves:** Identifying avoidable failure paths. Many teams can spot what *not* to do
faster than they can design the perfect path to success. Munger: "It is remarkable how
much long-term advantage people like us have gotten by trying to be consistently not
stupid, instead of trying to be very intelligent."

**Does NOT solve:** What to pursue. Inversion tells you what to avoid — pair it with
forward-looking strategy.

### When to Use

- Before committing to a plan — check whether you are already on the failure path
- When a goal is clear but the path to it is not
- When you want to stress-test an existing plan for blind spots
- Post-merger integration, hiring processes, product launches — high-stakes with
  known failure patterns

**Skip it when:** Success depends on creativity or emergence more than on avoiding
failure, or the operating environment is so novel that failure modes are unknown.

### Step-by-Step Workflow

1. **Define the goal as a specific, measurable outcome.** "Increase customer retention
   to 90% by Q4." Not "improve retention."

2. **Invert the goal.** "What would *guarantee* customer retention drops to the worst
   possible level?" or "How could we ensure we *fail*?"

3. **Brainstorm failure causes — be specific.**
   - "Ignore support tickets for >48 hours"
   - "Ship buggy releases without testing"
   - "Raise prices without adding value"
   - "Make cancellation impossible (creates resentment, not retention)"
   - "Let competitors outpace feature development for 2+ quarters"

4. **Check current reality against the failure list.** For each item: *Are we already
   doing this?* This is where the power lies — you often discover you are partially
   executing the failure playbook.

5. **Convert failure causes into avoidance actions.**
   - "Ignore tickets" → "SLA: first response within 4 hours, resolution within 24"
   - "Ship buggy releases" → "Mandatory staging + 48-hour soak test before production"

6. **Prioritize by (a) how catastrophic and (b) how close you currently are to it.**

7. **Return to forward mode.** "Now that we know what to avoid, what positive actions
   drive us toward the goal?"

### Good vs Bad Output

**Good:**
```
Goal: Successful product launch Q3.

INVERTED: How do we guarantee this launch fails?

1. Ship without talking to customers → Did 3 interviews; need 15.
   PARTIALLY FAILING.
2. Launch to everyone with no beta → Current plan has no beta.
   CURRENTLY FAILING.
3. Marketing and product don't align on messaging → Last sync was
   6 weeks ago. PARTIALLY FAILING.
4. Set date from executive desire, not engineering readiness →
   Date is CEO's board commitment. CURRENTLY FAILING.
5. No rollback plan if critical bugs surface day 1 → No plan exists.
   CURRENTLY FAILING.

Reality check: We are executing 4 of 5 failure modes.

Avoidance actions (prioritized):
1. [URGENT] Add 2-week beta; delay launch if needed.
2. [URGENT] Create rollback plan with engineering by Friday.
3. [THIS WEEK] Schedule product-marketing alignment.
4. [THIS WEEK] Expand customer interviews to 15.
5. [NEXT SPRINT] Renegotiate launch date from fixed to range.

Forward actions:
- PR embargo with 5 journalists for launch week
- Customer success trained on new features by Week -2
```

**Bad:**
```
Goal: Successful launch.
What could go wrong: bugs, delays, competition.
Plan: Avoid those things.
```

Why it fails: no specificity, no reality check against current state, no prioritization.
"Avoid those things" is not actionable.

### Common Mistakes

1. **Using inversion as the only tool.** Inversion alone makes you excessively
   risk-averse. Always pair with forward strategy.

2. **Staying too abstract.** "Don't make mistakes" is inversion like "eat healthy" is
   a diet plan. Value is in specificity: "Guarantee failure by shipping without load
   testing our payment API above 500 concurrent users."

3. **Skipping the reality check.** Generating a failure list without checking current
   state against it turns inversion into an academic exercise. Most teams discover they
   are already doing several things on the list.

4. **Inconsistency avoidance (Munger's own warning).** Once committed to a decision,
   your brain resists finding flaws. Have *someone else* run the inversion on your plan.

### When It Breaks Down

- **Innovation and exploration.** Inversion is conservative — it focuses on avoiding
  downside. Breakthrough innovation often requires doing things that *look* like
  failures from a conventional inversion perspective.
- **Excessive risk aversion.** Overweighting inversion makes you see danger everywhere.
  Munger himself balanced inversion with aggressive betting when odds were favorable.
- **Unknown unknowns.** Can only surface failure modes you can imagine. The Titanic's
  designers inverted for most known failures — but not the specific combination of
  conditions that sank it.
- **Circular reasoning.** "How do we fail? By making bad decisions. How do we avoid
  failing? By making good decisions." In ambiguous domains, inversion can become
  tautological.

### Best Combinations

- **Inversion + Pre-Mortem:** Inversion is the individual mental model; pre-mortem is
  the group exercise that operationalizes it with owners and mitigations.
- **Inversion + Second-Order Thinking:** Inversion identifies failure modes;
  second-order thinking maps how current "good" decisions cascade into them.
- **Inversion + Decision Matrix:** Inversion generates criteria for the matrix. "What
  would make this fail?" surfaces criteria you would not find in forward mode.
- **Inversion + Profit Tree:** "What would guarantee costs increase and revenue
  decreases?" Then check which of those conditions exist.

---

## Combination Playbooks

### High-Stakes Strategic Decision

1. **Decision Matrix** — compare options with weighted criteria
2. **Second-Order Thinking** — stress-test top 2 options for downstream cascades
3. **Pre-Mortem** — surface execution risks on the likely winner
4. **RAPID** — clarify who recommends, approves, decides, and executes

### Operational Launch / Change Program

1. **RAPID** — lock decision rights before work begins
2. **Pre-Mortem** — expose execution failure modes with the full team
3. **Inversion** — create simple operating guardrails from the failure list

### Ambiguous Problem With Political Friction

1. **RAPID** — clarify roles if role confusion is blocking progress
2. **Inversion** — create a less defensive way to discuss failure
3. **Decision Matrix** — add only when options are mature enough for structured
   comparison

### Full-Stack Decision (High Stakes + Long Horizon + Org Complexity)

1. **RAPID** — who decides
2. **Decision Matrix** — structured option comparison
3. **Second-Order Thinking** — downstream consequence mapping
4. **Pre-Mortem** — execution risk identification
5. **Inversion** — reality check against current failure modes
