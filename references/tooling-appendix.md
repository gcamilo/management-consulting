# Tooling Appendix — Environment-Specific Rendering

This appendix covers diagram rendering, theme selection, and delivery pipelines for specific environments. The core consulting skill works without any of these — they enhance visual output when available.

## SVG Rendering Pipeline

If you have SVG rendering capabilities:

```bash
# 1. Generate SVG
cat > /tmp/diagram.svg << 'EOF'
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 600" font-family="Inter, sans-serif">
  <rect width="800" height="600" fill="#ffffff"/>
  <!-- diagram content -->
</svg>
EOF

# 2. Lint (optional — catches overlaps, tiny text, out-of-bounds)
svg-lint /tmp/diagram.svg  # if available

# 3. Convert to PNG
python3 -c "import cairosvg; cairosvg.svg2png(url='/tmp/diagram.svg', write_to='/tmp/diagram.png', scale=2)"

# 4. Deliver (adapt to your environment)
# Discord: discord file <channel> /tmp/diagram.png
# Slack: upload via API
# Web: serve directly as SVG
# Docs: embed PNG in document
```

**If cairosvg is not installed:** Output the SVG code directly — most modern tools can render it.

## Theme Palettes

Pick the theme that matches your audience:

**light** (default — docs, exports)
- bg: #ffffff, card: #f8fafc, text: #0f172a, accent: #2563eb

**dark** (Discord, dark-mode UIs)
- bg: #0f172a, card: #1e293b, text: #f8fafc, accent: #3b82f6

**consulting** (client-facing decks)
- bg: #ffffff, card: #f1f5f9, text: #1e293b, primary: #1e40af

**ib** (investment banking)
- bg: #0a1628, card: #111d33, text: #e8dcc8, primary: #c5a55a (gold)

**ft** (Financial Times / research)
- bg: #fff1e5, card: #f2dfce, text: #33302e, primary: #990f3d

## AI Image Generation

For conceptual illustrations that SVG can't capture (cover slides, visual metaphors, infographics):

Use any image generation tool available in your environment. Prompt guidance:
- Keep it professional — consulting aesthetic, not clip art
- Use for abstract concepts ("digital transformation", "market disruption")
- Do NOT use for data-driven charts or structured diagrams
- Specify style: "clean, minimal, professional, blue color scheme"

## Fallback (no visual tooling)

If no diagram tools are available, provide:
1. A structured text description of the intended visual
2. ASCII representation for simple trees/matrices
3. A markdown table as a last resort

The analysis is more important than the visual. Never skip insights because you can't render a diagram.
