# Editing Skill

## Purpose

Refine a drafted LinkedIn post (in `content/drafts/`) to ensure it matches brand voice, meets quality standards, and is ready for human review.

## Input

- Topic file: `content/drafts/NNN-slug.md` with `ready_for_edit: true` and a populated `post_draft` section
- Frontmatter fields: `topic`, `subtopic`, `stage`, `researched_at`, `written_at`
- Body: `post_draft` section containing the draft post copy

## Process

1. **Read the post draft.** Understand the core message and audience.
2. **Edit for brand voice.** Check against the voice guidelines:
   - Is it technical-credible and plain-English? (Not marketing-speak, not overly simplified)
   - Does it lead with a concrete detail, not a hook?
   - Are there vague words or promotional language? ("game-changing," "next-gen," "sustainable future," etc.) — remove them
   - Are there unnecessary superlatives or unearned confidence claims? — rein them in
   - Do paragraphs stay short and stick to one idea each?
   - Is "we" used only for Ampfield's own work, third person for the industry?
   - Are technical details specific? (e.g., "4-hour lithium iron phosphate," not "advanced battery technology")
3. **Edit for clarity.** Check:
   - Does each sentence say one clear thing?
   - Are there jargon terms that need plain-English explanation?
   - Does the post logically flow from hook to close?
   - Is the call-to-action (if present) clear and specific?
4. **Fact-check.** Verify:
   - Numbers and ranges are accurate and attributed (or labeled as illustrative)
   - Technical descriptions of storage, grid balancing, policy are correct
   - If you can't verify a claim, flag it with `[VERIFY]` in a comment so the writing or research skill can confirm
5. **Update the post.** Replace the `post_draft` section with the refined version.
6. **Update frontmatter.** Set `edited_at: YYYY-MM-DD`, `ready_for_image: true`, and optionally note any flags or edits in a `editor_notes` field.
7. **Mark as ready.** Once editing is complete, update `stage: draft` to stay as-is (it doesn't move to a new folder until image-creation or approval).

## Editing checklist

- [ ] Removed vague adjectives ("game-changing," "revolutionary," "next-gen," "sustainable," "clean," "green") unless they're technical terms
- [ ] Replaced buzzwords with specifics: "advanced storage" → "4-hour lithium iron phosphate," "solutions" → actual mechanism
- [ ] Confirmed technical claims are accurate (battery chemistry, durations, policy status, costs within reasonable ranges)
- [ ] Rewrote overstated claims to be credible and qualified: "storage solves X" → "storage addresses X in these specific cases"
- [ ] Paragraphs are short; each paragraph is one idea
- [ ] Sentence case only; no em dashes in public copy
- [ ] No exclamation points (unless part of a direct quote)
- [ ] Call-to-action (if present) is specific and invites conversation, not a sales pitch
- [ ] Post reads as engineer-founder voice: precise, a little dry, quietly opinionated

## Example edits

**Before:**
> "We're excited to share how battery storage is revolutionizing the energy industry and transforming the way utilities manage grid balancing. Our next-generation sustainable energy solutions..."

**After:**
> "Most utilities now pair solar installations with 4-hour lithium iron phosphate storage. Not because it's trendy, but because it's cheaper than building a peaking plant."

---

**Before:**
> "Storage is game-changing for renewable projects because it unlocks amazing revenue opportunities across multiple streams."

**After:**
> "For renewable developers, storage pairing changes project economics. Storage unlocks ancillary revenue: frequency regulation pays $2–5/kW/year, capacity payments add another $5–15/kW/year depending on the region."

## Notes

- This skill's job is to refine, not rewrite. If a post needs fundamental restructuring, send it back to the writing skill with specific feedback.
- If you find claims that can't be verified, flag them for the writer or researcher to revisit — don't silently weaken or remove them.
- The goal is a polished draft that's ready for human review and approval before posting.
