# Consulting Diagram Templates

SVG templates for the most common consulting diagrams. Copy, modify, and render.

**Themes:** All templates below use `dark` theme. To adapt:
- `consulting` theme: bg=#ffffff, card=#f1f5f9, text=#1e293b, border=#cbd5e1, primary=#1e40af
- `ib` theme: bg=#0a1628, card=#111d33, text=#e8dcc8, border=#2a3a52, primary=#c5a55a, header-font=Georgia
- `ft` theme: bg=#fff1e5, card=#f2dfce, text=#33302e, border=#e0c9b1, primary=#990f3d, header-font=Georgia
- `light` theme: bg=#ffffff, card=#f8fafc, text=#0f172a, border=#e2e8f0, primary=#2563eb

Replace `fill`, `stroke`, and `font-family` values accordingly.

## Issue Tree

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 500" font-family="Inter, sans-serif">
  <rect width="900" height="500" fill="#0f172a"/>

  <!-- Root problem -->
  <rect x="350" y="20" width="200" height="45" rx="8" fill="#1e293b" stroke="#f59e0b" stroke-width="2"/>
  <text x="450" y="48" text-anchor="middle" font-size="13" font-weight="600" fill="#f8fafc">[Problem Statement]</text>

  <!-- Level 1 branches -->
  <line x1="450" y1="65" x2="150" y2="110" stroke="#475569" stroke-width="1"/>
  <line x1="450" y1="65" x2="450" y2="110" stroke="#475569" stroke-width="1"/>
  <line x1="450" y1="65" x2="750" y2="110" stroke="#475569" stroke-width="1"/>

  <rect x="50" y="110" width="200" height="40" rx="6" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="150" y="135" text-anchor="middle" font-size="11" fill="#93c5fd">[Branch 1]</text>

  <rect x="350" y="110" width="200" height="40" rx="6" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="450" y="135" text-anchor="middle" font-size="11" fill="#93c5fd">[Branch 2]</text>

  <rect x="650" y="110" width="200" height="40" rx="6" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="750" y="135" text-anchor="middle" font-size="11" fill="#93c5fd">[Branch 3]</text>

  <!-- Level 2 sub-branches (repeat pattern) -->
  <!-- Color code: green=#22c55e (supports), red=#ef4444 (contradicts), gray=#6b7280 (unknown) -->
</svg>
```

## 2x2 Matrix (Growth-Share / Positioning)

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 600 600" font-family="Inter, sans-serif">
  <rect width="600" height="600" fill="#0f172a"/>

  <!-- Title -->
  <text x="300" y="35" text-anchor="middle" font-size="16" font-weight="700" fill="#f8fafc">[Matrix Title]</text>

  <!-- Axes -->
  <line x1="100" y1="80" x2="100" y2="520" stroke="#475569" stroke-width="2"/>
  <line x1="100" y1="520" x2="540" y2="520" stroke="#475569" stroke-width="2"/>

  <!-- Axis labels -->
  <text x="320" y="560" text-anchor="middle" font-size="12" fill="#94a3b8">[X-axis label] →</text>
  <text x="40" y="300" text-anchor="middle" font-size="12" fill="#94a3b8" transform="rotate(-90,40,300)">↑ [Y-axis label]</text>

  <!-- Quadrant labels -->
  <text x="210" y="190" text-anchor="middle" font-size="14" font-weight="600" fill="#f59e0b">★ [Top-Left]</text>
  <text x="430" y="190" text-anchor="middle" font-size="14" font-weight="600" fill="#22c55e">★ [Top-Right]</text>
  <text x="210" y="420" text-anchor="middle" font-size="14" font-weight="600" fill="#ef4444">[Bottom-Left]</text>
  <text x="430" y="420" text-anchor="middle" font-size="14" font-weight="600" fill="#3b82f6">[Bottom-Right]</text>

  <!-- Divider lines -->
  <line x1="320" y1="80" x2="320" y2="520" stroke="#334155" stroke-width="1" stroke-dasharray="4,4"/>
  <line x1="100" y1="300" x2="540" y2="300" stroke="#334155" stroke-width="1" stroke-dasharray="4,4"/>

  <!-- Data points (circles sized by importance) -->
  <circle cx="200" cy="150" r="25" fill="#f59e0b" fill-opacity="0.3" stroke="#f59e0b" stroke-width="1.5"/>
  <text x="200" y="155" text-anchor="middle" font-size="9" fill="#f8fafc">[Item]</text>
</svg>
```

## Five Forces

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 700 500" font-family="Inter, sans-serif">
  <rect width="700" height="500" fill="#0f172a"/>

  <!-- Center: Rivalry -->
  <rect x="250" y="185" width="200" height="80" rx="10" fill="#1e293b" stroke="#ef4444" stroke-width="2"/>
  <text x="350" y="218" text-anchor="middle" font-size="12" font-weight="600" fill="#f8fafc">Industry Rivalry</text>
  <text x="350" y="238" text-anchor="middle" font-size="10" fill="#fca5a5">[HIGH/MED/LOW]</text>
  <text x="350" y="255" text-anchor="middle" font-size="9" fill="#94a3b8">[Key driver]</text>

  <!-- Top: New Entrants -->
  <rect x="250" y="30" width="200" height="65" rx="10" fill="#1e293b" stroke="#3b82f6" stroke-width="1.5"/>
  <text x="350" y="55" text-anchor="middle" font-size="11" font-weight="600" fill="#93c5fd">Threat of New Entrants</text>
  <text x="350" y="75" text-anchor="middle" font-size="10" fill="#94a3b8">[HIGH/MED/LOW]</text>
  <line x1="350" y1="95" x2="350" y2="185" stroke="#3b82f6" stroke-width="1.5" marker-end="url(#arrow)"/>

  <!-- Bottom: Substitutes -->
  <rect x="250" y="370" width="200" height="65" rx="10" fill="#1e293b" stroke="#a855f7" stroke-width="1.5"/>
  <text x="350" y="395" text-anchor="middle" font-size="11" font-weight="600" fill="#c084fc">Threat of Substitutes</text>
  <text x="350" y="415" text-anchor="middle" font-size="10" fill="#94a3b8">[HIGH/MED/LOW]</text>
  <line x1="350" y1="265" x2="350" y2="370" stroke="#a855f7" stroke-width="1.5"/>

  <!-- Left: Supplier Power -->
  <rect x="20" y="195" width="170" height="65" rx="10" fill="#1e293b" stroke="#f59e0b" stroke-width="1.5"/>
  <text x="105" y="220" text-anchor="middle" font-size="11" font-weight="600" fill="#fbbf24">Supplier Power</text>
  <text x="105" y="240" text-anchor="middle" font-size="10" fill="#94a3b8">[HIGH/MED/LOW]</text>
  <line x1="190" y1="225" x2="250" y2="225" stroke="#f59e0b" stroke-width="1.5"/>

  <!-- Right: Buyer Power -->
  <rect x="510" y="195" width="170" height="65" rx="10" fill="#1e293b" stroke="#22c55e" stroke-width="1.5"/>
  <text x="595" y="220" text-anchor="middle" font-size="11" font-weight="600" fill="#86efac">Buyer Power</text>
  <text x="595" y="240" text-anchor="middle" font-size="10" fill="#94a3b8">[HIGH/MED/LOW]</text>
  <line x1="450" y1="225" x2="510" y2="225" stroke="#22c55e" stroke-width="1.5"/>
</svg>
```

## Profit Tree

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 400" font-family="Inter, sans-serif">
  <rect width="900" height="400" fill="#0f172a"/>

  <!-- Profit -->
  <rect x="10" y="160" width="120" height="50" rx="8" fill="#1e293b" stroke="#f59e0b" stroke-width="2"/>
  <text x="70" y="182" text-anchor="middle" font-size="13" font-weight="700" fill="#f59e0b">Profit</text>
  <text x="70" y="200" text-anchor="middle" font-size="10" fill="#94a3b8">$[X]M</text>

  <!-- Revenue branch -->
  <line x1="130" y1="175" x2="180" y2="100" stroke="#22c55e" stroke-width="1.5"/>
  <rect x="180" y="75" width="120" height="50" rx="6" fill="#1e293b" stroke="#22c55e" stroke-width="1.5"/>
  <text x="240" y="97" text-anchor="middle" font-size="12" font-weight="600" fill="#86efac">Revenue</text>
  <text x="240" y="115" text-anchor="middle" font-size="10" fill="#94a3b8">$[X]M</text>

  <!-- Price x Volume -->
  <line x1="300" y1="90" x2="360" y2="40" stroke="#22c55e" stroke-width="1"/>
  <line x1="300" y1="110" x2="360" y2="140" stroke="#22c55e" stroke-width="1"/>
  <rect x="360" y="15" width="100" height="45" rx="5" fill="#1e293b" stroke="#475569" stroke-width="1"/>
  <text x="410" y="35" text-anchor="middle" font-size="10" fill="#94a3b8">Price</text>
  <text x="410" y="50" text-anchor="middle" font-size="10" fill="#64748b">$[X]</text>
  <rect x="360" y="120" width="100" height="45" rx="5" fill="#1e293b" stroke="#475569" stroke-width="1"/>
  <text x="410" y="140" text-anchor="middle" font-size="10" fill="#94a3b8">Volume</text>
  <text x="410" y="155" text-anchor="middle" font-size="10" fill="#64748b">[X] units</text>

  <!-- Cost branch -->
  <line x1="130" y1="195" x2="180" y2="275" stroke="#ef4444" stroke-width="1.5"/>
  <rect x="180" y="250" width="120" height="50" rx="6" fill="#1e293b" stroke="#ef4444" stroke-width="1.5"/>
  <text x="240" y="272" text-anchor="middle" font-size="12" font-weight="600" fill="#fca5a5">Costs</text>
  <text x="240" y="290" text-anchor="middle" font-size="10" fill="#94a3b8">$[X]M</text>

  <!-- Fixed + Variable -->
  <line x1="300" y1="265" x2="360" y2="230" stroke="#ef4444" stroke-width="1"/>
  <line x1="300" y1="285" x2="360" y2="320" stroke="#ef4444" stroke-width="1"/>
  <rect x="360" y="210" width="100" height="45" rx="5" fill="#1e293b" stroke="#475569" stroke-width="1"/>
  <text x="410" y="230" text-anchor="middle" font-size="10" fill="#94a3b8">Fixed</text>
  <text x="410" y="245" text-anchor="middle" font-size="10" fill="#64748b">$[X]M</text>
  <rect x="360" y="300" width="100" height="45" rx="5" fill="#1e293b" stroke="#475569" stroke-width="1"/>
  <text x="410" y="320" text-anchor="middle" font-size="10" fill="#94a3b8">Variable</text>
  <text x="410" y="335" text-anchor="middle" font-size="10" fill="#64748b">$[X]M</text>
</svg>
```

## Value Chain

Horizontal flow of primary activities: **Inbound Logistics -> Operations -> Outbound Logistics -> Marketing & Sales -> Service**. Support activities (firm infrastructure, HR, technology, procurement) run as a horizontal bar above the primary chain. Each activity box includes a cost % annotation (e.g., "23% of total cost"). Highlight the 1-2 activities where the company has a cost or differentiation advantage with a distinct border color (green for advantage, red for disadvantage).

SVG structure: 5 primary-activity rects in a row (connected by arrows), a wide support-activity rect spanning the top, percentage labels inside each box. Use the same theme palette as other templates.

## Customer Journey Map

Horizontal timeline with 6 stages: **Awareness -> Consideration -> Purchase -> Onboarding -> Retention -> Expansion**. Each stage is a column. Above the stages, plot an emotion line (curve connecting happy/neutral/frustrated icons or colored dots: green=happy, yellow=neutral, red=frustrated). Below each stage, annotate 1-2 pain points in small text. Touchpoints (e.g., "website", "sales call", "onboarding email") appear as labels within each column.

SVG structure: 6 column rects, a polyline/path for the emotion curve above them, emoji or colored circles at each stage's emotion level, pain-point text below. Horizontal arrows connect the stage headers.

## Decision Tree

Binary branching nodes with probabilities and expected values. Root node = the decision. Each branch is labeled with a choice or outcome and a probability (e.g., "P=0.6"). Leaf nodes show the expected value (e.g., "$2.4M") and are color-coded: green for favorable outcomes, red for unfavorable, gray for break-even. Interior decision nodes use diamond shapes; chance nodes use circles.

SVG structure: diamonds (decisions) and circles (chance nodes) connected by angled lines. Probability labels on each branch. Leaf rects with EV values. Use `fill-opacity` to distinguish node types.

## Swimlane / Process Flow

Horizontal lanes, one per role or department (e.g., "Customer", "Sales", "Engineering", "Finance"). Process steps flow left-to-right as rounded rects within each lane. Arrows connect steps, crossing lane boundaries to show handoffs. Handoff arrows use a distinct color (amber) to highlight friction points. Each lane has a light background tint for visual separation.

SVG structure: horizontal band rects for lanes (alternating fill shades), process-step rects within lanes, arrow paths (straight or right-angle) between steps. Lane labels on the left margin.

## Risk Matrix

3x3 or 5x5 grid. X-axis = **Likelihood** (low -> medium -> high). Y-axis = **Impact** (low -> medium -> high). Grid cells are color-coded: bottom-left zone = green (accept), diagonal = yellow (mitigate), top-right = red (avoid/transfer). Risks plotted as labeled circles positioned within the appropriate cell. Circle size can encode a secondary dimension (e.g., cost exposure).

SVG structure: grid of rects with fill colors (green/yellow/red zones), circle elements for each risk with text labels, axis labels on margins. A legend maps colors to response strategies.

## Wardley Map

X-axis = **Evolution** with 4 labeled stages: Genesis -> Custom-Built -> Product (+rental) -> Commodity (+utility). Y-axis = **Value Chain** (user-visible at top, infrastructure at bottom). Components are plotted as labeled circles at their (evolution, value-chain) position. Movement arrows show expected evolution direction (rightward). Dependencies are shown as lines connecting components vertically. Anchor components (user needs) sit at the top.

SVG structure: axis lines with stage labels, dashed vertical dividers between evolution stages, circle elements for components with text labels, arrow paths for movement, line paths for dependencies. Background shading gets lighter from left (genesis=darker) to right (commodity=lighter) to visually encode maturity.

## Waterfall / Bridge Chart

Use matplotlib for data-driven waterfalls:

```python
import matplotlib; matplotlib.use('Agg')
import matplotlib.pyplot as plt
import numpy as np

plt.style.use('dark_background')
fig, ax = plt.subplots(figsize=(10, 5))

categories = ['Base', 'Price', 'Volume', 'COGS', 'SGA', 'New']
values = [100, 15, 8, -12, -5, 106]
colors = ['#3b82f6', '#22c55e', '#22c55e', '#ef4444', '#ef4444', '#f59e0b']

# Calculate cumulative for waterfall positioning
cumulative = [0]
for i, v in enumerate(values[:-1]):
    cumulative.append(cumulative[-1] + v)

bottoms = [0] + cumulative[1:]
bottoms[-1] = 0  # last bar starts from 0

ax.bar(categories, values, bottom=bottoms, color=colors, edgecolor='#1e293b', width=0.6)

# Add value labels
for i, (cat, val, bot) in enumerate(zip(categories, values, bottoms)):
    y = bot + val/2
    ax.text(i, y, f'${val:+d}M' if i not in [0, len(values)-1] else f'${val}M',
            ha='center', va='center', fontsize=10, fontweight='bold', color='white')

ax.set_title('[Title] — Revenue Bridge', fontsize=14, fontweight='bold', pad=15)
ax.set_ylabel('$M')
ax.spines[['top', 'right']].set_visible(False)
plt.tight_layout()
plt.savefig('/tmp/waterfall.png', dpi=150, bbox_inches='tight')
```
