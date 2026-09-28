# Research Skill

## Purpose

Take a topic from `content/ideas/` and research it, producing a structured research brief that the writing skill will use to draft a LinkedIn post.

## Input

- Topic file: `content/ideas/NNN-slug.md` with minimal metadata
- Frontmatter fields used: `topic`, `subtopic` (if present)
- Body: empty or contains a rough prompt/angle

## Process

1. **Understand the topic.** Read the topic slug and frontmatter to understand what angle or subtopic the topic targets.
2. **Research.** Gather information about:
   - The technical/business mechanics of the topic (how it works, what's changing, why it matters)
   - Real-world examples or case studies relevant to Ampfield's audience (utilities, renewable developers, policy analysts)
   - How this topic relates to grid-scale battery storage and balancing
   - Any recent industry shifts, policy changes, or data that should inform the post
3. **Structure the brief.** Add a `research_brief` section to the topic file with:
   - **Context:** 1–2 sentences on why this topic matters now
   - **Key facts:** 3–5 bullet points with specific numbers, mechanisms, or examples
   - **Audience angles:** how each ICP (utility planner, renewable developer, policy analyst) sees this topic
   - **Risks:** what claims to avoid or nuance that must be included
4. **Move the file.** Once research is done, move the topic file from `content/ideas/` to `content/drafts/`.
5. **Document.** Log the research step in the file's frontmatter: `stage: draft` and `researched_at: YYYY-MM-DD`.

## Example output

```markdown
---
topic: Why Utilities Pair Storage with Solar Now
subtopic: Grid-scale storage drivers
created_at: 2026-09-28
stage: draft
researched_at: 2026-09-28
---

## research_brief

**Context:** As solar penetration hits 20–30% of peak capacity in some regions, utilities face higher ramping requirements. Pairing solar with 4-hour storage addresses peak-hour demand and reduces grid stress from afternoon clouds.

**Key facts:**
- Solar + 4-hour storage can shift peak generation to evening hours, aligning with evening demand.
- Utilities save $200–400/kW vs. building peaking plants for the same capacity.
- Storage-paired solar improves interconnection studies by showing firm capacity availability.
- Five states have explicit procurement mandates for storage + renewable pairs; more are expected.

**Audience angles:**
- *Utility planner:* Storage solves a real grid planning problem (ramping, peak shifting).
- *Renewable developer:* Storage improves project economics through capacity payments and peak-hour arbitrage.
- *Policy analyst:* This reflects market-driven procurement, not subsidy-driven — shows storage economics improving.

**Risks:**
- Don't claim storage "solves" renewable intermittency; it addresses specific peak-shifting use cases.
- Duration matters: 4-hour is different from 1-hour or 8-hour; be specific.
- Avoid vague "clean energy" framing — lead with the grid problem and economic case.
```

## Source material

Consult:
- `brand/audience.md` — understand each ICP's priorities
- `brand/voice.md` — tone is technical-credible, plain-English
- `brand/content-pillars.md` — confirm the topic fits the Sustainability pillar
- Industry sources: NREL reports, FERC filings, utility RFP summaries, trade press (Energy Storage Association, GridServe, Energy News Network, etc.)

## Notes

- This skill does NOT write the LinkedIn post yet — that's the writing skill's job.
- The research brief is structured prose for a human or downstream skill to read; it's not the post draft.
- If a topic lacks sufficient public information, flag it in the frontmatter: `research_status: blocked` and note the reason in a comment so the next session knows not to rework it.
