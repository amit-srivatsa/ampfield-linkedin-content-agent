# Agent Memory

Running log of decisions made in this project, newest first. Append only — don't rewrite or delete past entries. If a past decision is superseded, add a new entry saying so.

---

## 2026-09-28

- **Scaffold populated for the Sustainability niche.** `brand/`, `memory/`, `workflows/create-post.md`, and starter `content/ideas/` files were filled in. `skills/` was left untouched (empty) per instruction — no `SKILL.md` files written yet.
- **Architecture changed from Flask to a file-driven skill pipeline.** `AGENTS.md` previously described a Flask backend + LinkedIn API integration, which didn't match the existing `skills/{research,writing,editing,image-creation}/` folders. Rewrote it to match the proven pattern from `workshops/03 - Claude in terminal - 25-08-26/session-25-live/`: topic → research → write → edit → create visual → human-reviewed draft. No Flask, no LinkedIn API, no auto-posting.
- **Persona chosen: Ampfield Energy**, a fictional grid-scale battery storage and grid-balancing company — a demo persona, same role session 03's sheet-metal manufacturer played. `[NEEDS INPUT]` if this ever needs to become a real company.
- **Pillar scope: Sustainability only**, single niche. Subtopics: green energy generation, storage solutions, grid balancing, policy & incentives, project economics — a starting list, expandable.
- **Content lifecycle: one file per topic, moved between `content/ideas/` → `drafts/` → `published/`** (not copied), rather than session 03's per-topic-folder model — this matches the folder structure already scaffolded in this project (`content/{ideas,drafts,published}/` as separate top-level dirs, not `posts/NNN-slug/`).
- **Open:** the four skills (`research`, `writing`, `editing`, `image-creation`) still need `SKILL.md` files before this pipeline can actually run.

---

## Current session (continuing 2026-09-28)

- **Three pipeline skills built:** `skills/research/SKILL.md`, `skills/writing/SKILL.md`, `skills/editing/SKILL.md`. Image-creation skill deferred per session scope.
- **Research skill:** reads topic from `content/ideas/`, produces structured research brief (context, key facts, audience angles, risks), moves file to `content/drafts/`.
- **Writing skill:** reads research brief from `content/drafts/`, drafts a LinkedIn post in Ampfield voice (technical-credible, specific, 200–400 words), marks file `ready_for_edit: true`.
- **Editing skill:** refines post for brand voice consistency (removes vague adjectives, checks technical accuracy, tightens paragraphs), marks file `ready_for_image: true`.
- **Pipeline ready for proof-of-concept:** next step is to execute one topic end-to-end through all three skills. Recommend starting with topic `001-why-utilities-pairing-storage-with-solar-now.md` from `content/ideas/`.
