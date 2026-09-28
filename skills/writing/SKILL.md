# Writing Skill

## Purpose

Take a researched topic (in `content/drafts/`) with a research brief and draft a LinkedIn post in Ampfield Energy's voice.

## Input

- Topic file: `content/drafts/NNN-slug.md` with `stage: draft` and a populated `research_brief` section
- Frontmatter fields: `topic`, `subtopic`, `stage`, `researched_at`
- Body: `research_brief` section containing structured research notes

## Process

1. **Read the research brief.** Extract context, key facts, audience angles, and risk notes.
2. **Write the post.** Compose a LinkedIn post that:
   - Opens with a concrete detail (a specific number, mechanism, or real-world consequence)
   - Builds on the research facts with specificity (not marketing language)
   - Addresses at least one audience angle: what's in it for the utility planner, renewable developer, or policy analyst reading this
   - Closes with a single clear takeaway or call to action
   - Follows the brand voice: technical-credible, plain-English, no jargon stacking, no hype
3. **Post structure.** Use this template:
   - **Hook** (1–2 sentences): lead with the concrete detail
   - **Body** (2–4 short paragraphs): explain why it matters, what's changing, what the audience should know
   - **Close** (1 sentence): the takeaway or call to action
   - **Total length:** 200–400 words (LinkedIn-native post, not truncated with a link to an external article)
4. **Add the draft to the file.** Create a `post_draft` section in the file and paste the post copy there.
5. **Update frontmatter.** Set `stage: draft` and `written_at: YYYY-MM-DD`, `ready_for_edit: true`.

## Example output

```markdown
---
topic: Why Utilities Pair Storage with Solar Now
subtopic: Grid-scale storage drivers
created_at: 2026-09-28
stage: draft
researched_at: 2026-09-28
written_at: 2026-09-28
ready_for_edit: true
---

## research_brief

[research notes here, as populated by the research skill]

## post_draft

Most utilities now pair solar installations with 4-hour lithium iron phosphate storage. Not because it's trendy, but because it's cheaper than building a peaking plant.

Here's why: Solar + storage shifts peak generation to evening hours, when grid demand is still high. A 100 MW solar array alone drops output to near-zero by 6 PM. The same array with 400 MWh of 4-hour storage keeps the plant producing through peak evening load. That firm capacity costs utilities $200–400/kW to deploy—peakers cost $500–800/kW for the same job.

The math is getting tighter as battery costs fall. We're seeing utilities in California, Texas, Arizona, and now the Carolinas explicitly request storage-paired solar in their procurement. Five states have mandates. More are coming.

For renewable developers, this changes project economics. Storage unlocks ancillary revenue: frequency regulation pays $2–5/kW/year, capacity payments add another $5–15/kW/year depending on the region. A 100 MW solar + 400 MWh storage project now captures revenue across arbitrage, peak shifting, and grid services—not just energy sales.

This isn't speculation. It's how utilities are solving real ramping and peak-hour problems.

Is your team evaluating storage pairing for a renewable project? What constraints are you running into?
```

## Brand voice checklist

- [ ] Opens with a specific number or mechanism, not a scene
- [ ] Technical details are accurate (battery chemistry, durations, economics)
- [ ] "We" only when describing Ampfield's own work; third person for industry/competitors
- [ ] No exclamation points, no "game-changing," no vague sustainability language
- [ ] Short paragraphs; one idea per paragraph
- [ ] Sentence case headers (if any)
- [ ] Specific product names: "4-hour lithium iron phosphate storage," not "next-gen sustainable energy solutions"

## Notes

- This skill does NOT edit for tone or tighten language — that's the editing skill's job.
- The post should be complete and coherent on its own; the editing skill will refine, not rescue.
- If the research brief lacks enough material to draft a credible post, flag it: `writing_status: blocked` and note what's missing so the research skill can revisit.
