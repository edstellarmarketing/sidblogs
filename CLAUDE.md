# Skills in Demand (SID) Blog Pipeline — Project Instructions

## SID Overview

A multi-agent pipeline for producing Edstellar "Skills in Demand in {Country}" blog posts.
These are interactive, data-driven articles with skill cards, salary explorers, quizzes, and visa
pathway guides. The template is based on `skills-in-demand-australia.html`.

## SID Agent Pipeline

```
SID Agent 0 (Skills Researcher) ──┐
                                    ├── SID Agent 1 (SVG Generator) ──┐
SID Agent 2 (Keyword Researcher) ──┘                                   ├── SID Agent 3  (Blog Assembler)  → Standalone HTML
(optional, can be skipped)                                             ├── SID Agent 3W (Webflow Builder) → Webflow HTML
                                    └──────────────────────────────────┘
```

**SID Agent 0** (`sid-skills-researcher`) researches all factual data: labour market stats, skills
list, salary ranges, visa pathways, expert quotes, quiz data, and FAQ content.
**SID Agent 1** (`sid-svg-generator`) generates animated SVG banner images for each skill card.
Runs AFTER Agent 0 (needs the skill list).
**SID Agent 2** (`sid-keyword-researcher`) discovers competitor keywords for skills-in-demand content.
Runs IN PARALLEL with Agent 0 (no dependency). **Optional — can be skipped for faster runs.**
**SID Agent 3** (`sid-blog-assembler`) takes outputs and produces standalone HTML (with JS interactivity).
**SID Agent 3W** (`sid-webflow-builder`) takes outputs and produces Webflow-ready HTML with
`data-rt-embed-type="true"` wrappers, single-quoted attributes, injected CSS, static versions
of interactive elements, and no JS/document scaffolding. **This is the preferred output format.**

## How to Trigger the SID Pipeline

### Full SID Pipeline

When the user says any of the following, run the full pipeline:
- "I need article for skills in demand in {country}"
- "Skills in demand in {country}"
- "Create skills in demand blog for {country}"
- "Generate the {country} skills blog"
- "Run the SID pipeline for {country}"
- "New skills in demand for {country}"
- "Build the skills in demand {country} blog"

**Optimized Sequence (default):**
1. Run `sid-skills-researcher` (Agent 0) only (skip Agent 2 for speed)
   - Agent 0 saves the skills research brief
2. After Agent 0 completes, run `sid-svg-generator` (Agent 1)
   - Agent 1 reads the skills list from Agent 0's output and generates SVGs
3. After Agent 1 completes, run `sid-webflow-builder` (Agent 3W) — the **default output format**
   - Agent 3W reads research brief + SVGs and produces Webflow-ready HTML
4. Final HTML saved to `outputs/{country-slug}-skills-in-demand-webflow.html`

**If the user explicitly asks for standalone HTML instead of Webflow**, run `sid-blog-assembler`
(Agent 3) at step 3 instead. Use the pre-cached template at `templates/sid-template.html`.

**If the user asks for keyword research**, add Agent 2 in parallel with Agent 0 at step 1.

### Partial SID Pipeline — Skills Research Only

When the user says any of the following, run ONLY SID Agent 0:
- "Research skills for {country}"
- "Find in-demand skills in {country}"
- "Run SID Agent 0 for {country}"
- "Skills data for {country}"

### Partial SID Pipeline — SVG Generation Only

When the user says any of the following, run ONLY SID Agent 1:
- "Generate SVGs for {country} skills"
- "Create skill card images for {country}"
- "Run SID Agent 1 for {country}"

When running SID Agent 1 alone, check if the skills research brief exists in outputs.
If missing, warn: "No skills research brief found. Run SID Agent 0 first."

### Partial SID Pipeline — Keyword Research Only

When the user says any of the following, run ONLY SID Agent 2:
- "Find keywords for {country} skills blog"
- "Research skills in demand keywords for {country}"
- "Run SID Agent 2 for {country}"
- "SID keyword brief for {country}"

### Partial SID Pipeline — Blog Assembly Only (Standalone HTML)

When the user says any of the following, run ONLY SID Agent 3:
- "Assemble the {country} skills blog"
- "Generate the standalone skills in demand HTML for {country}"
- "Run SID Agent 3 for {country}"

When running SID Agent 3 alone, check if research brief and SVGs exist in outputs.
Warn for any missing inputs before proceeding.

### Partial SID Pipeline — Webflow Builder Only

When the user says any of the following, run ONLY SID Agent 3W:
- "Build the Webflow skills blog for {country}"
- "Generate Webflow SID HTML for {country}"
- "Run SID Webflow builder for {country}"
- "Create Webflow version of {country} skills blog"
- "Convert {country} skills blog to Webflow"
- "Webflow format for {country} skills in demand"

When running SID Agent 3W alone, check if research brief and SVGs exist in outputs.
Warn for any missing inputs before proceeding.

## SID Output Files

| SID Agent | Output File | Format |
|-----------|-----------|--------|
| SID Agent 0 | `{country-slug}-skills-research.md` | Markdown |
| SID Agent 1 | `{country-slug}-skill-svgs.md` | Markdown (with SVG code) |
| SID Agent 2 | `{country-slug}-sid-keyword-brief.md` | Markdown (optional) |
| SID Agent 3 | `{country-slug}-skills-in-demand.html` | HTML (standalone, with JS) |
| SID Agent 3W | `{country-slug}-skills-in-demand-webflow.html` | HTML (Webflow-ready, no JS) |

## SID Agent Data Flow

### SID Agent 0 + Agent 2 (parallel, no dependency)
These two agents run simultaneously. Agent 0 researches factual data. Agent 2 researches
keywords. Neither needs the other's output.

### SID Agent 0 → Agent 1 (sequential dependency)
Agent 1 MUST wait for Agent 0 to complete. It reads the skills list from the research brief
to know which skills need SVGs and what sector each belongs to.

### All → Agent 3 or Agent 3W (requires research brief + SVGs)
Agent 3 (standalone) and Agent 3W (Webflow) both need the research brief and SVGs.
The keyword brief is optional — if available, it improves SEO but is not required.
Agent 3W is the **default** output format. Agent 3 is used only when the user explicitly
requests standalone HTML.

## Important SID Pipeline Rules

1. **Agent 2 is optional.** Skip it by default for faster runs (~7 min saved). Run only if user requests keywords.
2. **Agent 1 runs after Agent 0.** It needs the skill list to generate the right SVGs.
3. **Agent 3W is the default output agent.** Use Webflow format unless user explicitly asks for standalone HTML.
4. **Agent 3/3W require research brief + SVGs.** Keyword brief is optional.
5. **Flexible skill count.** The number of skills varies by country (typically 8-15). Do not force a specific number.
6. **Local currency only.** All monetary values in the country's local currency.
7. **No em-dashes.** All SID agents enforce em-dash replacement in their outputs.
8. **Edstellar is a corporate training company.** Never call it a "platform" in any SID output.
9. **Keywords must be evidence-based.** SID Agent 2 extracts only from competitor pages.
10. **SVG IDs must be globally unique.** SID Agent 1 uses prefixed IDs to prevent DOM conflicts.
11. **All agents share the outputs directory.** SID files use distinct naming (`-skills-research.md`,
    `-skill-svgs.md`, `-sid-keyword-brief.md`, `-skills-in-demand.html`, `-skills-in-demand-webflow.html`).
12. **Use pre-cached template.** Agent 3 uses `templates/sid-template.html` instead of parsing the
    Australia template. Agent 3W has its own CSS patterns built into its skill definition.
