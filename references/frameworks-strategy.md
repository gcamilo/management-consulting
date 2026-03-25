# Strategy Frameworks -- Practitioner Reference

Eleven frameworks for strategy work. Each entry covers when to use it, step-by-step workflow, good vs. bad output, common mistakes, failure conditions, and best combinations. Examples use specific numbers, companies, and scenarios -- not textbook abstractions.

---

## Porter's Five Forces

### When to use
When you need to assess whether an industry (or segment within it) is structurally attractive -- i.e., whether participants can earn above-average returns. This is your first move for market entry, competitive positioning, or understanding why an industry's margins look the way they do.

### Step-by-step workflow

1. **Define the industry boundary precisely.** "US mid-market payroll software" is usable; "HR tech" is not. Too broad and you average away insight; too narrow and you miss adjacent threats. The test: do the firms in your boundary face the same five forces?

2. **Assemble a cross-functional team.** Best analyses include people from Sales (buyer dynamics), Procurement (supplier dynamics), Product (substitutes), and Strategy (new entrants, rivalry). Solo analysis from a strategy deck is inferior.

3. **Gather data before touching the framework.**
   - Industry reports (IBISWorld, Gartner, S&P Global) for market size, growth, key players
   - Public financials of major competitors, suppliers, and buyers for profitability, R&D spend, capital intensity
   - Expert interviews with industry veterans, former competitor employees, large customers, regulatory bodies
   - Customer surveys to understand price sensitivity, switching costs, perception of substitutes

4. **Analyze each force with structured evidence:**
   - **Threat of New Entrants:** Capital requirements, economies of scale, brand loyalty, switching costs, access to distribution, regulatory barriers, expected retaliation from incumbents
   - **Bargaining Power of Suppliers:** Supplier concentration, substitute inputs, supplier switching costs, threat of forward integration
   - **Bargaining Power of Buyers:** Buyer concentration, purchase volume per buyer, product differentiation, switching costs, price sensitivity, backward integration threat, information asymmetry
   - **Threat of Substitutes:** Alternatives serving the same job-to-be-done (not just same product category), price-performance ratio, switching costs, buyer propensity to switch
   - **Competitive Rivalry:** Number and balance of competitors, industry growth rate, fixed cost structure, exit barriers, product differentiation, strategic stakes

5. **Identify the 1-2 dominant forces.** Not all forces matter equally. Spending equal time on all five produces flat, uninformative analysis. Find the binding constraint on profitability.

6. **Quantify where possible.** Market share concentration (HHI or CR4), gross margin pressure, customer churn, CAC, switching costs in dollar terms, input concentration ratios.

7. **Synthesize force interaction.** High buyer power plus low switching costs compresses margins faster than either alone. The insight comes from how forces compound.

8. **Derive specific strategic actions.** For each dominant force, identify concrete moves: raise barriers to entry, reduce buyer power through differentiation, counter substitutes through switching costs, bundle to lock in distribution.

### Good output vs bad output

**Bad:** "Competition is intense and customers have choices, so the company should innovate and improve marketing."

**Good:** "In US domestic short-haul airlines, competitive rivalry is the dominant force. The top 4 carriers control 80% of capacity, but undifferentiated products and high fixed costs (aircraft leases, gate fees) trigger destructive fare wars on overlapping routes -- Southwest's entry into a route typically drops fares 30-40% within 6 months. Buyer power is structurally rising as fare aggregators (Google Flights, Kayak) make price comparison frictionless and switching costs are near-zero for leisure travelers. The strategic implication: compete on route-network density and loyalty lock-in (high-frequency business routes), not on fare -- every carrier that competed on price alone (People Express, ValueJet) was eventually absorbed or went bankrupt."

### Common mistakes

1. **Defining the industry wrong.** Too broad ("healthcare") mixes hospitals, pharma, devices, and payers into meaningless soup. Too narrow ("organic kombucha in Portland") misses the real competitive set. A product can be a Dog in "enterprise software" but a Star in "workflow automation for mid-market healthcare."

2. **Using it for internal strategy.** Five Forces analyzes industry structure, not your company's strengths. Practitioners constantly confuse "we have a strong brand" (internal) with "buyer power is low because of brand loyalty" (structural). The framework is outside-in only.

3. **Scoring forces without linking to concrete moves.** Every force rating must lead to a specific strategic action or explicit "no action needed" judgment. A completed Five Forces with no implications is a wasted exercise.

4. **Static snapshot bias.** The analysis reflects a moment in time. Digital disruption, regulatory shifts, and platform economics can restructure forces in 2-3 years. Always ask: "How are these forces changing?"

5. **Forgetting complements.** Porter's original model omitted complementors (Brandenburger & Nalebuff's addition). In platform and ecosystem businesses, complements are often more important than substitutes.

### When it breaks down

- **Platform and ecosystem businesses.** Two-sided markets (Uber, Airbnb, app stores) don't fit neatly -- are drivers suppliers or quasi-employees? Network effects create winner-take-all dynamics the model doesn't capture.
- **Hyper-dynamic industries.** In AI/ML, industry structure can shift within months. A static analysis is obsolete before the ink dries.
- **Cooperation-heavy industries.** The model assumes adversarial relationships. In industries with extensive co-opetition (semiconductors, pharma R&D partnerships), the zero-sum framing misleads.
- **When non-market forces dominate.** Five Forces says nothing about macroeconomic, political, or regulatory forces that can dwarf competitive dynamics (e.g., banking regulation, energy policy). Pair with PESTEL.
- **Very early markets where structure is still forming.** Forces have not stabilized enough to analyze meaningfully.

### Best combinations

- **PESTEL** -> **Five Forces** -> **Value Chain**: PESTEL identifies which macro shifts will reshape industry structure; Five Forces locates the structural pressure; Value Chain shows where to respond operationally.
- **Five Forces** -> **VRIO**: Outside-in then inside-out. Five Forces identifies where profit pools exist; VRIO tests whether you have the capabilities to capture them.
- **Five Forces** -> **Blue Ocean**: Five Forces reveals the structural constraints (the red ocean); Blue Ocean's ERRC redesigns around them.
- **Scenario Planning** -> **Five Forces** (per scenario): Test how industry structure changes under different futures. A force that is "low" today may be "high" under a plausible scenario.

---

## Value Chain

### When to use
When you need to understand where value is created, where cost accumulates, and which activities to invest in, outsource, or redesign. Most useful after you know the industry is attractive (Five Forces) and need to configure your operating model to capture profit.

### Step-by-step workflow

1. **Define the business model and profit logic.** State how the company creates value, captures margin, and serves customers. This anchors the entire analysis.

2. **Map all activities -- primary and support.**
   - Primary: inbound logistics, operations, outbound logistics, marketing & sales, service
   - Support: procurement, technology development, HR, firm infrastructure
   - For digital businesses, redefine primary activities as: Content/Data Acquisition, Platform Development, Distribution/Network, Monetization, Customer Success

3. **Break broad functions into real work.** "Operations" should become steps like sourcing, scheduling, assembly, QA, fulfillment, claims handling, or customer onboarding. Stopping at functional boxes is the most common failure.

4. **Assign costs to each activity.** Use activity-based costing where possible. What percentage of total cost does each activity represent? Without dollar figures, you are guessing -- a Value Chain without cost data is just a process diagram with labels.

5. **Identify value drivers per activity.** For each activity, ask: what does the customer actually care about here? Where does quality, speed, customization, or reliability matter most?

6. **Benchmark against competitors.** For each major activity, compare your cost and performance to the best competitor. Where are you significantly better or worse?

7. **Identify linkages between activities.** How do activities interact? A cheaper procurement choice might create quality problems in operations that increase service costs. The linkages are where competitive advantage often hides -- and where optimization in isolation causes damage.

8. **Decide the response by activity.** Standardize, automate, outsource, relocate, redesign, integrate, or invest to differentiate. Each choice must connect to a coherent market position.

### Good output vs bad output

**Bad:** "The company should optimize operations, improve marketing, and use technology to reduce costs."

**Good:** "Inbound logistics consumes 18% of COGS versus industry average of 12% -- root cause is fragmented supplier base (47 suppliers vs. competitor A's 12). Consolidating to 15 suppliers and implementing VMI would save $4.2M/year. However, this creates a linkage risk: current operations flexibility depends on supplier diversity for custom components. Recommendation: consolidate commodity inputs (80% of volume) while maintaining diverse sourcing for 6 specialty components. Net savings: $3.1M with no operations impact."

### Common mistakes

1. **Doing it without cost data.** A Value Chain analysis without activity-level cost allocation is just a process diagram with labels. You need actual dollar figures or percentages per activity.

2. **Ignoring linkages.** Optimizing one activity in isolation often degrades another. The classic: cutting procurement costs by choosing cheaper materials increases defect rates in operations and warranty claims in service.

3. **Confusing it with the customer journey.** The value chain maps internal activities and their costs. The customer journey maps external touchpoints and experiences. They overlap but are not the same -- optimizing operations efficiency might harm the customer experience.

4. **Applying it to digital/platform businesses without adaptation.** Porter designed this for manufacturing. In software, "inbound logistics" and "outbound logistics" have no analog. Redefine the categories or use Wardley Mapping instead.

5. **Looking only at cost and ignoring differentiation drivers.** The framework serves both cost advantage and differentiation advantage. An analysis that only finds cost savings misses half the picture.

### When it breaks down

- **Asset-light digital businesses** where value is co-created across ecosystems rather than a linear chain
- **Platform businesses** where value creation spans multiple firms (e.g., Apple's App Store ecosystem) -- you need value network analysis
- **Service and knowledge businesses** where the "product" is expertise and the manufacturing-oriented categories are awkward
- **Rapidly iterating startups** with no stable chain to analyze
- **When internal cost and process data are too poor** to support activity-level decisions

### Best combinations

- **Five Forces** -> **Value Chain**: Understand where profit is captured in the industry, then configure activities to capture it
- **Value Chain** -> **VRIO** (on key activities): Identify which activities create the most value, then test whether they constitute sustainable advantages
- **Value Chain** -> **7S**: Value Chain reveals the activity-level improvements; 7S reveals whether structure, systems, skills, and culture can support them
- **Blue Ocean** (ERRC) -> **Value Chain** redesign: ERRC defines what to eliminate/reduce/raise/create; Value Chain redesigns the operating model to deliver the new curve efficiently

---

## McKinsey 7S

### When to use
When an organization knows what it wants to do but is struggling to align execution. Diagnose why a strategy is failing by testing alignment across seven organizational elements. Most useful for transformation planning, M&A integration, or when a strategy shift requires organizational change.

### Step-by-step workflow

1. **Define the purpose.** Are you diagnosing a current misalignment, preparing for a merger, planning a transformation, or designing a new organization? The question shapes which elements you weight.

2. **Assess the seven elements with evidence -- current state:**
   - **Strategy:** What is the stated strategy? What is the *actual* strategy revealed by resource allocation?
   - **Structure:** Org chart, reporting lines, coordination mechanisms. Centralized vs. decentralized?
   - **Systems:** Budgeting, planning, performance management, IT, compensation, recruitment processes
   - **Shared Values:** Not the poster on the wall -- the values revealed by how people actually behave under pressure. What gets rewarded, what gets punished, who gets promoted.
   - **Skills:** Distinctive competencies of the organization as a whole, not just individuals
   - **Style:** How leaders actually spend their time. How decisions get made.
   - **Staff:** Talent profile, backgrounds, development paths -- not just headcount

3. **Test alignment between elements.** Focus on the most critical pairwise relationships rather than exhaustively scoring all 21 pairs. Ask: are these two elements mutually reinforcing or in tension?

4. **Identify 2-3 critical misalignments** that have the most downstream impact on strategy execution.

5. **Design the target state.** Start with hard elements (Strategy, Structure, Systems) since they are more directly changeable, but recognize that lasting change requires shifting soft elements.

6. **Sequence changes.** Systems, structure, and staff changes often need to precede behavior and culture shifts. But sometimes a system change (e.g., new incentive plan) is the lever that shifts behavior faster than a values campaign.

7. **Assign owners and milestones.** Reassess after implementation to catch secondary misalignments.

### Good output vs bad output

**Bad:** "Culture needs to improve and the organization must become more agile."

**Good:** "Critical misalignment: Strategy calls for rapid product innovation (launch 4 products/year), but Structure is a functional hierarchy where every new product requires sign-off from 5 VP-level gates (average approval cycle: 14 weeks). Systems reinforce the problem -- the stage-gate process was designed for a 2-product-per-year cadence and penalizes 'failures' in annual reviews. Staff in product are increasingly demoralized (38% voluntary turnover in 18 months) because stated strategy ('move fast, innovate') conflicts with lived experience ('get approval, don't fail'). Fix sequence: (1) Restructure product teams as autonomous squads with P&L ownership; (2) Replace stage-gate with a venture-board funding model; (3) Redesign performance reviews to reward experimentation, not just launch success."

### Common mistakes

1. **Describing elements without testing alignment.** Listing each S is not analysis. If you haven't identified misalignments, you haven't used the framework.

2. **Ignoring soft elements.** Organizations over-invest in changing Strategy, Structure, and Systems while leaving Style, Staff, Skills, and Shared Values unchanged. Culture eats strategy for breakfast.

3. **Treating it as a culture exercise rather than an alignment diagnosis.** The point is to find specific, fixable gaps between what the strategy demands and what the organization delivers -- not to write an essay about culture.

4. **Analysis paralysis.** With 7 elements and 21 pairwise relationships, teams can spend months mapping. Timebox the assessment (2-3 weeks) and focus on the 3-5 most impactful misalignments.

5. **Assuming Shared Values are what leadership says they are.** The real shared values are revealed by behavior -- what stories are told, who gets promoted, what gets punished. Corporate value statements are often disconnected from organizational reality.

### When it breaks down

- **When the strategy itself is unclear or wrong.** 7S assumes the strategy is sound and tests organizational alignment to it. If the strategy is the problem, 7S will align the organization around the wrong target.
- **Externally driven disruptions.** 7S is entirely internal. Perfect alignment won't save you from industry disruption. Pair with an external framework.
- **Startups (<50 people)** that don't have formalized systems, structures, or processes. The framework adds overhead without insight.
- **Crisis situations** where immediate operational fixes matter more than alignment mapping.
- **When the root cause is leadership.** If the CEO is the misalignment (autocratic style undermines collaborative strategy), the framework identifies it but the solution is a people problem.

### Best combinations

- **Value Chain** -> **7S**: Redesign the work first, then align the organization around it
- **Three Horizons** -> **7S**: Choose bets first, then prepare the organization to support them
- **7S** -> **Nine-Box**: 7S identifies organizational capability gaps; Nine-Box assesses whether the leadership bench can execute the change
- **Five Forces + Value Chain** -> **7S**: Determine strategy and operating model, then test whether the organization can execute it

---

## VRIO

### When to use
When you need to determine which of your internal resources and capabilities actually constitute sustainable competitive advantages -- versus mere table stakes. Use after Five Forces (to know which advantages matter in your industry) and often after Value Chain (to know where in your operations the advantages sit).

### Step-by-step workflow

1. **Inventory resources and capabilities comprehensively.** Include tangible resources (patents, equipment, cash, proprietary data, real estate), intangible resources (brand reputation, organizational culture, institutional knowledge, relationships, trade secrets), and capabilities (rapid product development, supply chain optimization, customer analytics).

2. **Group into capabilities rather than random asset lists.** "Data" is not a capability; "proprietary underwriting models trained on 14 years of behavioral data" is.

3. **Apply the four tests sequentially for each capability:**
   - **V -- Valuable?** Does it help exploit opportunities or neutralize threats? If NO: competitive disadvantage. Stop.
   - **R -- Rare?** Is it controlled by only a small number of competitors? If NO: competitive parity (table stakes). Stop.
   - **I -- Costly to Imitate?** Sources: unique historical conditions, causal ambiguity, social complexity, patents/legal protections. If NO: temporary competitive advantage.
   - **O -- Organized to Capture Value?** Does the firm have processes, policies, structure, and culture to exploit this resource? If NO: unused competitive advantage (valuable, rare, hard to copy, but wasted). If YES: sustained competitive advantage.

4. **Gather proof for each rating.** Use win rates, margins, retention, speed, defect rates, NPS, patent position, installed base, or partner dependency. Assertions without evidence are confirmation bias.

5. **Distinguish threshold from differentiating capabilities.** Most "strengths" are only table stakes. If your VRIO table shows 8 out of 10 resources as "Sustained Competitive Advantage," you are not being rigorous.

6. **Identify gaps in the O (Organization).** A capability can be valuable, rare, and hard to copy but still under-monetized because incentives, governance, or go-to-market are weak. Xerox PARC invented the GUI, mouse, and ethernet, but Xerox was not organized to commercialize them. Apple and Microsoft captured the value.

7. **Decide what to build, protect, leverage, or stop overinvesting in.** Double down on defensible advantages; de-emphasize undifferentiated areas.

### Good output vs bad output

**Bad:** "Our people and brand are our biggest strengths and give us a competitive advantage."

**Good:** "Proprietary recommendation algorithm (trained on 14 years of behavioral data from 230M users): Valuable (drives 80% of content discovery, reducing churn by 23% vs. non-personalized), Rare (only 2 competitors have comparable data depth; new entrants need 5+ years to accumulate), Inimitable (causal ambiguity with 1,200 interacting features, path-dependent training data, $200M cumulative R&D), Organized (dedicated ML org of 300 engineers, A/B testing infrastructure, rapid deployment pipeline) -- Sustained Competitive Advantage. Original content library ($17B invested): Valuable (exclusive titles drive 45% of new sign-ups), Partially Rare (competitors now invest $10-20B/year), Not Inimitable (any well-capitalized competitor can commission similar content; hits are unpredictable), Organized -- Temporary Advantage, eroding as competitors match spend. Protect by leveraging recommendation engine to maximize content ROI."

### Common mistakes

1. **Rating everything as 'Yes' across the board.** Cognitive bias leads teams to overrate their own resources. Be brutally honest -- most resources are competitive parity.

2. **Confusing 'we have it' with 'valuable.'** Having a resource does not make it valuable. An extensive physical retail network was valuable in 2010 and a costly liability by 2020.

3. **Ignoring the O (Organization).** Many firms have VRI resources but fail to organize around them. This is where the real actionable insight lives.

4. **Static assessment.** Resources that are inimitable today may become commodity tomorrow. "How long until this advantage erodes?" is as important as "Is this currently inimitable?"

5. **Analyzing resources in isolation.** Resources often create advantage in combination, not individually. Amazon's advantage is not logistics OR data OR brand -- it is the specific combination and how they reinforce each other.

### When it breaks down

- **Fast-changing industries** where "Rare" and "Inimitable" can flip within months as new technology arrives
- **Markets where advantage is transient** and imitation cycles are very short (e.g., fashion, mobile apps)
- **Network-effect businesses** where the advantage is the network itself, which doesn't fit neatly into VRIO categories
- **When the market disappears.** A perfectly organized, rare, inimitable resource is worthless if the entire market evaporates (Kodak's film processing capabilities)
- **When there is no evidence base** and the exercise becomes self-congratulatory

### Best combinations

- **Five Forces** -> **VRIO**: Outside-in then inside-out. Five Forces identifies profit pools; VRIO tests whether you can capture them.
- **Value Chain** -> **VRIO** (on key activities): Identify where value is created, then test which activities are defensible
- **VRIO** -> **Ansoff**: Know your true capabilities before choosing growth directions. VRIO prevents choosing quadrants you can't execute in.
- **Wardley Mapping** -> **VRIO**: Wardley identifies what might still be strategic vs. commoditizing; VRIO tests defensibility of the strategic components

---

## Three Horizons of Growth

### When to use
When you need to balance short-term earnings with long-term growth bets. Diagnoses whether a company is over-investing in today's business at the expense of tomorrow's, or spreading bets too thinly across time horizons. Most useful for portfolio allocation, innovation strategy, and board-level resource decisions.

### Step-by-step workflow

1. **Catalog current revenue sources and their trajectories.** For each business line: current revenue, growth rate, market maturity, competitive position, estimated remaining profitable life.

2. **Classify into horizons:**
   - **H1 (Defend & Extend):** Core businesses generating majority of current profit. Mature, well-understood. Task: maximize cash generation, extend life, defend share. Metrics: revenue, margin, cash flow, market share.
   - **H2 (Build):** Emerging businesses with demonstrated traction but not yet at scale. Task: scale rapidly, build competitive position. Metrics: revenue growth rate, CAC payback, market penetration, repeatability.
   - **H3 (Create):** Seeds, options, experiments. Task: explore, create options. Metrics: learning velocity, experiments run, option value. NOT revenue.

3. **Map current resource allocation across the three horizons.** The most common failure: H1 consuming >90% of all resources, starving H2 and H3.

4. **Define different success metrics by horizon.** Applying H1 metrics (ROI, market share) to H3 experiments is like grading a kindergartener on SAT scores. Each horizon needs its own metrics.

5. **Build a migration pipeline.** H3 experiments that validate graduate to H2 with dedicated funding. H2 businesses that reach scale graduate to H1. H1 businesses in decline are harvested or divested. Define explicit graduation criteria and the "valley of death" between stages.

6. **Assign distinct governance and leadership.** H1 = operational excellence; H2 = entrepreneurial scaling; H3 = exploratory and experimental. Forcing all three through the same governance process kills H2 and H3.

7. **Establish transition plans.** The real work is moving ideas from H3 to H2 and then into H1 without losing sponsorship.

### Good output vs bad output

**Bad:** "The company should focus on short term and long term growth at the same time."

**Good:** "H1 ($3.2B, 78% of revenue): Enterprise CRM platform -- 92% renewal rate, but growth slowing to 4% as market saturates. Extracting $380M free cash flow annually to fund H2/H3. H2 ($420M, 10%): AI-powered sales analytics -- growing 65% YoY, CAC payback at 14 months (target: 12). Needs $120M investment this year to reach profitability by Q3 2027. Graduation criteria: positive unit economics for 2 consecutive quarters. H3 ($48M, 1.2%): Three bets -- (a) Autonomous deal negotiation agent ($18M, 2 enterprise pilots), (b) Vertical CRM for healthcare ($22M, FDA pre-submission), (c) Developer platform ($8M, alpha). Each capped at $30M before requiring H2 graduation or kill decision. Resource allocation shift: moving from 92/6/2 to 78/15/7 over 18 months by redeploying 40 engineers from H1 feature maintenance to H2/H3."

### Common mistakes

1. **Starving H2 and H3.** H1 managers have political power and demonstrable revenue -- they win budget battles. Fix: ring-fence H2/H3 budgets at the board level.

2. **Using horizons as time labels only instead of different business logics.** The original model assumed H3 takes years. Steve Blank's critique: ChatGPT went from research project to 100M users in 2 months. Horizons should be defined by business model maturity, not calendar time.

3. **Forgetting the transition path.** The "valley of death" between H3 experimentation and H2 scaling is where most innovations die. They get too big for the innovation lab but too small for the business unit to care about.

4. **H1 co-opting H2/H3 innovations.** The existing business absorbs emerging innovations to extend its own life rather than letting them mature into separate businesses. Rational for H1 managers but kills transformational potential.

5. **Treating H3 concepts as strategies before they have evidence.** H3 bets are options, not commitments. They need learning milestones, not revenue targets.

### When it breaks down

- **Turnaround situations** where H1 survival overwhelms everything else. You don't have the luxury of H3 exploration.
- **Single-product companies** where the framework doesn't add much -- you need product roadmap management, not growth horizons.
- **When disruption comes from outside.** If a competitor leapfrogs from H3 to H1 in your industry, your orderly horizon progression is irrelevant.
- **Highly regulated industries** (pharma) where "horizons" are dictated by regulatory timelines (10-15 years), not business model maturity.

### Best combinations

- **Ansoff** -> **Three Horizons**: Ansoff defines the type of growth move; Horizons stages investment across time. H1 maps to market penetration, H2 to market/product development, H3 to diversification.
- **BCG Matrix** (concurrent): BCG classifies by current position; Horizons classifies by time-to-value. Cash Cows = H1, Stars = H1-H2, Question Marks = H2-H3.
- **Scenario Planning** -> **Three Horizons**: "What if H1 revenue declines 40% in 2 years?" Scenarios reveal whether horizon allocation is resilient or fragile.
- **7S** -> (after Horizons): Once new bets are chosen, 7S helps align the organization to support them.
- **Lean Startup** within H3: H3 experiments should use build-measure-learn loops, not stage-gate processes.

---

## Ansoff Matrix

### When to use
When you need to evaluate and compare growth options. Forces clarity on whether you are growing via market penetration, market development, product development, or diversification -- and makes the risk differential explicit. Most useful when the CEO says "we need to grow" and the team needs to prioritize among competing directions.

### Step-by-step workflow

1. **Audit your current position.** Define specifically:
   - What are your existing products/services? (Specific, not categorical)
   - What are your existing markets? (Geography, customer segment, channel)
   - What is your current performance in each product-market combination?

2. **Clarify what counts as "new."** Teams often blur incremental extensions with true newness. When is a product "new" vs. an extension? When is a market "new" vs. an adjacent segment? Define upfront to avoid classification debates.

3. **Populate each quadrant with specific options:**
   - **Market Penetration** (existing products, existing markets): Pricing, promotion, distribution expansion, loyalty, competitive displacement. Lowest risk. Ask: "Can we sell more of what we already have to customers we already serve?"
   - **Market Development** (existing products, new markets): New geographies, customer segments, channels. Ask: "Can we take what we already have to customers we don't yet serve?"
   - **Product Development** (new products, existing markets): New features, extensions, adjacent products for current customers. Ask: "Can we create something new for customers who already trust us?"
   - **Diversification** (new products, new markets): Related (leveraging existing capabilities) or unrelated (conglomerate plays). Highest risk.

4. **Estimate risk, capability gaps, and expected returns for each option.** Test strategic fit: does the move use existing channels, customers, capabilities, brand permission, or cost advantages?

5. **Prioritize and sequence.** Select a maximum of 2 strategies as primary focus. Apply the 70-20-10 rule: 70% resources on penetration, 20% on one medium-risk strategy, 10% on exploratory diversification.

6. **Define milestones and kill criteria for each selected move.** Each option needs: specific target, investment required, timeline, success metrics, and conditions under which you walk away.

### Good output vs bad output

**Bad:** "We should grow through new products and new markets."

**Good:** "Market Penetration (priority, 75% resources): Our B2B SaaS has 12% market share in mid-market (100-500 employees). Competitor X just lost their VP of Sales -- window to hire their top 3 reps and target their install base of 2,400 accounts. Target: 18% share in 18 months. Investment: $4.2M. Market Development (secondary, 20%): Product has 0% presence in DACH despite 3 inbound requests/week from German mid-market. Hire DACH country manager, localize product (4 months), partner with 2 local resellers. Target: 200 DACH customers in 12 months. Diversification (parked): Enterprise segment (>5,000 employees) requires fundamentally different architecture and sales motion. Not pursuing now -- would require $15M+ with 24+ month payback. Revisit Q3 2027 after DACH proves out."

### Common mistakes

1. **Pursuing all four quadrants simultaneously.** Spreading resources across all quadrants guarantees mediocre execution in all. Focus beats breadth.

2. **Underestimating Market Penetration.** Teams gravitate toward exciting quadrants (new markets, new products) while leaving 5-15% market share gains on the table. Penetration is usually highest ROI and should be exhausted before expanding.

3. **Treating Diversification as one category.** Related diversification (leveraging capabilities) and unrelated diversification (conglomerate plays) have wildly different risk profiles. Related diversification with clear capability leverage can be lower risk than market development in a radically different geography.

4. **Not linking to capabilities.** The matrix shows directions, not feasibility. Without assessing resources and skills for each option, you are choosing direction without checking fuel in the tank.

5. **Ignoring competitive response.** The matrix considers your options in isolation. A market penetration play through aggressive pricing may trigger a price war that destroys industry profitability.

### When it breaks down

- **Platform businesses** where the distinction between product and market is blurry -- the matrix assumes you sell products to markets
- **When "new" and "existing" aren't binary.** A SaaS company selling an AI add-on to existing customers -- is that product development or penetration? The binary framing forces artificial classification.
- **Rapidly converging industries** where industry boundaries blur (fintech + banking, healthtech + healthcare)
- **It does not assess brand elasticity.** A luxury brand diversifying into low-end products may destroy brand equity -- a risk the matrix doesn't surface.

### Best combinations

- **VRIO** -> **Ansoff**: Understand true capability advantages before choosing growth directions
- **Five Forces** -> **Ansoff**: Understand industry attractiveness before deciding which markets to enter
- **Ansoff** -> **Three Horizons**: Ansoff defines growth type; Horizons stages investment. H1 = penetration, H2 = development, H3 = diversification.
- **BCG** -> **Ansoff**: BCG identifies which units need growth; Ansoff specifies the direction
- **Ansoff** -> **Blue Ocean**: Ansoff identifies the quadrant; Blue Ocean's ERRC defines how to compete differently within it

---

## BCG Growth-Share Matrix

### When to use
When you need to evaluate a multi-business portfolio and make capital allocation decisions across units. Forces the question: which businesses deserve investment, which should generate cash, and which should be divested? Most useful for conglomerates, multi-product companies, or any firm with 4+ distinct business lines competing for capital.

### Step-by-step workflow

1. **Define the units of analysis.** Business units, product lines, brands, or individual products. Ensure comparable levels of aggregation.

2. **Define your market -- the most critical step.** The market definition determines relative market share. Too broadly ("beverages") and you look small; too narrowly ("organic cold-brew coffee in Brooklyn") and you look dominant. The right market is where you actually compete for the same customers.

3. **Calculate the two axes:**
   - **Market Growth Rate (vertical):** Annual growth of the *market* (not your revenue growth). Use 3-5 year projected growth. Threshold between "high" and "low" is typically GDP growth, company average, or 10%.
   - **Relative Market Share (horizontal):** Your share divided by the largest competitor's share. >1.0 means market leader. Logarithmic scale, not linear.

4. **Plot and classify:**
   - **Stars** (high growth, high share): Market leaders in fast-growing markets. Generate cash but consume it to maintain position.
   - **Cash Cows** (low growth, high share): Leaders in mature markets. Generate more cash than they consume.
   - **Question Marks** (high growth, low share): Small players in fast-growing markets. Cash-hungry, uncertain.
   - **Dogs** (low growth, low share): Weak in mature markets. Break-even at best.

5. **Add a reality layer.** Note margins, cash generation, reinvestment needs, strategic fit, synergies, and interdependencies. A "Dog" might be the loss leader driving acquisition for a "Star."

6. **Assess cash flow balance.** Cash Cows should fund Stars and selected Question Marks. All Question Marks and no Cash Cows = cash crisis. All Cash Cows and no Stars = growth crisis.

7. **Make allocation decisions.** Invest (grow share), Hold (maintain), Harvest (milk for cash), or Divest. For Question Marks: pick the best and fund heavily enough to become Stars; divest the rest.

### Good output vs bad output

**Bad:** "Cash Cows are good, Dogs are bad, so we should invest in Stars and exit Dogs."

**Good:** "The portfolio is dangerously unbalanced: 62% of revenue from two Cash Cows (legacy on-premise ERP and payroll processing), both in markets growing <2%. Only one Star (cloud HCM platform, 14% share vs. Workday's 28%, market growing 22% YoY) consuming $180M/year against Cash Cow free cash flow of only $210M. Question Mark: AI recruiting tool -- market growing 45%, but <2% share and 11 funded competitors. Decision: increase cloud HCM investment to $240M (reduce Cash Cow dividend by $30M, defer on-premise feature requests) to close the Workday gap while market still grows. Kill the AI recruiting tool -- insufficient differentiation, too many funded competitors, and funding it would starve the Star. Redeploy the 40-person AI recruiting team to cloud HCM."

### Common mistakes

1. **Using company revenue growth instead of market growth.** The vertical axis is *market* growth. Your revenue can grow 30% while the market grows 5% -- that's a Cash Cow gaining share, not a Star.

2. **Underfunding Question Marks by spreading investment.** The matrix says pick the best Question Marks and fund them heavily. Companies instead give a little to each -- none gets enough to gain share, and all fail. Be selective and decisive.

3. **Poor market definitions making growth and share numbers meaningless.** This is the same problem as in Five Forces -- garbage market definition, garbage quadrant placement.

4. **Labeling units as Dogs and demoralizing teams.** Teams labeled "Dog" become self-fulfilling prophecies -- talent leaves, investment is withheld, performance declines. Use the analytical insight without destructive labeling.

5. **Ignoring interdependencies between units.** A "Dog" might be the loss leader that drives customer acquisition for a "Star." The matrix treats units in isolation and misses portfolio synergies.

### When it breaks down

- **When market share doesn't drive profitability.** The model assumes strong scale economics. This holds in commodity businesses but fails in differentiated businesses (luxury goods, where niche players outperform leaders on margin).
- **Network-effect businesses** with winner-take-all dynamics. No stable "Cash Cow" position -- you are either the dominant platform or irrelevant.
- **Software and platform businesses** where the classic share-profitability correlation is weak.
- **When business units are too interdependent** to evaluate on a standalone basis.
- **Academic evidence is mixed.** Slater & Zwirlein (1992) found firms following BCG-style portfolio planning had lower shareholder returns than firms that didn't.

### Best combinations

- **Five Forces** -> **BCG**: Test whether a high-growth market is structurally attractive. Prevents investing in fast-growing but structurally unattractive markets.
- **BCG** -> **Ansoff**: BCG identifies which units need growth; Ansoff specifies the direction (penetration, development, diversification)
- **BCG** + **Three Horizons** (concurrent): BCG by current position; Horizons by time-to-value. Cash Cows = H1, Stars = H1-H2, Question Marks = H2-H3.
- **BCG** -> **GE-McKinsey Nine-Box**: BCG as quick screen; Nine-Box for deeper analysis on the ambiguous cases

---

## GE-McKinsey Nine-Box Matrix

### When to use
When BCG's two dimensions (growth + share) are too simplistic for your portfolio decision. The Nine-Box uses multi-factor axes (Industry Attractiveness and Competitive Strength) with weighted scoring, giving a more nuanced but more labor-intensive assessment. Best for large portfolios where the invest/hold/harvest decision requires rigor beyond two variables.

### Step-by-step workflow

1. **Identify the business units to analyze.** Ensure comparable levels of aggregation.

2. **Define factors and weights for each axis:**

   **Industry Attractiveness (vertical):** Market size (15%), market growth rate (20%), industry profitability (20%), competitive intensity (15%), technology requirements (10%), regulatory environment (10%), cyclicality (10%). Weights must total 100% and reflect what actually drives long-term value.

   **Competitive Strength (horizontal):** Relative market share (20%), brand strength (15%), production capacity/efficiency (10%), profit margins vs. competitors (15%), technological capability (15%), management quality (10%), distribution strength (15%).

3. **Score each unit on every factor (1-5).** Define what a "1" and a "5" look like before scoring to reduce subjectivity. Document evidence behind each score.

4. **Calculate weighted scores.** Multiply each factor score by its weight, sum for composite score per axis. This gives (x, y) coordinates.

5. **Plot on the 3x3 grid.** Bubble size proportional to revenue.

6. **Apply zone prescriptions:**
   - **Green zone** (top-left 3 cells): High attractiveness, strong position. Invest for growth.
   - **Yellow zone** (diagonal 3 cells): Medium. Selective investment. Invest in units with clear improvement paths; hold or harvest others.
   - **Red zone** (bottom-right 3 cells): Low attractiveness, weak position. Harvest or divest.

7. **Plot trajectories.** Draw arrows showing projected movement. A market scoring "high" today may score "low" in 3 years.

### Good output vs bad output

**Bad:** "Business Unit A scored High/High -- invest. Unit B scored Medium/Medium -- hold. Unit C scored Low/Low -- divest."

**Good:** "Cloud Security (scored: Industry Attractiveness 4.3/5, Competitive Strength 3.1/5 -- upper-middle Yellow zone). Attractiveness breakdown: Market growing 28% CAGR (score 5, weight 20% = 1.0), high margins (score 4, weight 20% = 0.8), but intense competition with 40+ vendors (score 2, weight 15% = 0.3), favorable regulation via SEC cyber rules (score 5, weight 10% = 0.5). Competitive Strength breakdown: 3.2% share vs. Palo Alto's 9.8% (score 2, weight 20% = 0.4), but superior zero-trust technology (score 5, weight 15% = 0.75), weak distribution -- only direct sales, no channel (score 1, weight 15% = 0.15). Prescription: invest selectively. The gap is distribution, not technology. Add 3 channel partnerships with major SIs (Accenture, Deloitte, KPMG) within 6 months. If share reaches 5% by Q2 2027, reclassify as Green and increase investment 2x."

### Common mistakes

1. **Arbitrary factor weights.** Teams pick weights without connecting them to value drivers. Run sensitivity analyses: if changing a factor's weight from 10% to 20% doesn't change any unit's zone, it's not a meaningful factor.

2. **Scoring without calibration.** If different teams score their own units, each inflates scores. Solution: one cross-functional team scores all units, or explicit rubrics with examples per score level.

3. **Weighting political dynamics.** Business unit leaders lobby for weights that favor their unit. The weighting exercise becomes political negotiation rather than analytical exercise. Insulate weighting from unit-level advocacy.

4. **Treating zone prescriptions as rules.** A Red-zone unit might be strategically important as a loss leader, defensive play, or capability source. The matrix informs decisions; it does not make them.

5. **Small portfolios.** If you have 2-3 business units, you don't need a nine-box. The methodology overhead exceeds the benefit.

### When it breaks down

- **When the weighting exercise becomes subjective consensus.** Complex methodology, garbage inputs, confident-looking outputs -- precisely calibrated nonsense.
- **Diversified conglomerates with truly unrelated businesses.** Using the same attractiveness factors across healthcare, real estate, and software is inappropriate.
- **Rapidly evolving industries** where scores are stale by the time analysis completes.
- **When you lack data** to score factors credibly. Mathematical precision of weighted scores creates false confidence with guessed inputs.

### Best combinations

- **BCG** -> **Nine-Box**: BCG as quick screen; Nine-Box for deeper dives on ambiguous cases
- **Five Forces** feeds Industry Attractiveness axis: Five Forces provides scoring data for competitive intensity, entry barriers, buyer/supplier power
- **VRIO** feeds Competitive Strength axis: Resource-based advantages directly inform brand strength, technology capability scores
- **Scenario Planning** -> **Nine-Box** (stress-test): How do attractiveness scores change under different scenarios? A Green-zone unit under base case may be Red zone under a downturn.

---

## Blue Ocean Strategy

### When to use
When competition in your industry has become a zero-sum fight over the same customers on the same factors. You need to unlock demand from noncustomers by fundamentally redesigning the value proposition -- not by doing the same things better, but by doing different things. Most useful when industry margins are compressed, differentiation has converged, and price wars dominate.

### Step-by-step workflow

1. **Define the arena.** Product/service scope, buyer group (distinguish user, purchaser, and influencer), geography. Critically: identify the three tiers of noncustomers:
   - Tier 1: People on the edge of your market who minimally use current offerings
   - Tier 2: People who consciously refuse the offering
   - Tier 3: People who have never considered the offering

2. **Draw the current Strategy Canvas.** X-axis: 8-15 competitive factors the industry competes on (price, quality, speed, features, brand, customization, support, compliance). Y-axis: offering level (low to high). Plot value curves for yourself and 2-3 competitors. If all curves look similar, you are in a red ocean.

3. **Explore the Six Paths Framework:**
   - Look across alternative industries (not just direct competitors)
   - Look across strategic groups within the industry
   - Look across the chain of buyers (user, purchaser, influencer)
   - Look across complementary products and services
   - Look across functional-emotional orientation
   - Look across time (anticipate trends)

4. **Apply the ERRC Grid (Eliminate-Reduce-Raise-Create):**
   - **Eliminate:** Which industry-standard factors should be removed entirely?
   - **Reduce:** Which factors should be reduced well below standard?
   - **Raise:** Which factors should be raised well above standard?
   - **Create:** Which factors has the industry never offered?

   **Critical rule:** Eliminate and Reduce must fund Raise and Create. If you only Raise and Create, you just increased your cost structure. Breaking the value-cost trade-off is the whole point.

5. **Draw the new Strategy Canvas.** A good blue ocean curve has three qualities: Focus (emphasis on few key factors), Divergence (clearly different from competitors), Compelling tagline (describable in one sentence).

6. **Validate with the Buyer Utility Map.** Six stages (purchase, delivery, use, supplements, maintenance, disposal) x six utility levers (productivity, simplicity, convenience, risk reduction, fun/image, environmental). Ensure your new offering removes adoption barriers.

7. **Set the strategic price using the price corridor of the mass.** The price must be low enough to attract noncustomers and high enough to deter imitators while maintaining margins (enabled by E/R savings).

8. **Test the business model.** Target cost minus strategic price = required margin. If the math doesn't work, redesign cost structure, not price.

### Good output vs bad output

**Bad:** "We should create uncontested market space by innovating and being different."

**Good (the [yellow tail] wine example):** "Eliminate: wine complexity and jargon, aging qualities, prestige advertising. Reduce: wine range (2 wines only: Chardonnay and Shiraz), vineyard prestige, wine critics' scores. Raise: retail store involvement, price just above budget ($6.99 vs. $4.99 budget, below $10+ premium). Create: easy drinking (sweet, fruity, approachable), easy selection (simplified label, reduced choice anxiety), fun identity (kangaroo logo, non-intimidating brand). Target noncustomers: beer and cocktail drinkers who found wine intimidating and hard to choose. E/R savings from eliminating oak aging, vineyard premiums, and prestige advertising funded mass retail distribution. Result: fastest-growing wine brand in US history within 2 years."

### Common mistakes

1. **Treating ERRC as a branding exercise.** Teams fill the grid with marketing language but don't change the operating model or cost structure. ERRC must translate to actual budget reallocation: dollars saved from E/R must fund R/C.

2. **Only Raising and Creating.** Adding features and quality without eliminating or reducing anything just increases cost. The discipline is in what you cut.

3. **Ignoring the price corridor.** Setting a premium price undermines the core logic -- blue oceans capture noncustomers through accessibility. Premium pricing = boutique offering in a red ocean.

4. **Skipping noncustomer analysis.** The entire framework hinges on why people currently don't buy from your industry. Surveying only existing customers produces red ocean improvements.

5. **Confusing differentiation with demand unlock.** Being different is not enough. The difference must unlock previously unserved demand at viable economics.

### When it breaks down

- **When there are no noncustomers.** In some industries, virtually everyone who could be a customer already is (utility electricity). No pool of nonconsumers to convert.
- **When the "blue ocean" has no fish.** No competition can mean no demand. Empty space may be empty for good reason.
- **Heavily regulated industries** where you cannot "eliminate" compliance or "reduce" safety features
- **B2B with complex buying processes.** The framework is strongest for consumer and simple B2B. Enterprise sales with 12-month procurement cycles and 8-person buying committees make noncustomer conversion much harder.
- **Survivorship bias.** The book's cases are retroactive analyses of successes. The framework is essentially unfalsifiable -- failed attempts "didn't really do it right."
- **Commodity markets** with very low room for meaningful value curve redesign

### Best combinations

- **Five Forces** -> **Blue Ocean**: Five Forces reveals structural profit destroyers; Blue Ocean's ERRC redesigns around them
- **Blue Ocean** (ERRC) -> **Value Chain**: ERRC defines the new offering; Value Chain redesigns the operating model to deliver it at the right cost
- **Jobs-to-Be-Done** -> **Blue Ocean**: JTBD identifies what noncustomers actually need; this directly feeds the Create/Raise factors
- **Blue Ocean** -> **Scenario Planning**: Stress-test whether the blue ocean move is robust across multiple futures
- **Ansoff** -> **Blue Ocean**: Ansoff identifies the quadrant; Blue Ocean defines how to compete differently within it

---

## Wardley Mapping

### When to use
When you need to make build-vs-buy decisions, understand which components of your value chain are commoditizing, or determine where to invest in differentiation vs. where to adopt off-the-shelf solutions. Particularly powerful for technology-driven businesses where component evolution creates strategic risk and opportunity.

### Step-by-step workflow

1. **Start with a specific user need.** Not "customers want good software" but "Enterprise security teams need to detect and respond to threats within 5 minutes." If you start from your tech stack instead of user needs, you'll produce an inventory, not a strategy map.

2. **Build the value chain top to bottom.** Working backward from user need, list every component required to deliver it. Components higher = more visible to the user; lower = less visible (infrastructure, dependencies).
   - Example: User Need -> Threat Detection Dashboard -> Alert Correlation Engine -> Log Collection -> Cloud Storage -> Compute -> Power/Cooling

3. **Draw dependency lines.** Connect components to show what depends on what. This reveals your actual value chain topology -- often surprising.

4. **Position each component on the evolution axis (left to right):**
   - **Genesis** (far left): Novel, poorly understood, one-of-a-kind. (New AI architecture)
   - **Custom-Built:** Better understood, built bespoke. (Proprietary fraud detection system)
   - **Product/Rental:** Standardized, multiple vendors. (CRM software, cloud databases)
   - **Commodity/Utility** (far right): Ubiquitous, interchangeable. (Electricity, AWS compute, email)

5. **Add movement arrows.** All components evolve left-to-right over time. Which are about to commoditize? Which are still Genesis?

6. **Identify strategic mismatches:**
   - Over-customizing commodity components (waste)
   - Underinvesting in differentiating Genesis/Custom components
   - Inertia: components that should have moved right but haven't (custom-building what you should rent)

7. **Decide strategic plays.** Build Genesis/Custom components that differentiate. Buy products for Product-stage components. Use commodity/utility for everything far-right.

8. **Iterate.** Expect 3-5 iterations before the map stabilizes. Share with team and challenge every placement.

### Good output vs bad output

**Bad:** A diagram with 5 boxes labeled "AI," "Cloud," "Data," "Platform," "Users" scattered across the canvas with no dependency lines, no evolution evidence. Conclusion: "We should invest in AI."

**Good:** "Enterprise document management map: User Need = 'Legal teams find relevant documents in <30 seconds during litigation.' Semantic Search Engine (Genesis -- competitive differentiator, 2 engineers). Document Classification (Custom-Built -- moving toward Product as vendors emerge; decision point: continue building or adopt vendor in 12 months?). OCR/Text Extraction (Product -- ABBYY, 3 alternatives, no differentiation). Cloud Storage (Commodity -- S3/GCS). Strategic insight: We are over-investing in Document Classification (3 engineers maintaining custom system) when 2 vendors (Kofax, Hyland) now offer equivalent capability at 30% of our cost. Redeploying those engineers to Semantic Search Engine would accelerate our competitive moat by 6 months. Risk: if we don't move Classification to vendor within 12 months, we'll maintain a commodity system at custom-build costs while competitors leapfrog us on search."

### Common mistakes

1. **Confusing evolution with maturity.** Evolution means a component transitions through distinct phases (Genesis -> Custom -> Product -> Commodity). Substituting "maturity" misses the phase-shift dynamics. Billions lost when companies treated cloud computing as merely a "mature" version of data centers.

2. **Starting from org charts or systems instead of user needs.** This produces a technology inventory, not a strategy map.

3. **Confusing visibility with importance.** Low-visibility infrastructure components can be strategically critical (e.g., a proprietary data pipeline buried deep in the stack).

4. **Ignoring evolution and treating every component as permanent differentiation.** Components evolve toward commodity. Your custom-built system will eventually be a product you can buy.

5. **Not using the map for decisions.** A beautiful map that doesn't drive build/buy/partner decisions, investment allocation, or organizational changes is an intellectual exercise.

### When it breaks down

- **When you can't identify the user.** In platforms serving multiple stakeholders with conflicting needs, which user need anchors the map? May need multiple maps.
- **When evolution stages are genuinely ambiguous.** Is blockchain Custom or Product? Depends on application. The map becomes a classification debate rather than insight tool.
- **Requires deep domain knowledge.** Unlike simpler frameworks, Wardley Mapping needs substantial industry and technology knowledge. Wrong knowledge = wrong map = bad strategy.
- **No standardized methodology.** Two experienced practitioners can produce different maps of the same landscape. Quality depends on mapper skill.
- **Scale complexity.** Large organizations with hundreds of components produce unwieldy maps. Need multiple maps at different resolutions.
- **Highly stable, low-complexity businesses** where the map adds little over simpler analysis

### Best combinations

- **Wardley Map** -> **VRIO**: Map identifies which Genesis/Custom components differentiate; VRIO tests whether they constitute sustainable advantages
- **Wardley Map** extends **Value Chain**: Wardley is essentially a value chain with an evolution dimension. It supersedes Porter's Value Chain for technology-driven businesses.
- **Wardley Map** -> **Five Forces** (on critical components): Map reveals where you compete; Five Forces assesses structural attractiveness of those arenas
- **Scenario Planning** -> **Wardley Map**: "Under Scenario A, does this component commoditize in 2 years instead of 5? What does that change for build vs. buy?"
- **Three Horizons** (concurrent): H1 = Product/Commodity components (defend, optimize). H2 = Custom components scaling toward Product. H3 = Genesis experiments.

---

## Scenario Planning

### When to use
When you face an irreversible, high-capital strategic decision under genuine uncertainty that forecasting cannot resolve. Not for routine planning. Best for 5-15 year questions: market entry, infrastructure investment, regulatory positioning, technology platform bets. The value is not in predicting the future but in stress-testing strategy against qualitatively different futures.

### Step-by-step workflow

1. **Define the focal question.** Specific, decision-oriented, time-bounded. Not "What will the future look like?" but "What should our investment strategy for Southeast Asian logistics be over the next 5 years?" The question determines scope and relevance.

2. **Identify 20-40 driving forces.** Use STEEP prompts:
   - **S**ocial: demographics, urbanization, consumer behavior
   - **T**echnological: AI, automation, energy tech, biotech
   - **E**conomic: growth rates, interest rates, trade policy, commodities
   - **E**nvironmental: climate, resource scarcity, regulation
   - **P**olitical: regulation, geopolitics, government stability

3. **Rank by impact and uncertainty.** Focus on forces that are both high-impact AND high-uncertainty. High-impact + low-uncertainty forces are "predetermined elements" -- include them in all scenarios but don't build scenarios around them.

4. **Select two critical uncertainties as axes (2x2 method).** The two most important and most independent. If axes are correlated (e.g., "economic growth" and "employment"), you get only 2 truly distinct scenarios instead of 4.

5. **Build scenario narratives (4 scenarios).** For each quadrant:
   - Memorable name ("Green Fortress," "National Champions," "Contested Drift")
   - 1-2 page narrative: what happened, why, consequences
   - Internally consistent -- events follow logically from axis assumptions
   - Include predetermined elements in all four
   - Make each plausible, not prediction or fantasy
   - Include signposts -- early indicators signaling this scenario is unfolding

6. **Test strategies against each scenario.** Score each candidate strategy across all four: Strong / Weak / Neutral. Create a strategy-scenario matrix.

7. **Identify robust strategies, contingent moves, and trigger points:**
   - **Robust:** Perform well across 3-4 scenarios. Prioritize these.
   - **Opportunistic:** Spectacular in one scenario, poor in others. Pursue only with clear triggers.
   - **Hedges:** Protect in worst-case scenarios.
   - **Signpost monitoring plan:** Which indicators to track, what adjustments to make.

8. **Embed in ongoing process.** Assign monitoring to specific people. Review signposts quarterly. Update scenarios every 1-2 years.

### Good output vs bad output

**Bad:** "Best case: economy grows, strategy succeeds. Base case: moderate growth, strategy mostly works. Worst case: recession, strategy underperforms. Recommendation: plan for base case."

This is forecasting with a low/medium/high wrapper, not scenario planning. One future at different volume levels. "Tyranny of the mid-case" -- gravitating to the comfortable middle.

**Good:** "Focal question: How should we position our European energy company over the next decade?

Axis 1: Speed of energy transition (Gradual <-> Accelerated mandate)
Axis 2: European geopolitical posture (Fragmented/national <-> Integrated/unified)

Scenario A -- 'Green Fortress' (Accelerated + Integrated): EU mandates net-zero by 2035, coordinated industrial policy, carbon border tax >$100/ton isolates EU market. Implication: massive renewables investment, only pan-European scale companies survive. Signpost: carbon border tax >$100/ton by 2028.

Scenario B -- 'National Champions' (Accelerated + Fragmented): Transition accelerates but each country goes alone. Germany bets hydrogen, France nuclear, Spain solar. 27 micro-markets. Implication: country-by-country strategy, flexible asset mix, avoid pan-European infrastructure bets. Signpost: failure of 2+ major EU energy coordination initiatives by 2028.

Scenario C -- 'Slow Burn United' (Gradual + Integrated): Fossil gas remains bridge fuel through 2040. Implication: gas assets retain value, renewables build gradually. Signpost: EU extends gas taxonomy past 2030.

Scenario D -- 'Contested Drift' (Gradual + Fragmented): Political stalemate, aging infrastructure, import dependence. Implication: defensive posture, minimize capital commitments. Signpost: EU energy policy gridlock for 3+ consecutive summits.

Robust strategies (3-4 scenarios): Invest in modular, scalable renewables (good in A, B, C); build regulatory affairs in 5 largest markets (all 4); maintain gas optionality (C, D, partial B). Hedge: do NOT commit to pan-European mega-projects until Scenario A signposts confirm."

### Common mistakes

1. **Building scenarios around your preferred future.** If all scenarios conveniently support the strategy leadership already wants, you have confirmation bias, not planning. Test: at least one scenario should make leadership genuinely uncomfortable.

2. **The tyranny of the mid-case.** Low/medium/high scenarios that gravitate to the middle. Good scenario planning uses qualitatively different futures, not quantitatively different projections.

3. **Not translating scenarios into action.** The number one complaint: "We did a great scenario exercise and nothing changed." Without testing actual strategy against each scenario and developing contingency plans, the exercise is purely intellectual.

4. **Correlated axes.** If your two axes are not independent, opposite quadrants become implausible and you have only 2 distinct scenarios instead of 4.

5. **Leadership disengagement.** If senior leaders are not involved in building scenarios, they will not internalize or use them. It's as much a leadership alignment tool as an analytical one.

6. **One-and-done exercise.** Scenarios go stale. Build a signpost monitoring process and update annually.

7. **Building on predetermined elements.** Using certain trends (aging population) as axes produces scenarios where axes aren't truly uncertain. Reserve axes for genuine uncertainties.

### When it breaks down

- **Short time horizons.** For 6-12 month decisions, traditional forecasting and sensitivity analysis are more efficient.
- **When critical uncertainties exceed 2.** The 2x2 forces two axes. With 4-5 genuinely critical uncertainties, alternatives needed: morphological analysis, Monte Carlo, or multiple 2x2s.
- **When the audience wants predictions.** Scenario planning deliberately refuses to assign probabilities. If leadership demands a single forecast, it will frustrate them.
- **When decisions are reversible.** If you can change course cheaply and quickly, the apparatus is overkill. Most valuable for irreversible, high-capital decisions.
- **Cognitive overload.** Maintaining 4 distinct mental models is hard. Many organizations collapse to "Plan A and contingencies."
- **Evidence on effectiveness is limited.** Academic reviews note "conceptual confusion, methodological chaos, and scarcity of evidence on effectiveness." Shell's success may be an N=1 case with survivorship bias.

### Best combinations

- **Scenario Planning** -> **Five Forces** (per scenario): Industry structure changes under different futures. Stress-tests competitive positioning.
- **Scenario Planning** -> **Wardley Map**: "Under Scenario B, does this component commoditize in 2 years instead of 5?"
- **Scenario Planning** -> **Three Horizons**: Reveals whether horizon allocation is resilient or fragile under different futures
- **Scenario Planning** -> **GE Nine-Box**: Attractiveness and strength scores may shift dramatically. Green zone under one future = Red zone under another.
- **Blue Ocean** -> **Scenario Planning**: Test whether the blue ocean move is robust across multiple states of the world

---

## Cross-Framework Integration Patterns

### By problem type

**Market attractiveness:**
Five Forces -> Value Chain -> VRIO. Test whether the market is structurally attractive, identify where value is created, then test whether you have a defendable advantage in critical activities.

**Growth strategy:**
Ansoff -> Three Horizons -> BCG. Ansoff defines growth type, Horizons stages investment over time, BCG funds the portfolio rationally.

**Organizational execution:**
Value Chain -> 7S -> Nine-Box. Value Chain clarifies the work, 7S aligns the organization, Nine-Box tests whether the leadership bench can execute.

**Strategic uncertainty:**
Scenario Planning -> Three Horizons -> Wardley Mapping. Scenarios explore external uncertainty, Horizons manages investment timing, Wardley shows which capabilities will commoditize or become strategic.

**Market creation or repositioning:**
Five Forces -> Blue Ocean -> Value Chain. Five Forces identifies where the market punishes profitability, Blue Ocean redesigns the value curve, Value Chain ensures the redesign is operationally viable.

### The master sequence for comprehensive analysis

```
1. PESTEL + Scenario Planning  -->  Macro environment + alternative futures
       |
2. Five Forces (per scenario)  -->  Industry structure and profit pools
       |
3. Value Chain / Wardley Map   -->  How value is created and delivered
       |
4. VRIO                        -->  Which resources are sustainable advantages
       |
5. BCG / GE Nine-Box           -->  Portfolio assessment and allocation
       |
6. Ansoff / Blue Ocean         -->  Growth direction and competitive approach
       |
7. Three Horizons              -->  Allocation across time horizons
       |
8. 7S                          -->  Organizational readiness to execute
```

### Quick reference: which framework for which question

| Question | Primary | Support with |
|----------|---------|-------------|
| Is this industry worth being in? | Five Forces | PESTEL, Scenario Planning |
| What are our real advantages? | VRIO | Value Chain, Wardley Map |
| Where should we invest across the portfolio? | GE Nine-Box or BCG | Five Forces, VRIO |
| How should we grow? | Ansoff | VRIO, Five Forces |
| How can we escape competition? | Blue Ocean | Five Forces, Value Chain, JTBD |
| How should we balance today vs. tomorrow? | Three Horizons | BCG, Scenario Planning |
| Can our organization execute this? | 7S | Value Chain, VRIO |
| What are the build vs. buy decisions? | Wardley Map | VRIO, Five Forces |
| What if the world changes? | Scenario Planning | Five Forces, Nine-Box, Wardley |
| Where do we create and deliver value? | Value Chain (traditional) / Wardley (tech) | VRIO, Five Forces |

### Practitioner notes

- These frameworks are lenses, not answers. Output should always end in choices, tradeoffs, and actions.
- The most common failure mode across all of them: false precision built on weak market definitions and poor evidence.
- The highest-quality strategy work combines one external lens, one internal capability lens, and one execution lens.
- A completed framework without specific strategic implications is a wasted exercise. If the output could apply to any company in any industry, it is not yet useful.
