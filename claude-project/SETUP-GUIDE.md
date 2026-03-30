# Claude Project Setup Guide

## Step 1: Create the Project

1. Go to [claude.ai](https://claude.ai)
2. Click **Projects** in the left sidebar
3. Click **+ New Project**
4. Name it: **SID Blog Generator**

## Step 2: Set Project Instructions

1. Open the project
2. Click the **gear icon** (Project Settings)
3. Paste the ENTIRE contents of `PROJECT-INSTRUCTIONS.md` into the **Custom Instructions** field
4. Save

## Step 3: Upload Knowledge Files

Upload these files to the project's **Knowledge** section:

| File | Purpose |
|------|---------|
| `usa-skills-in-demand-webflow.html` | Reference template for HTML structure |
| `usa-skills-research.md` | Reference for research brief format |
| `In-Demand Skills - IT.xlsx` | Your keyword data (paste as text — see below) |

**Important:** Claude Projects can't read XLS files directly. Before each run:
1. Open your XLS in Excel
2. Copy the data (or export as CSV)
3. Paste it into the chat when starting a new article

## Step 4: How to Use

### Full Pipeline (research + HTML)
Start a new conversation in the project and type:

```
Skills in demand in {country}

Here's my keyword data:
[paste your search query data here as a table]
```

Claude will:
1. Generate the research brief (Step 1)
2. Then immediately generate the Webflow HTML (Step 2)

### Research Only
```
Research only for Germany
[paste keyword data]
```

### HTML Only (if you already have the research brief)
```
Write the HTML for Germany

Here's the research brief:
[paste the research brief from a previous conversation]
```

## Step 5: Copy the Output

- The research brief can be copied directly from the chat
- The Webflow HTML will be long — use the **Copy** button on the code block
- Paste directly into Webflow Rich Text embed blocks

## Tips

1. **Claude has a knowledge cutoff.** For the most current data, supplement by pasting recent stats/reports into the chat
2. **Long outputs may get truncated.** If the HTML gets cut off, say "continue from where you stopped" and Claude will resume
3. **Review the research brief** before proceeding to HTML. You can ask Claude to adjust skills, add/remove entries, or fix data
4. **Keyword data format:** Paste as a table with columns: Query, Clicks, Impressions, CTR, Position
