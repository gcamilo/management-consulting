# Operations & Change Management Frameworks

Practitioner reference. Each framework: when to use, step-by-step workflow, good vs bad output, common mistakes, breakdown conditions, best combinations.

---

## 1. ADKAR (Prosci)

Individual-level change adoption diagnostic. Five sequential outcomes a person must achieve: **Awareness, Desire, Knowledge, Ability, Reinforcement**. Not an organizational transformation model -- it diagnoses and fixes the *people side* of specific changes.

### When to Use

- Technology rollouts where frontline adoption determines ROI (ERP, CRM, new tools)
- Process changes requiring new daily behaviors from specific employee groups
- Any change where you need to pinpoint *why* adoption is stalling and *where* to intervene
- NOT for culture transformations, political reorganizations, or questioning whether the change itself is correct

### Step-by-Step Workflow

**1. Define the change in behavioral terms.**
Write one sentence: what changes, for whom, by when. Convert vague transformation language into observable behaviors. Identify all impacted groups -- including downstream teams, customers, vendors.

**2. Segment impacted populations.**
Group by role, geography, function, manager chain, and level of disruption. Never treat all employees as one audience. Example: 200 sales reps, 50 managers, 10 IT support staff each face different changes.

**3. Assess current ADKAR state per segment.**
Score each element 1-5. Identify the **barrier point**: the first element scoring 3 or below. The barrier point is the *only* thing you address -- do not skip ahead.

**4. Intervene at the barrier.**
- **Awareness barrier**: Executive communications, competitive benchmarks, customer complaint data. Test: can employees articulate *why* in their own words?
- **Desire barrier**: Manager 1:1 conversations (not mass emails), peer advocates, personal impact statements addressing WIIFM. Test: are people volunteering for pilots or passively resisting?
- **Knowledge barrier**: Role-based training, simulations, job aids. Must be sequenced *after* Awareness and Desire -- training without buy-in is wasted budget.
- **Ability barrier**: Coaching, practice time, sandbox environments, reduced workload during transition. The gap between Knowledge and Ability is where most implementations fail silently.
- **Reinforcement barrier**: Recognition, metrics dashboards, incentive realignment, removal of old-system access. Without this, people revert within 60-90 days.

**5. Reassess at 30/60/90 days.** New barriers emerge as the change matures. Feed insights back to the organizational change plan.

### Good vs Bad Output

**Good:**
```
Group: Field Sales Team (42 people)
Change: Migration from Salesforce Classic to Lightning
Assessment Date: 2026-02-15

  Awareness:  4.2  -- Strong. Town halls + manager cascade worked.
  Desire:     2.8  -- BARRIER POINT. Reps fear quota impact during learning curve.
  Knowledge:  N/A  -- Cannot assess until Desire resolved.
  Ability:    N/A
  Reinforcement: N/A

Barrier Diagnosis: Reps understand WHY but don't want the productivity hit.
Intervention: Manager 1:1s this week with quota adjustment memo. Pilot group
testimonials from Denver office. Reassess Desire in 2 weeks.
```

**Bad:**
```
ADKAR Assessment: Company-Wide
All scores: 3.5 average
Action: Continue communications and training.
```
Averaged scores hide variance. No barrier identified. No specific intervention. ADKAR's value is specificity -- averaging destroys that.

### Common Mistakes

1. **Jumping to training before Awareness and Desire are achieved.** The #1 ADKAR failure. Prosci data: 39% of employees say lack of awareness drives resistance. Training without buy-in doesn't stick.
2. **Treating ADKAR as a one-time checklist.** It is a diagnostic loop. People who had Desire at launch lose it when difficulties mount. Practitioners who "complete" ADKAR at go-live are misusing the model.
3. **Assessing groups instead of individuals.** Averaging a department masks the 20% stuck at Awareness and the 15% stuck at Ability. Those require completely different interventions.
4. **Confusing Knowledge with Ability.** A surgeon can *know* a procedure but not *perform* it. Most orgs declare success when training completes (Knowledge), then are shocked when adoption stalls (Ability gap).
5. **Neglecting Reinforcement.** Most change plans end at go-live. Without ongoing metrics, recognition, and removal of old workarounds, drift begins within 60 days.

### When It Breaks Down

- **Structural or political changes** (mergers, layoffs, mandates). ADKAR focuses on individual Desire -- irrelevant when people have no opt-out.
- **Culture-level transformations.** No mechanism for systemic cultural patterns or power dynamics.
- **Continuous/agile change environments.** The sequential model becomes unwieldy with overlapping changes and pervasive change fatigue.
- **When the change itself is wrong.** ADKAR assumes the change is correct. It can become a tool for pushing through bad decisions by labeling legitimate resistance as a "Desire barrier."

### Best Combinations

- **ADKAR + Kotter**: Kotter structures the organizational program; ADKAR diagnoses where individuals are stuck within each step. Kotter says "create urgency" -- ADKAR measures whether Awareness actually landed.
- **ADKAR + Lewin**: Unfreeze = Awareness + Desire. Change = Knowledge + Ability. Refreeze = Reinforcement. Adds tactical depth to Lewin's simplicity.
- **ADKAR + Influence Model**: Use the four levers as the intervention toolkit for barrier points. Desire barrier? Deploy compelling story + role modeling. Ability barrier? Deploy skill-building + formal mechanisms.

---

## 2. Kotter 8-Step Change Model

Organizational-level framework for leading large-scale transformation. A *leadership* model: it tells leaders what to orchestrate, not individuals what to feel.

### When to Use

- Large transformations requiring broad organizational momentum (ERP, merger integration, operating model redesign)
- When the problem is mobilizing leadership commitment and cross-functional alignment
- NOT for bounded process improvements, agile/continuous change, or founder-led orgs where coalition logic is weak

### Step-by-Step Workflow

**1. Create urgency.** Quantify the cost of inaction: revenue at risk, competitive position lost, regulatory deadline. Communicate to 75%+ of management. Deliverable: one-page burning platform with data, not opinions. Test: if people nod but don't change their calendars, urgency is performative.

**2. Build a guiding coalition.** 3-8 people with positional power, expertise, credibility, and leadership ability spanning levels and functions. Include at least one respected skeptic. Must operate as a *team* with weekly working sessions and decision authority -- not a monthly review committee.

**3. Form strategic vision and initiatives.** Vision must be communicable in under 5 minutes. Translate into 3-5 initiatives with owners and timelines. Test: ask 10 random employees to describe the vision.

**4. Enlist a volunteer army.** Multiply planned communication by 10x. Use stories, not decks. Recruit change champions at every level who amplify and translate the vision locally.

**5. Remove barriers.** Identify structural obstacles: misaligned incentives, blocking managers, legacy systems, outdated processes. Confront managers who undermine the change (the hardest step for most orgs).

**6. Generate short-term wins.** Plan visible, unambiguous wins within 6-18 months that relate to the change effort. Recognize people publicly. Wins must be credible to skeptics, not vanity metrics.

**7. Sustain acceleration.** Use win credibility to tackle bigger changes. Hire and promote people who embody the change. Do NOT declare victory too early.

**8. Institute change.** Embed in onboarding, performance reviews, promotions, governance, and leadership succession.

### Good vs Bad Output

**Good guiding coalition:**
```
Coalition for ERP Transformation:
- CFO (budget authority)
- VP Operations (process owner)
- Regional Sales Director - Southwest (field credibility, known skeptic)
- IT Architecture Lead (technical expertise)
- Plant Manager - Ohio (frontline credibility, respected by unionized workforce)

Operating model: Weekly 90-min working sessions. Decision authority on
scope changes up to $500K. Coalition owns the initiative.
```

**Bad guiding coalition:**
```
Change Steering Committee: All 12 VPs. Meets monthly for 1 hour.
Reviews status updates from PMO. No decision authority.
```
Too many people, too infrequent, passive reviewers, no real authority. A committee, not a coalition.

**Good quick win:**
```
Win: First automated PO processed end-to-end in new ERP.
Timeline: 8 weeks post-launch.
Metric: Order-to-payment cycle from 14 days to 3 days.
Visibility: Announced at all-hands with the AP clerk who processed it.
```

**Bad quick win:** "ERP training completed for 85% of users." Training completion is an input metric. It proves nothing about whether the change is working.

### Common Mistakes

1. **Performing the steps rather than genuinely executing them.** Town halls are staged, coalitions have no authority, visions are written by consultants. Kotter's steps become theatrical compliance.
2. **Skipping urgency.** Leaders assume the case for change is obvious. It is not. Kotter says this is the #1 error.
3. **Declaring victory after quick wins.** The change is not yet embedded in culture. Within 12-18 months the organization reverts, especially when the executive sponsor moves on.
4. **Under-communicating the vision by 10-100x.** A single all-hands is roughly 0.01% of the communication needed.
5. **Building a committee instead of a coalition.** A committee reviews. A coalition leads. If it doesn't meet weekly with decision authority, it's a committee wearing a coalition's name.

### When It Breaks Down

- **Agile/continuous-change environments.** The model assumes a bounded change initiative.
- **When the problem is structural, not motivational.** No amount of urgency fixes a bad architecture or broken supply chain.
- **Entrenched middle management.** The model underestimates institutional inertia rooted in politics, not psychology.
- **Lacks empirical validation.** Wide adoption but no controlled studies proving the 8 steps produce better outcomes.

### Best Combinations

- **Kotter + ADKAR**: The gold standard. Kotter structures the program; ADKAR diagnoses individual adoption within each step.
- **Kotter + Influence Model**: Use Kotter for sequencing, McKinsey's four levers for execution. Step 4 maps to Understanding & Conviction + Role Modeling. Step 5 maps to Formal Mechanisms.
- **Kotter + Customer Journey Map**: For customer-facing transformations, map the journey first, then use Kotter to drive internal change.

---

## 3. Lewin Change Model (Unfreeze-Change-Refreeze)

The simplest change model. Three phases with an embedded diagnostic (Force Field Analysis). Best as a framing model for transition design and stakeholder communication.

### When to Use

- Bounded, single-stream changes where a clean narrative is needed
- When you need to diagnose driving and restraining forces before launching
- As a framing layer paired with more detailed models (ADKAR, Kotter)
- NOT for multi-stream transformations, agile environments, or complex political contexts

### Step-by-Step Workflow

**Phase 1: Unfreeze**

1a. **Conduct Force Field Analysis.** T-chart: Driving Forces (left, scored 1-10) vs Restraining Forces (right, scored 1-10). Prioritize: weakening restraining forces is cheaper than strengthening drivers.

1b. **Build the case for change.** Use data: financial gaps, customer complaints, competitive benchmarks, regulatory deadlines. Make the status quo feel uncomfortable.

1c. **Create psychological safety.** Acknowledge disruption. Clarify what will and won't change. Leadership must model openness.

1d. **Test readiness.** Are people asking questions (engaged) or silent (withdrawn)? Visible resistance is healthier than silent compliance.

**Phase 2: Change**

2a. Define target state in measurable terms. 2b. Pilot before full rollout. 2c. Manage the "valley of despair" -- performance dips during transition. Set expectations and increase support. 2d. Monitor and adjust iteratively.

**Phase 3: Refreeze**

3a. Embed in SOPs, job descriptions, KPIs, governance, onboarding. 3b. **Remove old-state artifacts** -- decommission old systems, templates, workarounds. Leaving the old system available guarantees reversion. 3c. Celebrate and reinforce. 3d. Audit stability at 90 and 180 days.

### Good vs Bad Output

**Good Force Field Analysis:**
```
CHANGE: Migrate manufacturing QC from paper to digital tablets

DRIVING FORCES                     | Score | RESTRAINING FORCES                 | Score
FDA audit findings (3 observations)| 9     | 15-year veterans comfortable w/paper| 7
Lost 2 contracts to digital rival  | 8     | Unreliable WiFi on plant floor      | 8
CEO mandate + budget approved      | 7     | Union concern about surveillance    | 6
Younger workers prefer digital     | 5     | Tablet durability in wet/cold env   | 4
                                   |       | Training = production downtime      | 5

TOTAL DRIVING: 29                  |       | TOTAL RESTRAINING: 30

Priority: Weaken restraints before launch
1. Fix WiFi infrastructure (8 -> 0)
2. Union briefing: tablets track QC, not people. Written commitment. (6 -> 3)
3. Industrial-grade tablets, not consumer iPads (4 -> 1)
Net after: Driving 29 vs. Restraining 16 --> proceed
```

**Bad:** "Driving: Management wants it. Restraining: People resist change. Score: 5 vs 5. Need more communication." Abstract forces, meaningless scores, generic intervention.

### Common Mistakes

1. **Rushing Unfreeze.** One town hall and a memo is not Unfreezing. Takes 2-4x longer than leaders expect.
2. **Skipping Refreeze entirely.** The Change phase is exciting; Refreeze is boring admin (updating SOPs, changing incentives, decommissioning old systems). Without it, the change erodes over 3-12 months.
3. **Treating phases as linear when reality is iterative.** You may need to re-Unfreeze midway through Change when new resistance emerges.
4. **Interpreting Refreeze as permanent rigidity.** Lewin's intent was stabilization, not ossification. "The new way is now the default" -- not "we never change again."

### When It Breaks Down

- **Complex, multi-stream transformations.** What is "frozen" for one initiative is being "unfrozen" for another.
- **Continuous change environments.** Refreeze is a fiction if the org never reaches stability.
- **No individual-level guidance.** Describes organizational phases but provides no tools for individual transitions.
- **Oversimplifies politics and power.** Assumes rational actors responding to rational arguments.
- **Force Field scores create false precision.** Scoring 1-10 feels rigorous but is entirely subjective.

### Best Combinations

- **Lewin + ADKAR**: Lewin provides macro phases; ADKAR provides individual diagnostics. The combination adds tactical depth.
- **Lewin + Kotter**: Kotter's 8 steps map onto Lewin's phases (Steps 1-4 = Unfreeze, 5-7 = Change, 8 = Refreeze).
- **Lewin + Force Field Analysis**: Built-in pairing. Always use FFA during Unfreeze.

---

## 4. McKinsey Influence Model

Behavioral change framework. Four levers must work *simultaneously*: (1) Understanding & Conviction, (2) Role Modeling, (3) Talent & Skills, (4) Formal Mechanisms. Core insight: most programs over-invest in one lever (usually communication) and neglect the other three.

### When to Use

- Culture shifts and behavior change at scale
- When multiple previous change efforts have failed despite good communications
- When the problem is clearly behavioral (not structural, technological, or strategic)
- NOT for structural problems (org design, technology migration) or when top leaders refuse to model the change

### Step-by-Step Workflow

**1. Define critical behaviors.** Specify the few behaviors that must change to move business outcomes. Avoid broad statements ("be more collaborative"). Good: "Product, regulatory, and operations leads resolve launch risks in weekly issue meetings with explicit decision ownership instead of email escalation loops."

**2. Diagnose the four levers per population segment.** Score each 1-10.

**3. Build Understanding & Conviction.** Craft a change story: Where are we? Where are we going? Why is this better *for you*? Test: run it past frontline employees. If they roll their eyes, rewrite it. Anti-pattern: 40-slide PowerPoint sent by email.

**4. Activate Role Modeling.** Identify the most influential people at every level -- not just executives. They must *visibly* demonstrate new behaviors before asking others to follow. Anti-pattern: CEO announces "we are data-driven" then makes the next three decisions by gut feel.

**5. Develop Talent & Skills.** Experiential learning: simulations, on-the-job practice, peer coaching. Build psychological safety for skill-building. Anti-pattern: one-day classroom training followed by "now go do it."

**6. Align Formal Mechanisms.** Audit everything: incentives, performance reviews, reporting structures, approval processes, meeting cadences. Every mechanism must support the new behavior or be neutral. Any mechanism rewarding old behavior will win. Anti-pattern: telling people to "collaborate more" while maintaining individual sales commissions and stack-ranked reviews.

**7. Activate all four simultaneously.** Sequencing (story first, then skills, then mechanisms) is less effective than parallel activation. Each lever reinforces the others.

### Good vs Bad Output

**Good diagnostic:**
```
Population: Regional Store Managers (200 people)
Change: Transaction-focused to relationship-focused selling

Understanding & Conviction: WEAK (3/10)
  Managers see it as "corporate flavor of the month"
  Intervention: Regional VP store visits with customer lifetime value data

Role Modeling: MODERATE (5/10)
  District managers talk about it but still reward daily transaction counts
  Intervention: Film 3 top-performing stores already doing it. DMs demo one
  relationship conversation per store visit.

Talent & Skills: WEAK (2/10)
  Managers know transactions. They don't know customer profiling or pipeline mgmt.
  Intervention: 3-day experiential workshop + 8 weeks of coaching calls

Formal Mechanisms: CRITICAL GAP (1/10)
  Commission: 100% transaction count. No CRM. No relationship metrics in reviews.
  Intervention: Redesign commission 60/40 transaction/relationship. Deploy CRM.
```

**Bad:** "We need better communication, more training, and leadership commitment." Names three levers generically, no diagnosis, no specific interventions. Indistinguishable from any change management platitude.

### Common Mistakes

1. **Over-investing in the story, under-investing in formal mechanisms.** McKinsey's own research shows this is the most common imbalance. A bank rolled out customer scripts and profiling questions but left the old commission structure intact -- sales didn't budge.
2. **Treating role modeling as communication.** "The CEO sent a video" is not role modeling. Leaders must *do* the new behavior visibly and consistently.
3. **Running levers sequentially instead of in parallel.** The model explicitly requires simultaneous activation. Sequential execution means early levers lose momentum.
4. **Ignoring feedback loops.** If skills training isn't landing, the intervention needs to change -- not just more of the same training.

### When It Breaks Down

- **When the change is fundamentally structural.** The four levers target behavior, not org charts or technology.
- **Top-down bias.** Limited space for bottom-up initiative or emergent change.
- **Difficulty measuring lever strength.** No standardized diagnostic. Two teams can assess the same situation differently.
- **The "70% fail" trap.** McKinsey cites this alongside the model, but no controlled evidence proves the model improves success rates.

### Best Combinations

- **Influence Model + ADKAR**: ADKAR diagnoses *where individuals are stuck*; Influence Model determines *which lever to pull*.
- **Influence Model + Kotter**: Kotter provides sequence; Influence Model provides execution toolkit. Step 1 = Understanding & Conviction. Step 2 = Role Modeling. Step 5 = Formal Mechanisms.
- **Influence Model + Customer Journey Map**: For CX transformations, map the journey first, then use the model to drive behavior changes at critical touchpoints.

---

## 5. Customer Journey Map

Visual representation of the customer's end-to-end experience. Outside-in: captures what the customer does, thinks, and feels -- NOT an internal process map. Originated in service design; now used in CX, marketing, product, and operations.

### When to Use

- Diagnosing why customers churn, stall, or complain at specific points
- Redesigning customer experience across channels and handoffs
- Building cross-functional empathy -- the workshop is as valuable as the map
- NOT for pre-launch products with no customers, commoditized journeys, or purely internal efficiency problems

### Step-by-Step Workflow

**1. Define scope.** State the question: "Why do 40% of trial users not convert?" Select ONE persona. Define journey boundaries (start and end events). Never mix personas in one map.

**2. Gather customer research.** Primary: 8-12 customer interviews (qualitative saturation), contextual observation, diary studies, support ticket analysis. Secondary: web/app analytics, NPS data, CRM funnels. Rule: qualitative reveals *why*, analytics reveals *how many*. Start with qualitative.

**3. Identify stages from the customer's perspective.** Not your org chart. B2C typical: Awareness -> Consideration -> Purchase -> Onboarding -> Usage -> Renewal. Validate stage names with customer language from interviews.

**4. Map the layers per stage.** Customer goals, actions, touchpoints, thoughts, emotions (as a curve from high to low), pain points, and opportunities.

**5. Run a cross-functional workshop (half-day).** 5-8 participants from product, marketing, sales, support, operations. Hour 1: present research. Hour 2: map stages and actions. Hour 3: add emotions and pain points. Hour 4: identify top 3-5 opportunities and assign owners.

**6. Prioritize and act.** Score opportunities on Impact x Feasibility. Select 3-5 for immediate action with owners, timelines, and metrics. The map without an action plan is decorative.

**7. Iterate.** Revisit every 6-12 months. Layer in quantitative data over time.

### Good vs Bad Output

**Good (Onboarding stage):**
```
STAGE: Onboarding (Day 1-14)
Customer Goal: Get tool working with real data, see first value

Actions: Creates account, uploads CSV (Day 1) -> Watches tutorial (Day 1-2) ->
  Attempts first email campaign (Day 3-5) -> Contacts support re merge tags
  (Day 4) -> Considers abandoning (Day 7-10) -> Receives CS check-in (Day 8)
  -> Completes first successful campaign (Day 12)

Emotions: Excited (Day 1) -> Confused (Day 3) -> Frustrated (Day 4-7) ->
  Relieved (Day 8) -> Satisfied (Day 12)

Pain Points:
- CSV import silently drops rows with formatting errors (no feedback)
- Tutorial assumes Mailchimp experience; doesn't explain merge tags
- Support chat wait: 45 min average

Moment of Truth: Day 4-7 is the danger zone. 62% of churned users last
opened the app on Day 5-7.

Opportunities:
1. CSV validation with error messages before import (HIGH impact, LOW effort)
2. "Absolute beginner" tutorial path (HIGH impact, MEDIUM effort)
3. In-app nudge on Day 3 if no campaign created (HIGH impact, LOW effort)
```

**Bad:** "Stage: Onboarding. Touchpoints: Website, Email, App. Emotion: Neutral to Positive." No research, no specific actions, emotions are guesses, no quantitative backing, no opportunities.

### Common Mistakes

1. **Building from internal assumptions, not customer research.** The #1 failure. Even 5 interviews will radically change the map.
2. **Mapping touchpoints only.** Touchpoints are the *where*. A good map captures the full experience: actions, thoughts, emotions, pain points.
3. **Mixing personas.** First-time buyer and power user have fundamentally different journeys.
4. **Creating a beautiful map nobody acts on.** 70% of organizations fail to define clear objectives for their maps. The deliverable is the prioritized action plan.
5. **Making it a one-time exercise.** A 2024 map is likely inaccurate by 2026.

### When It Breaks Down

- **When the org can't act on findings.** Creates frustration and cynicism without executive sponsorship and budget.
- **Complexity explosion with multiple segments.** 8 personas x 6 stages x 12 touchpoints = hundreds of cells. Prioritize the 2-3 journeys representing 80% of revenue or churn risk.
- **Can identify problems but can't solve them.** "Customer waits 45 minutes on hold" doesn't fix the staffing model. Must be paired with operational improvement methods.

### Best Combinations

- **Journey Map + NPS**: Overlay NPS at each stage to quantify where satisfaction drops.
- **Journey Map + Kotter/ADKAR**: When the map reveals needed internal changes, use change frameworks to drive them.
- **Journey Map + Service Blueprint**: Journey maps = customer view. Blueprints = operational view. Together, they connect customer pain to operational root cause.

---

## 6. NPS / Loyalty Measurement

Net Promoter Score. Single question: "How likely are you to recommend [X]?" Promoters (9-10) minus Detractors (0-6). Range: -100 to +100. Best used as a directional signal and closed-loop feedback system, not as a standalone strategy.

### When to Use

- Benchmarking customer loyalty trends over time
- Identifying where experience breaks via transactional NPS at journey touchpoints
- Driving a closed-loop improvement system (inner loop = individual follow-up, outer loop = structural fixes)
- NOT as the sole customer metric, for cross-cultural comparison, or as a reliable growth predictor

### Step-by-Step Workflow

**1. Design survey.** Core question + mandatory open-ended follow-up ("What is the primary reason for your score?"). Max 5 questions total. Decide: relationship NPS (quarterly brand health) vs transactional NPS (after specific interactions).

**2. Determine sampling.** Minimum ~250 responses for segment-level significance. Cadence: relationship quarterly, transactional triggered by events. Never survey the same customer more than once per quarter.

**3. Calculate and segment.** NPS = % Promoters - % Detractors. Segment by cohort, product, geography, channel, revenue tier. Segmented scores are far more actionable than aggregate.

**4. Analyze verbatims.** Code responses into themes. Separate Promoter drivers from Detractor drivers. Identify top 3-5 drivers of each. This qualitative analysis is where the actionable insights live.

**5. Close the loop (Inner Loop).** Contact Detractors within 24-48 hours. Understand the issue, resolve if possible. Log outcomes.

**6. Drive structural change (Outer Loop).** Aggregate findings monthly. Identify systemic issues appearing across multiple customers. Route to appropriate teams with data. Track whether fixes move subsequent NPS.

### Good vs Bad Output

**Good:**
```
Q1 2026 NPS: +38 (up from +32 Q4 2025). n=1,247, CI +/- 2.8 pts

Segments: Enterprise +52 | Mid-Market +41 | SMB +18 <-- gap

Top Detractor drivers:
  "Reporting is limited, need custom dashboards" (47% of Detractor verbatims)
  "Price increased but no new features" (29%)
  "Mobile app crashes" (24%)

Inner Loop: 89% of Detractors contacted within 48h. 23% converted to Passive.
Outer Loop: Custom reporting in dev (Q2). Mobile stability sprint done (crashes -60%).
```

**Bad:** "NPS: +38. Good score! Above industry average. Keep up the great work!" No segmentation, no drivers, no loop metrics, no actions. The number alone tells you nothing.

### Common Mistakes

1. **Not asking the follow-up "why" question.** The score alone is a dashboard number. The reason behind it is where every actionable insight lives.
2. **No closed-loop system.** NPS without Inner Loop (individual follow-up) and Outer Loop (structural fixes) is expensive surveying.
3. **Insufficient sample sizes.** Reporting segment-level NPS with 30 responses and treating 5-point movements as meaningful. Margin of error can be +/- 15 points.
4. **Gaming and score inflation.** The moment NPS is tied to individual compensation, the incentive to game overwhelms the incentive to improve. Car dealerships are notorious for coaching customers to give 9s.
5. **Ignoring Passives.** NPS excludes Passives (7-8) from the calculation, but they are the largest moveable group -- satisfied enough not to complain, not loyal enough to recommend.

### When It Breaks Down

- **Not a reliable growth predictor.** Despite Reichheld's original claim, subsequent research has not validated that NPS consistently predicts revenue growth better than other satisfaction measures.
- **Binning destroys information.** A customer scoring 6 is grouped with one scoring 0. A simple average of 0-10 scores is often more informative.
- **Cultural bias.** In Japan and Northern Europe, respondents rarely give 9-10 regardless of satisfaction. Cross-country comparisons are misleading.
- **"Likelihood to recommend" is not loyalty.** People may love enterprise middleware but never discuss it socially. NPS conflates satisfaction with referral behavior.
- **Easily gamed.** Any metric tied to compensation gets optimized for the metric, not the underlying experience.

### Best Combinations

- **NPS + Customer Journey Map**: The most natural pairing. Transactional NPS at touchpoints quantifies where the experience breaks. Journey map provides context; NPS provides signal.
- **NPS + CSAT + CES**: NPS = loyalty, CSAT = satisfaction, CES = friction. Multi-dimensional view.
- **NPS + Influence Model**: When NPS reveals employee behavior driving detraction, use the four levers to shift behaviors at the touchpoints that matter.

---

## Cross-Framework Selection Guide

| Situation | Lead Framework | Support With |
|-----------|---------------|-------------|
| Large transformation (ERP, merger) | Kotter | ADKAR + Influence Model |
| Customer experience overhaul | Journey Map | NPS + Influence Model + Kotter |
| Bounded process/technology change | Lewin | ADKAR + Force Field Analysis |
| Culture change initiative | Influence Model | Kotter Steps 1-3 + ADKAR |
| Ongoing CX management | NPS system | Journey Map + Service Recovery |
| Frontline adoption stalling | ADKAR | Influence Model for intervention design |

**The practical test for any framework application:** Can an operator read the output and know what to do differently next week? If not, the framework has been used as presentation language, not execution design.
