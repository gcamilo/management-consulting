# Innovation & Business Model Frameworks

Practitioner reference. Each framework: when to use, step-by-step workflow, good vs bad output, common mistakes, breakdown conditions, best combinations.

---

## 1. Jobs to Be Done (JTBD)

Demand-side innovation framework. Customers don't buy products -- they *hire* them to make progress in a specific life situation. Three schools: Christensen (disruption origin), Moesta (switch interviews), Ulwick (Outcome-Driven Innovation / quantitative). This guide synthesizes all three.

### When to Use

- Discovering why customers switch to or from solutions (and what they're really buying)
- Finding innovation opportunities in existing markets by identifying underserved outcomes
- Redefining market segmentation around jobs rather than demographics
- NOT for purely commoditized markets where cost is the only dimension, early-stage disruptive innovation where the job doesn't exist yet, or internal process optimization

### Step-by-Step Workflow

**Phase 1: Define the Market Around a Job**

1. **Write the core functional job.** Format: `[verb] + [object] + [contextual clarifier]`. Example: "get breakfast while commuting to work." No adjectives, adverbs, solutions, or technologies in the statement.
2. **Map the full job scope.** Functional job + emotional jobs ("feel confident I'm eating healthy") + social jobs ("appear responsible to coworkers") + consumption chain jobs (purchase, set up, maintain, dispose). Most teams only capture functional.
3. **Identify all job executors.** Buyer, user, and influencer may be different people with different jobs.

**Phase 2: Conduct Switch Interviews (12-15 minimum per segment)**

4. **Recruit "switch" customers.** People who recently switched to or from a solution -- they have the clearest memory of the forces at play. Also recruit non-consumers.
5. **Run the timeline interview.** Walk backward from the purchase moment:
   - First thought: "When did you first realize you needed something different?"
   - Passive looking: "What did you notice but not act on?"
   - Active looking: "When did you start deliberately searching?"
   - Decision: "What tipped you over?"
   - Post-purchase: "What surprised you after?"
6. **Capture the four forces in every switch story:**
   - Push of current situation (dissatisfaction)
   - Pull of new solution (attraction)
   - Anxiety of new solution (risk/uncertainty)
   - Habit of current situation (inertia)
7. **Stop when you hear the same forces repeated.** 12-15 interviews usually reach saturation.

**Phase 3: Extract Outcome Statements (Ulwick ODI method)**

8. **Write desired outcomes.** Format: `[direction] + [metric] + [object] + [context]`. Example: "Minimize the time it takes to verify breakfast is ready before leaving the house."
9. **Survey for importance and satisfaction** (n=200+, 1-10 scale each).
10. **Calculate opportunity scores.** Opportunity = Importance + max(Importance - Satisfaction, 0). Above 10 = underserved. Below 6 = overserved.

**Phase 4: Prioritize and Design Solutions**

11. Cluster underserved outcomes into opportunity segments.
12. Ideate solutions against specific underserved outcomes, not vague "needs."
13. Validate with prototypes measuring whether they improve the identified outcomes.

### Good vs Bad Output

**Job statements:**

| Quality | Statement | Why |
|---------|-----------|-----|
| GOOD | "Get breakfast while commuting to work" | Verb + object + context. Solution-free. |
| GOOD | "Pass on life lessons to children" | Aspirational, durable, solution-agnostic. |
| BAD | "Play MP3s" | Contains a solution (MP3). Real job: "listen to music while on the go." |
| BAD | "Manage cash flow" | "Manage" is a weak verb. Better: "Optimize cash flow to maintain solvency through seasonal dips." |
| BAD | "Users want to generate reports" | A task, not a job. Real job: "demonstrate progress to stakeholders." |

**Outcome statements:**

| Quality | Statement | Why |
|---------|-----------|-----|
| GOOD | "Minimize the likelihood the breakfast choice causes a mess while driving" | Direction + metric + object + context. Measurable, solution-free. |
| BAD | "Have a good breakfast experience" | Vague, subjective, no metric. |
| BAD | "The app should load faster" | Contains a solution ("the app"). Must be solution-agnostic. |

**Good job story (from switch interview):**
> "When I get home at 6 PM exhausted and see my kids asking 'What's for dinner?' while my partner is still commuting, I want to quickly prepare a nutritious meal everyone will eat, so I can avoid the guilt of ordering takeout again and actually sit down to enjoy dinner without a mountain of dishes."

This reveals: emotional burden, time constraint, desire for family connection, post-meal cleanup pain. Compare to the bad version: "When I'm hungry, I want to eat food, so I can be full."

### Common Mistakes

1. **Confusing tasks/activities with jobs.** "Generate a report" is a task. "Demonstrate progress to stakeholders" is the job. If you can ask "why?" and get a more fundamental answer, you haven't found the job. Teams that stop at the task level build incremental features instead of breakthrough products.
2. **Wrong level of abstraction.** Too broad: "live a healthy life" (life aspiration, not targetable). Too narrow: "find parking on 5th Avenue Tuesday mornings" (micro-task). Sweet spot: stable over time, solution-agnostic, guides product decisions. "Get to a destination on time" is well-calibrated.
3. **Retrofitting to justify existing features.** If discovered jobs perfectly align with your current feature set, you are almost certainly working backward. Genuine research should produce surprises -- jobs you didn't expect, substitute competitors you hadn't considered (the milkshake competing with a banana, a bagel, and boredom).
4. **Ignoring emotional and social dimensions.** Products that nail the functional job but miss the emotional one lose to competitors that address all three. The milkshake study found the job was partly "make the commute less boring" -- an emotional dimension.
5. **Interviewing the wrong people.** Satisfied, loyal customers produce feature requests, not job insights. The richest data: recent switchers, non-consumers, and people who "fire" your product.

### When It Breaks Down

- **Disruptive innovation.** Excellent at uncovering existing unmet needs but weaker at identifying entirely new categories. Starts from what people already try to do -- cannot easily surface jobs that don't exist because enabling technology doesn't exist.
- **Habitual/automatic behavior.** When a job is so deeply habitual people can't articulate it (brushing teeth, locking a door), interview-based research struggles. Use ethnographic observation instead.
- **Markets with network effects.** JTBD focuses on individual jobs, but in social networks and marketplaces, value depends on other users. Individual job framing misses the systemic dimension.
- **B2B with long decision chains.** When buyer, user, influencer, economic decision-maker, and end-beneficiary all have conflicting jobs, the framework becomes unwieldy. No built-in prioritization across competing stakeholders.

### Best Combinations

- **JTBD + Value Proposition Canvas**: JTBD interviews produce the jobs, pains, and gains that populate the VPC's customer profile. The strongest natural pairing -- Strategyzer designed the VPC for compatibility with JTBD.
- **JTBD + Design Thinking**: JTBD structures the Empathize and Define phases with rigor. Then use Design Thinking's prototyping loops for solution development.
- **JTBD + ODI (quantitative)**: Use qualitative interviews to discover jobs, then ODI's survey methodology to quantify opportunity. Qualitative + quantitative in sequence.
- **JTBD + Business Model Canvas**: JTBD fills Value Proposition and Customer Segment blocks; BMC forces you to think about channels, cost structure, and revenue.

---

## 2. Business Model Canvas (BMC)

Strategic management tool for describing, designing, challenging, and pivoting business models. Nine blocks. A thinking tool for structured debate, not a form to fill in.

### When to Use

- Designing a new business model or documenting an existing one for team alignment
- Comparing business models (current vs proposed, yours vs competitor's)
- Identifying the riskiest assumptions before committing resources
- NOT for execution planning (no sequencing), resource allocation (no prioritization), or competitive positioning (no external forces block)

### Step-by-Step Workflow

**Setup**

1. Large format: A1 poster or whiteboard. Sticky notes in 3-4 colors. Digital tools (Miro, Strategyzer) for remote; physical is better for first-timers.
2. **Label it**: "As-Is" (documenting) or "Hypothesis" (designing). Never mix current and future state on one canvas.
3. **One canvas per business model.** B2B and B2C models get separate canvases. Multi-sided platforms need one per side plus an integration view.

**Right Side First (Value Creation)**

4. **Customer Segments.** Be specific. Not "SMEs" but "SaaS companies with 10-50 employees that lack in-house finance teams, burning $200K-$500K/month." Color-code by segment to trace through the entire canvas.
5. **Value Propositions.** For each segment: what problem do you solve? What specific value? Each VP links to a specific segment. If a VP doesn't connect, delete it. Example: "Reduces month-end close from 12 days to 2 days for mid-market SaaS companies."
6. **Channels.** Map the full channel journey: awareness, evaluation, purchase, delivery, after-sales. Direct vs indirect.
7. **Customer Relationships.** Personal assistance, self-service, automated, community, co-creation. The nature of the relationship, not the channel.
8. **Revenue Streams.** For what value do customers pay? Pricing mechanism: fixed, negotiated, auction, usage-based? Assign dollar amounts. Example: "Annual subscription at $499/seat, targeting 500 seats Year 1 = $249,500 ARR."

**Left Side (Value Delivery)**

9. **Key Resources.** Only truly essential ones -- if removing it breaks the model, it's key.
10. **Key Activities.** What must you do exceptionally well? Production, problem-solving, platform management.
11. **Key Partnerships.** Why: optimization, risk reduction, resource acquisition, activity acquisition.
12. **Cost Structure.** Cost-driven vs value-driven? Fixed, variable, economies of scale/scope.

**Validate and Stress-Test**

13. **Check linkages.** Every segment needs at least one VP and one revenue stream. Everything left-side supports right-side.
14. **Add numbers.** Sticky notes are hypotheses until quantified. How many customers per segment? What price per stream? Refuse to leave without rough numbers.
15. **Identify the 3 riskiest assumptions.** Design experiments to test them within 2 weeks. The canvas without a validation plan is theater.

### Good vs Bad Output

**Customer Segments:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Series A SaaS founders (10-50 employees) with no CFO, burning $200K-$500K/month" | Specific, findable, reachable. |
| BAD | "SMEs" | Who? What industry? What size? Census category, not customer segment. |

**Value Propositions:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Delivers hot, fresh pizza within 30 minutes or it's free" | Specific, measurable, addresses clear pain, includes guarantee. |
| BAD | "Innovative and convenient solution" | Every startup says this. What specifically? |

**Revenue Streams:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Annual subscription $499/seat, 500 seats Y1 = $249,500 ARR" | Model, unit economics, and projection in one note. |
| BAD | "Subscription" | What kind? What price? Tells you nothing actionable. |

### Common Mistakes

1. **Treating it as a form, not a thinking tool.** Teams race through in 30 minutes with one note per block. A good session takes 2-4 hours, generates 50+ notes, and produces vigorous disagreement. If there was no argument, the session was superficial.
2. **Mixing current and future state.** "We have 200 enterprise customers" and "We'll have 2,000 community members" on the same canvas creates confusion. Use separate canvases, compare to define the migration path.
3. **Vague content without numbers.** "Millennials" is not a segment. "Technology" is not a resource. The test: could a stranger read this and understand the business?
4. **No validation plan.** If the session doesn't end with "here are our 3 riskiest assumptions and how we test them this week," it was theater.
5. **Ignoring external forces.** The BMC has no block for competitors, substitutes, regulations, or macro trends. Pair with Porter's Five Forces or PESTEL.

### When It Breaks Down

- **Static snapshot in a dynamic world.** Markets shift but the canvas on the wall stays the same. Must be revisited quarterly.
- **No execution or sequencing logic.** Says "what" but not "in what order" or "how." Two identical canvases can have completely different risk profiles.
- **Forces ideas into nine boxes.** Genuinely novel models (platforms, decentralized orgs, open-source) don't always fit. The structure can constrain creative thinking.
- **Multi-sided platforms are awkward.** When customer segments are interdependent (riders/drivers, buyers/sellers), the canvas struggles with network effects and cross-side dependencies.
- **Missing strategic context.** No block for mission, competitive advantage, or strategic positioning. Two competitor canvases might look similar -- the BMC doesn't capture what makes one superior.

### Best Combinations

- **BMC + Value Proposition Canvas**: VPC zooms into the VP and Customer Segment blocks. Validate fit per segment via VPC, then return to BMC for the full operational model.
- **BMC + Lean Canvas**: Lean Canvas for early-stage validation (Problem, Solution, Key Metrics, Unfair Advantage). Graduate to BMC for operational scaling.
- **BMC + Porter's Five Forces / PESTEL**: Covers the external forces the BMC ignores. Run these before or alongside.
- **BMC + Financial Modeling**: Revenue Streams and Cost Structure are starting points. Build a spreadsheet turning qualitative blocks into P&L, cash flow, and unit economics. BMC without numbers is a story; with numbers, it's a plan.

---

## 3. Value Proposition Canvas (VPC)

A designed zoom-in on two BMC blocks: Value Proposition and Customer Segment. Diagnoses problem-solution fit by mapping what customers need against what you offer.

### When to Use

- Validating whether your product addresses real, prioritized customer needs
- Designing or refining a value proposition for a specific segment
- Identifying product gaps and innovation opportunities
- NOT for multi-stakeholder B2B with 5+ decision roles (need one canvas per role), emotional/status-driven products that resist structured analysis, or when customer needs are genuinely emergent

### Step-by-Step Workflow

**Phase 1: Customer Profile (Right Side -- Always Start Here)**

1. **Pick ONE customer segment.** Separate canvases per segment. Mixing is the #1 mistake.
2. **List Customer Jobs** in three categories:
   - Functional: "File quarterly taxes." "Onboard new hires within 2 weeks."
   - Social: "Appear competent to the board." "Be seen as innovative."
   - Emotional: "Feel confident the numbers are right." "Feel in control."
3. **List Pains** in three categories:
   - Undesired outcomes: "Report has errors." "New hire quits in month 1."
   - Obstacles: "Need 6 departments to approve." "No budget until Q3."
   - Risks: "Audit finding." "Bad hire damages team morale."
4. **List Gains** in four categories:
   - Required: minimum for solution to work. "Filing is accepted by IRS."
   - Expected: standard expectation. "Filing completed within 2 hours."
   - Desired: would love but don't expect. "Automatic deduction detection."
   - Unexpected: beyond imagination. "Proactive planning saves $50K."
5. **Rank each list by intensity.** Mark top 3-5 per category. People decide for 1-2 reasons and rationalize the rest.

**Phase 2: Value Map (Left Side)**

6. **List Products & Services.** Concrete: "Automated quarterly tax filing software" not "innovative solution."
7. **List Pain Relievers.** For each top pain, how specifically does your offering alleviate it? Test: "How does the customer's life change?" If you can't answer specifically, it's a feature, not a pain reliever.
8. **List Gain Creators.** Same test. Be concrete and quantified: "Reduces filing from 12 hours to 45 minutes" not "saves time."
9. **Rank each list** by importance.

**Phase 3: Fit Assessment**

10. Draw explicit connections from pain relievers to specific pains, gain creators to specific gains.
11. Score fit quality. Strong fit = your top relievers address their top pains.
12. Identify gaps. Which top pains have no reliever? Those are your biggest opportunities.
13. Check for "phantom fit." Are connections validated by customers or assumed? Mark hypotheses.

**Phase 4: Validation**

14. Design cheapest, fastest tests: 15 customer interviews beat 1,000 surveys. Landing page tests. Concierge MVPs.
15. Iterate. Update canvas after validation. Remove invalidated assumptions.

### Good vs Bad Output

**Pains:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Current process requires manually reconciling 6 spreadsheets, taking 12+ hours, errors 40% of the time" | Quantified activity burden + failure rate. |
| BAD | "The process is slow" | How slow? Compared to what? Vague pains produce vague solutions. |

**Pain Relievers:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Auto-imports from all 6 sources, reconciles in 3 minutes, flags discrepancies for review" | Directly addresses the specific pain. Quantified. |
| GOOD | "7.9L/100km fuel economy saves $15/week" | Translates feature into concrete monetary impact. |
| BAD | "Our software is fast" | Compared to what? Marketing copy, not a pain reliever. |
| BAD | "Clean taxi" (when the pain is "dirty taxi") | Flipping a pain into its opposite is lazy. Produces commodity value propositions. |

**Gain Creators:**

| Quality | Content | Why |
|---------|---------|-----|
| GOOD | "Proactively identifies $12K-$50K in missed deductions based on industry benchmarks" | Unexpected gain. Quantified. Goes beyond what customer asked for. |
| BAD | "Saves time" | How much? On what? Indistinguishable from competitors. |

### Common Mistakes

1. **Mixing segments on one canvas.** Startup founder and enterprise CFO have different jobs, pains, gains. Combined canvas serves neither.
2. **Starting with the Value Map (left side).** Teams want to talk about their solution. If you start with your product, you unconsciously shape the customer profile to match what you already built. Always start with customer side, informed by interviews.
3. **Listing features instead of pain relievers.** "256-bit encryption" is a feature. "Your data has never been breached in 10 years, SOC 2 certified" is a pain reliever. Test: can you complete "This means you can now..."?
4. **Trying to address every pain and gain.** A focused VP addresses 3-5 brilliantly. The "Swiss Army knife" does everything, excels at nothing. Customers buy for 1-2 compelling reasons.
5. **No competitive context.** If your competitor already offers the same pain reliever, it's table stakes, not a differentiator. The VPC has no built-in competitive comparison.

### When It Breaks Down

- **Emotional and status-driven value.** The structured format favors functional analysis. Luxury, identity, and community products are awkward on the VPC.
- **Complex B2B with multiple stakeholders.** User, buyer, IT security, CFO all have different jobs/pains/gains. Need a canvas per role plus a meta-view of the buying committee.
- **Overconfidence from "fit."** Drawing lines between pains and relievers creates a visual sense of completeness. Those connections are hypotheses until validated with real customers.

### Best Combinations

- **VPC + JTBD**: JTBD interviews produce the raw material (jobs, pains, gains) for the customer profile. Without JTBD, the profile is guesswork.
- **VPC + Business Model Canvas**: VPC validates fit per segment; BMC maps the full operational model. Cycle between both.
- **VPC + Lean Startup**: Every unvalidated item is a hypothesis. Lean Startup's build-measure-learn loop tests the riskiest assumptions.
- **VPC + Competitive Analysis**: For each pain reliever and gain creator, note what competitors offer. Exposes differentiation vs parity.
- **VPC + Pricing Research**: Gain creators suggest willingness to pay. Pair with Van Westendorp or conjoint to quantify and set pricing.

---

## 4. BCG Advantage Matrix

Classifies *industries* (not companies) based on the nature of competitive advantage available. Two axes: number of approaches to achieve advantage (few vs many) and size of potential advantage (small vs large). Four quadrants with distinct strategic implications.

### When to Use

- Determining the right competitive strategy for an industry or segment (scale vs differentiation vs niche)
- M&A due diligence: understanding what kind of competitive game the target operates in
- Portfolio resource allocation across businesses in different industry types
- Identifying quadrant migration opportunities (the highest-value strategic insight)
- NOT for company-level positioning, execution planning, or industries undergoing rapid tech disruption

### Step-by-Step Workflow

**Phase 1: Define Unit of Analysis**

1. Specify what you're classifying: industry, business unit, product line, or geography. The matrix applies to competitive arenas, not companies. The same company might be in "Volume" for one segment and "Specialized" in another.
2. Set the decision context: growth investment, M&A posture, operating model design?
3. Time horizon: 3-5 years typical.

**Phase 2: Assess the Two Dimensions**

4. **Number of approaches to achieve advantage (Y-axis).**
   - How many distinctly different successful business models coexist? If most winners look alike (same strategy, different scale), approaches are "few." If winners look very different, approaches are "many."
   - Commodity steel: winners are almost all low-cost producers (few). Restaurants: fine dining, fast casual, fast food, ghost kitchens, chains, independents (many).

5. **Size of potential advantage (X-axis).**
   - How much difference can the best player create over the average? Measure in ROIC spread or market share concentration.
   - If best performer earns 30% ROIC and average earns 8%, advantage is large. If spread is 12% to 10%, advantage is small.
   - High concentration (top 3 hold 60%+ share) suggests large advantages. Fragmented share (no player above 5%) suggests small advantages.

**Phase 3: Classify**

|  | Few Approaches | Many Approaches |
|---|---|---|
| **Large Advantage** | **Volume** (scale dominates) | **Specialized** (multiple paths to superior returns) |
| **Small Advantage** | **Stalemate** (thin margins, price competition) | **Fragmented** (many ways to compete, none durable) |

**Phase 4: Strategic Implications**

- **Volume**: Pursue scale aggressively. Invest in capacity, standardize, consolidate. Market share = primary objective. Examples: semiconductors, commercial aircraft, cloud computing.
- **Specialized**: Invest in distinctive capabilities -- brand, IP, data, talent. Compete on uniqueness, not price. Multiple competitors can thrive differently. Examples: specialty pharma, luxury goods, professional services.
- **Fragmented**: Large-scale advantage is difficult. Compete locally or in niches. Strategies: operational excellence, franchise models, roll-ups, or platform plays to shift toward Volume. Examples: restaurants, hair salons, residential brokerage.
- **Stalemate**: Cost discipline and capital efficiency. Don't over-invest in differentiation. Manage for cash flow, not growth. Consider consolidation. Examples: bulk chemicals, commodity paper.

**Phase 5: Migration Analysis (highest-value insight)**

Ask: "What would have to be true for this industry to be in a different quadrant?" If the answer involves plausible changes (new tech, regulation, platform entry), your strategy must account for potential migration. Example: ride-hailing migrated from Fragmented (local medallion systems) to Volume (network effects: more drivers = shorter waits = more riders).

### Good vs Bad Output

**Good classification:**
> "US commercial airlines: Stalemate. Few viable strategies (hub-and-spoke vs point-to-point, both competing on cost/route), small durable advantage (top performers 12-15% ROIC vs average 8-10%, spreads narrow in downturns). Implication: cost discipline, capacity management, avoid differentiation investment that doesn't stick."

**Good migration analysis:**
> "Taxi/ride-hailing migrating Fragmented -> Volume. Pre-2012: local operators, no scalable advantage. Post-Uber/Lyft: network effects create scale advantages. Evidence: 2-player concentration in most markets. Implication: independents face structural disadvantage; compete on niche segments or exit."

**Bad:** "Airlines: Volume business because they're big." Confuses company size with industry quadrant. "Restaurants: Fragmented" (with no evidence). Correct label but useless without reasoning and implications.

### Common Mistakes

1. **Confusing company characteristics with industry characteristics.** A small company in a Volume industry is not in a Fragmented industry -- it's a disadvantaged player in a Volume industry. The quadrant describes the arena, not the player.
2. **Static classification.** Industries migrate over time. Digital platforms move fragmented industries toward volume. Treating classification as permanent leads to strategic errors.
3. **Using anecdotal evidence.** "I can think of five strategies" often collapses into 2-3 viable ones when profitability data is examined. Use ROIC spreads and concentration data.
4. **Ignoring within-quadrant heterogeneity.** Automotive = Volume at mass-market but Specialized at luxury. Pharma = Specialized in branded drugs, Stalemated in generics.

### When It Breaks Down

- **Digital platform dynamics.** Platforms can simultaneously exhibit volume (scale in matching) and specialization (niche verticals). Amazon has both massive scale advantages AND differentiated capabilities.
- **Ecosystem competition.** When competition is ecosystem-vs-ecosystem (Apple vs Google), industry-level classification breaks down.
- **Two-dimensional reduction.** Network effects, data advantages, regulatory moats, switching costs are all compressed into two axes. Loses nuance.
- **No prescriptive depth.** Tells you "pursue scale" but not how, how fast, through what mechanisms.

### Best Combinations

- **Advantage Matrix + Porter's Five Forces**: Matrix classifies the industry type; Five Forces explains *why* (which forces create or limit advantage).
- **Advantage Matrix + Value Chain Analysis**: In Specialized industries, identifies where differentiation resides. In Volume, where scale economies concentrate.
- **Advantage Matrix + Scenario Planning**: Since migration is the highest-value insight, stress-test: "Under what scenarios does this industry shift quadrants?"
- **Advantage Matrix + JTBD**: In Fragmented/Specialized, JTBD reveals the different jobs sustaining multiple strategies. In Volume, tests whether hidden segmentation creates specialization opportunities.

---

## Cross-Framework Integration Sequence

The four frameworks address different questions at different levels:

| Framework | Core Question | Level |
|-----------|--------------|-------|
| **Advantage Matrix** | What kind of competitive game are we playing? | Industry/strategy |
| **JTBD** | What is the customer trying to accomplish? | Customer/demand |
| **VPC** | How does our offering match what customers need? | Product-market fit |
| **BMC** | How do we deliver and capture value as a business? | Business model |

**Recommended sequence:**

1. **Advantage Matrix first** -- understand industry structure. Determines whether scale, differentiation, niche, or cost discipline is dominant.
2. **JTBD second** -- within that context, discover customer jobs. In Volume industries, look for the dominant job scale should serve. In Specialized, look for diverse jobs enabling multiple positions.
3. **VPC third** -- design a value proposition fitting discovered jobs, within strategic constraints.
4. **BMC fourth** -- build the operational model. Left-side (resources, activities, partners, costs) should reflect the Advantage Matrix posture (heavy capital for Volume, capability investment for Specialized).

Each step is informed and constrained by the previous one: macro structure -> customer needs -> solution design -> operational model.
