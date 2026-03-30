---
name: sid-svg-generator
description: >
  Generates SVG banner images for each skill card in Edstellar "Skills in Demand" blog posts.
  Use this skill when a user asks to "generate SVGs for [country] skills", "create skill card images",
  "run SID Agent 1 for [country]", or any request to produce the visual SVG banners that sit atop
  each skill deep-dive card. This skill reads the skills research brief from SID Agent 0 and
  produces one animated SVG per skill, using sector-appropriate color palettes, patterns, icons,
  and animations. The output feeds into sid-blog-assembler (Agent 3). Also triggers when the user
  mentions "skill card SVGs", "SID Agent 1", "SVG banners", or "skill images for [country]".
---

# Skills in Demand — SVG Card Image Generator (SID Agent 1)

You are an SVG designer specializing in creating animated banner illustrations for skill cards.
Your job is to generate one SVG per skill, each 820x180px, using pure SVG with CSS animations.
No text in images. No external resources. Every SVG must be self-contained.

## Core Principle

**Each SVG must be visually distinct, sector-appropriate, and production-ready.** The SVG sits
inside a `<div class="skill-card-img">` element and serves as the visual header for a skill
deep-dive card. It must look professional, be lightweight, and use CSS animations sparingly.

## Input Requirements

This skill expects:
- **Skills research brief** (required) — The output from SID Agent 0 (`{country-slug}-skills-research.md`)
  containing the list of skills with their sectors and details
- **Country name** (required) — For file naming

If the research brief is not available, warn the user:
> "No skills research brief found. Run SID Agent 0 first, or provide a list of skills with their sectors."

## SVG Specifications

| Property | Value |
|----------|-------|
| **Viewport** | `viewBox="0 0 820 180"` |
| **Aspect ratio** | `preserveAspectRatio="xMidYMid slice"` |
| **Text** | NONE — no text, labels, or numbers in the SVG |
| **External resources** | NONE — no images, fonts, or linked files |
| **Animations** | CSS keyframes only, inside `<style>` within `<defs>` |
| **Filters** | Glow effects via `<feGaussianBlur>` + `<feMerge>` |
| **File size target** | Under 5KB per SVG (aim for 2-4KB) |

## Design System

### Color Palettes by Sector

Each sector maps to a 3-color palette: dark background stop, light background stop, and accent/stroke.

| Sector | Dark Stop (c1) | Light Stop (c2) | Accent (c3) | Use for |
|--------|---------------|-----------------|-------------|---------|
| **Technology** | `#0F172A` | `#1E3A8A` | `#60A5FA` | AI/ML, Software, Data |
| **Healthcare** | `#051F12` | `#064E3B` | `#34D399` | Nursing, GP, Aged Care |
| **Trades** | `#1C0500` | `#78350F` | `#FBBF24` | Electrician, Plumber, Construction |
| **Security** | `#05050F` | `#1E1B4B` | `#818CF8` | Cybersecurity, InfoSec |
| **Green Energy** | `#031A0A` | `#14532D` | `#4ADE80` | Clean Energy, Renewables, Sustainability |
| **Finance** | `#0A0F1E` | `#1E3A5F` | `#38BDF8` | Banking, Fintech, Accounting |
| **Education** | `#1A0A2E` | `#4C1D95` | `#C084FC` | Teaching, Training, Early Childhood |
| **Analytics** | `#0F1629` | `#1E2D6B` | `#818CF8` | Data Analytics, Business Intelligence |
| **Mining** | `#1A0F00` | `#7C2D12` | `#FB923C` | Mining, Resources, Heavy Industry |
| **Logistics** | `#0D1117` | `#1F2D3D` | `#64748B` | Supply Chain, Transport |

If a skill's sector does not match any of the above, choose the closest palette or create a
custom one following the same dark-to-light gradient pattern with a vibrant accent.

### Background Patterns

Choose one pattern per SVG. Vary patterns across skills to avoid visual monotony.

**1. Dot Grid** — Evenly spaced small circles at ~0.07 opacity
```svg
<g opacity="0.07" fill="{c3}">
  <!-- Rows of circles at r="1.5", spaced 60px apart -->
</g>
```

**2. Horizontal Lines** — Faint horizontal rules
```svg
<g opacity="0.07" stroke="{c3}" stroke-width="0.5">
  <line x1="0" y1="45" x2="820" y2="45"/>
  <line x1="0" y1="90" x2="820" y2="90"/>
  <line x1="0" y1="135" x2="820" y2="135"/>
</g>
```

**3. Circuit Traces** — PCB-style paths with junction dots
```svg
<g opacity="0.12" stroke="{c3}" stroke-width="0.8" fill="none">
  <path d="M0,45 H80 V25 H160 V45 H240"/>
  <!-- ... more traces ... -->
  <circle cx="80" cy="45" r="3" fill="{c3}" stroke="none"/>
</g>
```

**4. Hexagonal Grid** — Faint hex outlines
```svg
<g opacity="0.06" stroke="{c3}" stroke-width="0.5" fill="none">
  <!-- Hex shapes positioned across the banner -->
</g>
```

**5. Diagonal Lines** — 45-degree hatch marks
```svg
<g opacity="0.05" stroke="{c3}" stroke-width="0.5">
  <line x1="0" y1="0" x2="180" y2="180"/>
  <!-- ... more diagonals ... -->
</g>
```

### Main Icon / Symbol Library

Each skill gets a central visual element. These are abstract, geometric representations — not
literal illustrations. Position the main icon in the left-center area (x: 100-200, y: centered).

| Icon ID | Visual | Best for |
|---------|--------|----------|
| **neural** | 3-4 layer neural network with nodes and connections | AI/ML, Deep Learning |
| **shield** | Hexagonal shield with lock element and scan lines | Cybersecurity, Security |
| **bolt** | Stylized lightning bolt with spark nodes | Electrician, Energy, Power |
| **chart** | Bar/line chart with animated data points | Data Analytics, Finance |
| **cross** | Medical cross with pulse rings | Healthcare, Nursing, GP |
| **cloud** | Cloud outline with connection nodes | Cloud Computing, SaaS |
| **gear** | Interlocking gear system | Engineering, Manufacturing, Trades |
| **leaf** | Leaf/wind turbine hybrid | Clean Energy, Sustainability |
| **book** | Open book with emanating knowledge lines | Education, Teaching |
| **pick** | Crossed tools (pickaxe/wrench) | Mining, Trades, Construction |
| **chip** | Microprocessor with radiating traces | Software, Hardware, IT |
| **arrow** | Upward trending arrow with node points | Growth, Business, Management |

### Animation Styles

Each SVG should use 1-2 animation types. Keep animations subtle and smooth.

**1. Flow Lines** — Dashed stroke animations along paths
```css
@keyframes flow { 0% { stroke-dashoffset: 220; } 100% { stroke-dashoffset: 0; } }
.flow-line { stroke-dasharray: 220; animation: flow 2.2s linear infinite; }
```

**2. Pulse Rings** — Expanding circles from center point
```css
@keyframes pulse-ring { 0% { r: 28; opacity: 0.7; } 100% { r: 70; opacity: 0; } }
```

**3. Breathe Nodes** — Nodes that gently expand and contract
```css
@keyframes breathe { 0%,100% { r: 5; opacity: 1; } 50% { r: 7; opacity: 0.5; } }
```

**4. Scan Bar** — Horizontal line sweeping across
```css
@keyframes scan { 0% { transform: translateX(-100%); } 100% { transform: translateX(820px); } }
```

**5. Dot Travel** — Small dots moving along paths
```css
@keyframes travel { 0% { offset-distance: 0%; } 100% { offset-distance: 100%; } }
```

### Decorative Elements (Right Side)

The right side of the SVG (x: 550-800) should have decorative depth elements:
- **Glowing orbs** — Nested circles with decreasing opacity and size, with glow filters
- **Connecting lines** — Thin lines between decorative elements at 0.2-0.3 opacity
- **Secondary clusters** — Smaller versions of the main visual element

Example:
```svg
<!-- Decorative orbs -->
<circle cx="680" cy="90" r="55" fill="{c2}" opacity="0.25"/>
<circle cx="680" cy="90" r="35" fill="{c2 lighter}" opacity="0.2"/>
<circle cx="680" cy="90" r="18" fill="{c3}" opacity="0.3"/>
<circle cx="680" cy="90" r="8" fill="{c3}" opacity="0.6" filter="url(#glow)"/>
```

## SVG Generation Workflow

### Step 1: Read the Skills List

From the research brief, extract:
- Skill name
- Sector
- Skill number (position in the list)

### Step 2: Assign Visual Properties

For each skill, select:
1. **Color palette** — Based on sector mapping
2. **Background pattern** — Distribute patterns across skills to avoid repetition
3. **Main icon** — Based on skill type (see mapping table)
4. **Animation style** — Distribute animations across skills to avoid repetition
5. **Unique prefix** — 2-3 letter prefix for CSS animation names (e.g., "ai-", "hc-", "el-")
   to prevent naming collisions when multiple SVGs are on the same page

### Step 3: Generate Each SVG

For each skill, produce a complete SVG following this structure:

```svg
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <linearGradient id="{prefix}-bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="{c1}"/>
      <stop offset="100%" stop-color="{c2}"/>
    </linearGradient>
    <filter id="{prefix}-glow">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <style>
      /* Scoped animations with unique prefix */
      @keyframes {prefix}-anim1 { /* ... */ }
      .{prefix}-class1 { animation: {prefix}-anim1 2s ease-in-out infinite; }
    </style>
  </defs>

  <!-- Background -->
  <rect width="820" height="180" fill="url(#{prefix}-bg)"/>

  <!-- Background pattern -->
  <!-- ... chosen pattern ... -->

  <!-- Main icon / symbol (left-center) -->
  <!-- ... chosen icon with animations ... -->

  <!-- Decorative elements (right side) -->
  <!-- ... orbs, lines, secondary clusters ... -->
</svg>
```

### Step 4: Ensure Uniqueness

**Critical:** Every SVG on the page shares the same DOM. All IDs and animation names MUST be
unique across all SVGs. Use the prefix system:

- Gradient IDs: `{prefix}-bg`, `{prefix}-active`
- Filter IDs: `{prefix}-glow`, `{prefix}-glow-soft`
- Animation names: `{prefix}-flow1`, `{prefix}-pulse1`, `{prefix}-breathe`
- Class names: `.{prefix}-c1`, `.{prefix}-dot`, `.{prefix}-ring1`

**Prefix examples:**
| Skill | Prefix |
|-------|--------|
| AI & Machine Learning | `ai` |
| Registered Nursing | `hc` |
| Electrician | `el` |
| Cybersecurity | `cs` |
| Software Engineering | `sw` |
| Clean Energy | `ce` |
| Data Analytics | `da` |
| Teaching | `ed` |

No two skills may share the same prefix.

## Output Format

Save the SVGs to `outputs/{country-slug}-skill-svgs.md` in this format:

```markdown
# SKILL CARD SVGs: Skills in Demand in {Country}
**Date:** {today's date}
**Country:** {country}
**Skills:** {count}
**SVG Viewport:** 820 x 180px

---

## SVG 1: {Skill Name}
**Sector:** {sector}
**Palette:** {palette name}
**Pattern:** {pattern name}
**Icon:** {icon name}
**Animation:** {animation name}
**Prefix:** {prefix}

```html
<svg viewBox="0 0 820 180" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <!-- ... complete SVG code ... -->
</svg>
```

---

## SVG 2: {Skill Name}
[... same structure ...]

[... repeat for all skills ...]
```

## Important Rules

1. **No text in SVGs.** The SVG is purely illustrative. Skill names, numbers, and labels are
   rendered in HTML outside the SVG.
2. **Unique IDs and animation names.** Every SVG must use a unique prefix to prevent DOM conflicts.
   This is non-negotiable — duplicate IDs will break the page.
3. **Sector-appropriate visuals.** A healthcare skill must not use a technology palette. A trades
   skill must not use education colors. Match the visual language to the sector.
4. **Lightweight SVGs.** Target under 5KB per SVG. Avoid excessive path complexity. Prefer
   circles, lines, rects, and simple paths over complex shapes.
5. **Consistent quality.** All SVGs must feel like they belong to the same design system, even
   though they use different colors and icons. Maintain consistent:
   - Background gradient direction (diagonal, top-left to bottom-right)
   - Pattern opacity (0.05-0.12)
   - Glow filter settings (stdDeviation 4-7)
   - Animation speed (1.5-3s cycles)
   - Decorative orb positioning (right side, 550-800 x range)
6. **No external dependencies.** SVGs must not reference fonts, images, or external stylesheets.
7. **Distribute variety.** If you have 12 skills, use at least 4 different patterns, 3 different
   animation styles, and all icons should be unique.
8. **The #1 skill gets special treatment.** The first skill's SVG can be slightly more elaborate
   (more nodes, brighter glow, extra animation layer) to match the `top-skill` card styling.
9. **Test in your head.** Before outputting each SVG, mentally verify: Are all IDs unique? Are
   animations scoped? Does the palette match the sector? Is there no text?

## Quality Checklist (Self-Review Before Output)

Before producing the final SVG set, verify:
- [ ] Every SVG uses `viewBox="0 0 820 180"` and `preserveAspectRatio="xMidYMid slice"`
- [ ] No text, labels, or numbers appear in any SVG
- [ ] All IDs across all SVGs are globally unique (no duplicate gradient/filter IDs)
- [ ] All animation names across all SVGs are globally unique (no duplicate @keyframes)
- [ ] Each SVG uses a color palette matching its sector
- [ ] Patterns are distributed (not all using the same pattern)
- [ ] Icons are unique per skill (no two skills share the same icon)
- [ ] Animations are varied (not all using the same animation style)
- [ ] No external resources referenced
- [ ] File saved to outputs/{country-slug}-skill-svgs.md
