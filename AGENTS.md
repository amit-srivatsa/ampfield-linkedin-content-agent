# AGENTS.md — LinkedIn Content Agent (Ampfield Energy / Sustainability)

## Goal

Turn one Sustainability subtopic into a researched LinkedIn post and matching visual for **Ampfield Energy** — a fictional grid-scale battery storage and grid-balancing company selling to utilities and renewable-energy developers. `[NEEDS INPUT]` if this ever stops being a demo persona and needs a real company behind it.

This file is an index, not a reference manual. Real content lives in the files below.

## Scope

- Single content pillar: Sustainability (grid-scale energy storage & balancing). No other pillars.
- File-driven skill pipeline: research → write → edit → create visual → human review. No Flask app, no LinkedIn API integration, no auto-posting.
- Human approval before publishing. This project stops at a reviewable draft.

## Inputs

- Topic (drawn from `content/ideas/`)
- Audience (from `brand/audience.md`)
- Point of view / voice (from `brand/voice.md`)
- Desired action

## Outputs

- A drafted post + image prompt inside `content/drafts/`
- A published record inside `content/published/` once approved and manually posted

## Where things live

- `brand/voice.md` — tone, style, personality for Ampfield Energy's LinkedIn presence.
- `brand/audience.md` — ICPs: who this content is written for and what persuades them.
- `brand/content-pillars.md` — the Sustainability pillar and its subtopics (green energy, storage solutions, grid balancing, etc.).
- `workflows/create-post.md` — the pipeline steps and the `ideas/ → drafts/ → published/` lifecycle, including the topic-file naming convention.
- `memory/agent-memory.md` — running decision log. Append an entry each session.
- `memory/sessions/` — one handoff file per session (`YYYY-MM-DD.md`, from `memory/sessions/TEMPLATE.md`). Read the most recent one at the start of a session; write a new one at the end.
- `content/ideas/`, `content/drafts/`, `content/published/` — topic files at each pipeline stage. See `workflows/create-post.md`.
- `skills/research/`, `skills/writing/`, `skills/editing/`, `skills/image-creation/` — the four pipeline skills. Not yet built.

## Session protocol

- **Start:** read `memory/agent-memory.md` and the most recent file in `memory/sessions/` before doing new work.
- **End:** write `memory/sessions/YYYY-MM-DD.md` from the template, and append one entry to `memory/agent-memory.md` summarizing what changed and why.

## Rules

- The agent owns the outcome. Each skill owns one part of the work.
- Label facts, inference, and opinion separately.
- Do not silently strengthen claims.
- Human approval before publishing — no auto-posting to LinkedIn.
