# management-consulting — Strategy Skill for AI Coding Agents

Turn your AI agent into a structured thinking partner for strategy, decisions, and analysis. 42 frameworks with practitioner-grade depth — not textbook theory, but step-by-step workflows, real examples, common mistakes, and when each framework breaks down.

Built for Claude Code. Compatible with Codex, Gemini CLI, Cursor, and any agent that reads SKILL.md files.

## Why this exists

Asking an LLM to "act like a consultant" produces generic framework-salad. This skill fixes that by providing:

- **Process discipline** — clarify the decision before analyzing. Structure before hypothesizing. Evidence-label every claim.
- **Framework depth** — 4,100+ lines of practitioner workflows across 42 frameworks. Each has step-by-step application, good/bad output examples, common mistakes, and failure conditions.
- **Three modes** — Quick Structure (exploratory), Full Case (analytical), Client Deliverable (polished). Matches response depth to your actual need.
- **Quality gates** — output contract, devil's advocate step, 9-point checklist. Prevents shallow answers.
- **Anti-selection rules** — tells the agent when NOT to use a framework. Stops Five Forces on every strategy question.

## Install

```bash
# Claude Code
cp -r management-consulting/ ~/.claude/skills/management-consulting/

# Or use npx
npx skills add gcamilo/management-consulting
```

## Usage

Just ask naturally. The skill activates on strategy questions, decisions, market analysis, due diligence, or structured recommendations.

**Quick Structure** — thinking out loud, exploratory
> "Help me think through build vs buy for our data pipeline"

**Full Case** — specific decision with real stakes
> "Should we expand into the mid-market segment?"

**Client Deliverable** — deck-ready, stakeholder-facing
> "Draft a strategy memo for the board on our market entry options"

## What's inside

```
management-consulting/
├── SKILL.md (237 lines)                    # Core: modes, workflow, output contract
├── references/
│   ├── frameworks-strategy.md (798 lines)  # Five Forces, Value Chain, 7S, VRIO, Blue Ocean...
│   ├── frameworks-financial.md (781 lines) # Profit Tree, Revenue Tree, TAM/SAM/SOM, Unit Econ
│   ├── frameworks-decision.md (708 lines)  # RAPID, Decision Matrix, Pre-Mortem, Inversion
│   ├── frameworks-problem-solving.md (511) # MECE, Issue Tree, Hypothesis Tree, Pyramid
│   ├── frameworks-operations.md (484)      # ADKAR, Kotter, Lewin, Customer Journey, NPS
│   ├── frameworks-pricing.md (402 lines)   # Value-Based, Cost-Plus, Competitive, Dynamic, Freemium
│   ├── frameworks-innovation.md (390)      # JTBD, Business Model Canvas, Advantage Matrix
│   ├── frameworks-index.md                 # Quick-reference: all 42 frameworks, one-line each
│   ├── evidence-standards.md               # Claim labeling: Fact / Inference / Assumption
│   ├── diagram-templates.md                # 12 diagram types (SVG templates)
│   └── tooling-appendix.md                 # Optional: rendering pipeline, themes
├── examples/
│   ├── end-to-end-full-case.md             # SaaS mid-market expansion (complete walkthrough)
│   ├── end-to-end-quick-structure.md       # Build vs Buy (light mode)
│   ├── issue-tree-good-vs-bad.md           # Before/after comparison
│   └── recommendation-good-vs-bad.md       # Before/after comparison
└── variants/
    ├── market-entry.md                     # Five Forces + TAM + positioning
    ├── due-diligence.md                    # Commercial DD + red flags
    ├── org-effectiveness.md                # 7S + ADKAR + stakeholder mapping
    └── strategy-memo.md                    # Pyramid Principle + SCQA + deck outline
```

**22 files. 5,300+ lines. 287K chars.**

## Framework depth

Every framework reference file includes (per framework):

| Section | What it provides |
|---|---|
| **When to use** | The specific problem type this framework solves |
| **Step-by-step workflow** | Numbered practitioner steps — not theory, the actual work |
| **Good vs bad output** | Concrete examples with real numbers showing shallow vs actionable |
| **Common mistakes** | 3-5 things practitioners get wrong, with root cause |
| **When it breaks down** | Failure conditions — when the framework misleads |
| **Best combinations** | Which frameworks pair well, in what sequence |

### 42 frameworks across 7 categories

**Strategy (11):** Five Forces, Value Chain, 7S, VRIO, 3 Horizons, Ansoff, Growth-Share Matrix, Nine-Box, Blue Ocean, Wardley Mapping, Scenario Planning

**Problem Solving (6):** MECE, Issue Trees, Hypothesis Trees, 7-Step Problem Solving, Pyramid Principle, SCQA

**Decision Making (5):** RAPID, Decision Matrix, Pre-Mortem, Second-Order Thinking, Inversion

**Financial (5):** Profit Tree, Revenue Tree, TAM/SAM/SOM, Unit Economics, Waterfall/Bridge

**Operations (6):** ADKAR, Kotter's 8-Step, Lewin's Change Model, Influence Model, Customer Journey, NPS

**Innovation (4):** Jobs to Be Done, Business Model Canvas, Value Proposition Canvas, Advantage Matrix

**Pricing (5):** Value-Based, Cost-Plus, Competitive, Dynamic, Freemium

## How it was built

1. **3-way AI research** — Gemini, Codex, and Claude independently researched all 42 frameworks in parallel (21 research tasks, 497K chars of raw material)
2. **Synthesis** — 4 agents merged the best from each AI per category. Took the sharpest examples, cut textbook filler, resolved disagreements.
3. **3 rounds of adversarial review** — Codex (scored 7/10), Gemini (scored 9.4/10), and self-review identified gaps in portability, completeness, and actionability. All addressed.
4. **A/B eval** — 7-way comparison of different reference configurations to find the highest-impact bundle.
5. **v2 eval redesign** — 9-criteria rubric with programmatic checkers, pairwise comparison with position swap, and Gemini+Codex adversarial review of the eval plan itself. Key finding: baseline beating the skill on some prompts revealed a skill bug (hard gate too aggressive — the skill stopped at clarifying questions on vague prompts instead of stating assumptions and proceeding), not a measurement problem. But the rubric redesign was needed to properly measure process discipline, which the v1 absolute scoring missed.

## Eval results (v2)

Evaluated with [gcamilo/skill-eval](https://github.com/gcamilo/skill-eval) — an open-source A/B testing framework for AI agent skills.

**3-tier rubric, 9 criteria** across Process Discipline (problem framing, MECE structure, evidence labeling), Output Quality (specificity, so-what per finding, visual structure), and Decision Quality (options with trade-offs, falsifiability, stated assumptions).

| Tier | What it measures | Skill delta |
|------|-----------------|-------------|
| T1 — Process Discipline | Structure, framing, evidence | **+1.6** |
| T2 — Output Quality | Specificity, insights, formatting | **+0.6** |
| T3 — Decision Quality | Options, falsifiability, assumptions | **+0.4** |
| **Overall** | | **+0.9** |

**Key findings:**

- **Easy prompts show the largest gap** — T1 delta of +4.8 on straightforward prompts. The skill enforces structured process that Opus naturally skips when the question seems simple.
- **Pairwise results** — skill wins on hard and ambiguous prompts; baseline wins on well-specified prompts where the framework overhead adds less value.
- **Hard gate fix was critical** — the original skill stopped at clarifying questions on vague prompts. The fixed version states assumptions and proceeds, which is what a real consultant does.

## Customization

- **Add variants** — `variants/your-scenario.md` with upfront questions, required frameworks, deliverables
- **Add examples** — `examples/your-example.md` showing input → mode → output
- **Adjust strictness** — edit hard gate, output contract, or quality checklist in SKILL.md
- **Add frameworks** — create or extend `references/frameworks-{category}.md`

## License

MIT
