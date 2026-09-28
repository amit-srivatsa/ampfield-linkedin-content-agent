# LinkedIn Content Agent — Ampfield Energy

A file-driven pipeline for creating research-backed LinkedIn posts about grid-scale battery storage and energy transition.

**Built in Claude Code.** This repository demonstrates how to use Claude as a content strategist for technical B2B LinkedIn posts—research, writing, editing, and visual generation.

---

## What's Inside

### Directory Structure

```
├── README.md                          # This file
├── AGENTS.md                          # Project operating contract
├── brand/                             # Brand positioning & voice
│   ├── voice.md                       # Tone, style, personality
│   ├── audience.md                    # ICPs and what persuades them
│   └── content-pillars.md             # Topic areas (Sustainability pillar)
├── content/
│   ├── ideas/                         # Topic ideas (001–010)
│   ├── drafts/                        # Researched, written, edited posts (ready for images)
│   └── published/                     # Final posts + images (ready for LinkedIn)
├── skills/                            # Claude skills for each pipeline stage
│   ├── research/                      # Research skill (fact-gathering, sourcing)
│   ├── writing/                       # Writing skill (post creation)
│   ├── editing/                       # Editing skill (tightening, voice polish)
│   └── image-creation/                # Image generation skills
├── workflows/                         # Pipeline documentation
│   └── create-post.md                 # Step-by-step pipeline process
└── memory/                            # Session logs and decision tracking
```

---

## The Pipeline: Research → Write → Edit → Publish

Each post goes through four stages:

### 1. **Research**
- Read the idea topic and audience
- Gather facts, data, timelines, cost ranges
- Identify the angle: what's the insight worth 3 minutes of a busy executive's time?
- Document findings in research brief

### 2. **Write**
- 280–300 word LinkedIn post
- Technical-credible tone; engineer-founder voice
- Opens with concrete detail, not abstraction
- Addresses audience pain point or decision

### 3. **Edit**
- Remove buzzwords ("game-changing," "future," "transition")
- Tighten for punchiness
- Verify all claims with specific data
- Maintain voice consistency

### 4. **Publish**
- Generate matching visual (two approaches available: bold & vibrant, or editorial & sophisticated)
- Move post + image to `content/published/`
- Ready for manual LinkedIn posting

---

## Current Posts (Published & Ready)

| Idea | Topic | Status | Audience |
|------|-------|--------|----------|
| #1 | Why utilities are pairing storage with solar now | ✅ Draft | Developers, utility procurement |
| #2 | What 4-hour vs. 8-hour duration storage actually changes | ✅ Draft | Engineers, investors |
| #3 | Grid balancing 101 for non-engineers | ✅ Draft | Utility planners, policy analysts |
| #4 | The permitting bottleneck nobody talks about | ✅ Draft | Project developers, executives |
| #5 | Battery chemistry choices explained | ✅ Draft | Engineers, storage investors |

All posts are complete and ready for image generation and LinkedIn posting.

---

## How to Use This Repository

### Fork & Adapt for Your Company

1. **Clone or fork this repo**
   ```bash
   git clone https://github.com/amit-srivatsa/ampfield-linkedin-content-agent.git
   cd ampfield-linkedin-content-agent
   ```

2. **Update brand positioning** (if using for your company):
   - Edit `brand/voice.md` with your company's tone
   - Edit `brand/audience.md` with your ICPs
   - Edit `brand/content-pillars.md` with your topics

3. **Add new ideas**:
   - Create `content/ideas/{NN}-{topic}.md` (follow naming convention)
   - Write a 1–2 sentence idea description

4. **Run the pipeline**:
   - Use Claude Code with the skills in `skills/` directory
   - Follow `workflows/create-post.md` step-by-step
   - Output goes to `content/drafts/`

5. **Generate images**:
   - Use the image prompts in `skills/image-creation/`
   - Two visual approaches available (Claude skill: bold & vibrant; ChatGPT skill: editorial & sophisticated)
   - Save to `content/published/images/`

6. **Publish to LinkedIn**:
   - Copy post text + image
   - Post manually (no API automation)
   - Archive published items in `content/published/`

---

## Key Files for Students

### To Understand the Voice & Approach
- `brand/voice.md` — How Ampfield writes (technical-credible, no marketing speak)
- `brand/audience.md` — Who we're talking to and what they care about
- `content/drafts/001-why-utilities-pairing-storage-with-solar-now.md` — Example: solar economics post

### To Build Your Own Posts
- `workflows/create-post.md` — Step-by-step pipeline
- `skills/research/` — How to gather facts and verify claims
- `skills/writing/` — Post structure and tone guidelines
- `skills/editing/` — How to tighten language and remove jargon

### To Generate Visuals
- `skills/image-creation/system-prompt.md` — Visual DNA and color palette
- `skills/image-creation/STYLE-ANALYSIS.md` — Deep dive into the visual language
- `skills/image-creation/TOPIC-GUIDE.md` — Pre-built visual concepts by topic

---

## Brand Voice (TL;DR)

- **Tone:** Technical-credible, engineer-founder perspective
- **Approach:** Concrete details first; abstractions never
- **Audience:** Utility planners, renewable developers, policy analysts (not consumers)
- **Data:** Always include specific numbers (costs, timelines, percentages)
- **Avoid:** Buzzwords like "game-changing," "clean energy future," "transition"

Example opening (✅ good):
> "Solar keeps getting cheaper. That's created a new problem for utilities: too much solar at noon."

Example opening (❌ avoid):
> "The renewable energy transition is accelerating. Battery storage is now playing a critical role in enabling a cleaner future."

---

## Image Generation

Two validated visual approaches:

### 1. Bold & Vibrant (Claude Skill)
- Modern urban photography + vibrant illustrated overlay
- Energetic, playful-professional, stands out in feed
- Best for: Announcements, features, younger demographics
- Example: Grid operator conducting energy with electric-blue ribbons and hot pink accents

### 2. Editorial & Sophisticated (ChatGPT Skill)
- Hand-drawn editorial illustration on real backdrop
- Understated elegance, professional
- Best for: Thought leadership, strategic topics
- Example: Professional on rooftop gesturing balance between sunset solar and evening demand

---

## For Teachers / Workshop Facilitators

This repo is designed as a **teaching framework** for Claude Code workflows:

1. **Demonstrates multi-step pipelines** — students see how to break complex tasks (content creation) into discrete skills
2. **Shows voice consistency** — all posts maintain the same tone despite different topics
3. **Teaches data literacy** — posts are fact-checked with specific numbers, not marketing claims
4. **Is forkable & adaptable** — students can use this template for their own companies/industries

### Workshop Exercise Ideas

- **Fork this repo** and create posts for a different company (clean energy, fintech, etc.)
- **Change the voice** — rewrite a post as if it's from a marketing team (vs. engineer-founder)
- **Add a new topic** — research and draft a post on a topic not covered
- **Experiment with images** — generate visuals using different prompts and compare

---

## Next Steps

1. **Review the current posts** in `content/drafts/` to understand the quality bar
2. **Fork or clone** this repo
3. **Adapt brand positioning** for your use case
4. **Create new ideas** and run through the pipeline
5. **Generate images** and publish when ready

---

## Questions?

- See `AGENTS.md` for the full operating contract
- See `workflows/create-post.md` for detailed pipeline steps
- Review past sessions in `memory/` to understand decision-making

---

**Built with Claude Code | Ampfield Energy (fictional company for demo)**
