# Create Post Workflow

## Pipeline

1. Pick a topic file from `content/ideas/` (or write a new one — see naming below).
2. Move it to `content/drafts/` the moment research starts on it.
3. Run `research` → `writing` → `editing` → `image-creation` skills against it (skills not yet built — see `skills/`).
4. Score against a quality bar before calling it done (rubric to be defined once `skills/editing/` exists).
5. Human review and approval — required before anything is posted.
6. Once approved and manually posted to LinkedIn, move the topic file to `content/published/`.

No step in this pipeline posts to LinkedIn automatically. This project stops at a reviewable draft.

## Naming convention

- Every topic gets one file: `NNN-slug.md`.
- `NNN` is a zero-padded 3-digit sequence, assigned in creation order. Never reuse a number, never renumber — a topic that stalls in `ideas/` still keeps its number.
- `slug` is the topic in lowercase kebab-case.
- The file moves between `content/ideas/` → `content/drafts/` → `content/published/` as it progresses — it isn't copied, and it isn't renamed at each stage. Before creating a new topic file, check all three folders for an existing one with that slug.
- Each topic file accumulates its own research notes, post copy, and image prompt inline as the pipeline runs, since there's a single file per topic rather than a per-topic folder.
