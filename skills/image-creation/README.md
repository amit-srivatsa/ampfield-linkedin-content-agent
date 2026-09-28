# Image Creation Skill — Ampfield Energy

Generate LinkedIn post visuals for Ampfield Energy that are **modern, energetic, playful, and optimistic** by combining real urban photography with vibrant illustrated overlays.

## Files in This Skill

### Core Files
- **`system-prompt.md`** — Full system prompt for the visual direction. Copy this into image generation tools or AI requests to ensure consistency.
- **`.agents-skill.md`** — Condensed skill reference (for loading into Claude Code as a skill).

### Reference & Guidance  
- **`STYLE-ANALYSIS.md`** — Deep dive into the visual language. Read this to understand the "why" behind each design choice. Includes:
  - How the hybrid real + illustrated style works
  - Color palette and saturation rules
  - Character design principles
  - Composition and layering
  - How to regenerate the style for new topics

- **`TOPIC-GUIDE.md`** — Practical quick reference for specific Ampfield topics. Includes:
  - 6 Ampfield sustainability topics with tailored visual concepts
  - Pre-built image prompt templates for each topic
  - Tips, pitfalls, and a workflow for generating new images

- **`sample-images/`** — The 10 reference images you provided. Study these to internalize the visual direction.

- **`README.md`** — This file.

---

## How to Use This Skill

### Scenario 1: Generate a Quick Image for a Post

1. **Identify your topic** from `TOPIC-GUIDE.md` (e.g., "Grid Balancing," "Renewable Integration")
2. **Adapt the suggested prompt** to your specific post angle
3. **Pass the prompt** to your image generation tool (Midjourney, DALL-E, Claude's image generation, etc.)
4. **Refine if needed** using the style principles in `STYLE-ANALYSIS.md`

### Scenario 2: Train a New Generator or Brief a Designer

1. **Share `system-prompt.md`** with the generator (AI or human)
2. **Provide context** from `STYLE-ANALYSIS.md` if they ask "why" questions
3. **Use `TOPIC-GUIDE.md`** to show topic-specific examples

### Scenario 3: Create a Custom Topic Image

1. **Read the "How to Regenerate This Style" section** in `STYLE-ANALYSIS.md`
2. **Choose your urban backdrop** (real place that fits your message)
3. **Design your character** (pose, outfit, emotion)
4. **Select 5–8 decorative elements** from the style palette
5. **Write your image prompt** using the template format
6. **Generate and refine** iteratively

### Scenario 4: Integrate into a Skill or Workflow

- Use **`system-prompt.md`** as the actual system prompt in your Claude session or tool
- Include **`TOPIC-GUIDE.md`** in your context so the AI/agent can suggest images based on post topic
- Refer to **`STYLE-ANALYSIS.md`** for validation (does the generated image match the style?)

---

## Key Visual Principles

**Remember these 5 things:**

1. **Real photo base + illustrated overlay** — Never seamlessly blended; keep them as distinct layers
2. **Bold, saturated colors** — Bright magenta, electric lime, vibrant blue, sunny yellow. Never pastel or muted.
3. **Diverse, expressive human character** — Prominent, dynamic pose, relatable, emotionally engaging
4. **5–8 playful decorative elements** — Plants, geometric shapes, whimsical creatures, flow lines
5. **Optimistic, energetic tone** — Fun, forward-looking, celebrating the future. Never corporate or technical.

---

## Quick Reference Checklist

When generating an image, verify:

- [ ] Real urban photo base visible?
- [ ] Illustrated elements layered on top with white outlines?
- [ ] Diverse human character centered & prominent?
- [ ] Character in dynamic, confident pose?
- [ ] Hot pink + electric lime + vibrant blue + sunny yellow all present?
- [ ] 5–8 decorative elements well-distributed?
- [ ] Playful, not corporate feel?
- [ ] Tone optimistic and energetic?
- [ ] No overly technical or literal tech imagery?

---

## Common Workflows

### For the LinkedIn Content Agent

The image creation skill is **step 4** in the content pipeline:
1. **Research** the topic (skill: research/)
2. **Write** the post (skill: writing/)
3. **Edit** the draft (skill: editing/)
4. **Create visual** (skill: image-creation/) ← You are here
5. **Human review & publish** (manual)

When a post draft is ready, this skill should:
- Extract the post's core theme
- Match it to a topic in `TOPIC-GUIDE.md`
- Generate a visual prompt
- Create the image
- Return both the post and the image for human review

### For Manual Image Creation

1. Open `TOPIC-GUIDE.md`
2. Find your topic
3. Copy the example prompt
4. Paste into your image generation tool (Midjourney, DALL-E, etc.)
5. Adjust any details specific to your post
6. Generate
7. Check against the style checklist above

### For Custom/Unusual Topics

1. Read `STYLE-ANALYSIS.md` — "How to Regenerate This Style for New Topics"
2. Follow the 6-step process
3. Write your prompt
4. Generate & refine

---

## Tips for Best Results

**Color Saturation**: If the generated image feels muted or pastel, add to your prompt: "Bold, saturated, vibrant colors—bright magenta, electric lime, sky blue, sunny yellow. No muted or pastel tones."

**Character Presence**: If the character feels small or passive, add: "Central human character should be prominent, sized 30–50% of image height, in a dynamic, energetic pose that draws the eye."

**Urban Authenticity**: If the real photo feels too abstract or unreal, add: "Real urban photograph as the base—recognizable landmark or city street. Slightly desaturated or color-graded for cohesion, but clearly photographic."

**Illustration Separation**: If overlays blend too much: "Bold white outlines on all illustration elements. Clear visual separation between real photo and illustrated layer. Intentionally artificial-looking illustration."

**Playfulness**: If the tone feels too serious: "Playful, youthful, joyful. Whimsical creatures, flowing ribbons, hand-drawn marks. Celebrate rather than educate. Optimistic and energetic."

---

## Sample Prompts

### Grid Balancing (copied from TOPIC-GUIDE)

> Urban city at dawn with modern skyline. Diverse professional in lime-green jacket with arms outstretched in a balanced, powerful stance. Surrounding elements: flowing electric-blue ribbons, simple star-burst shapes, oscillating wave lines in white and green, a stylized balance-scale decoration. Motion lines suggest energy flow. Bright, optimistic, controlled energy. Modern illustration overlay on cityscape.

### Renewable Integration (copied from TOPIC-GUIDE)

> Modern city rooftop with bright sky and distant wind turbines. Young figure in bright yellow outfit, arm raised upward in an expansive, hopeful pose, smiling toward the horizon. Surrounding elements: large sun with radiating lines, flowing wind-like ribbons in sky blue, vibrant lime-green stylized leaves and flowers, simple geometric fan-blade shapes, sparkle marks. Plants and tech symbols woven together. Bright, forward-looking, energized mood.

---

## Attribution & Notes

**Visual Direction**: Based on analysis of 10 reference images provided. This skill captures the consistent aesthetic across diverse urban locations (Toronto, San Francisco, Paris, Istanbul, London, etc.).

**Tone**: Designed for Ampfield Energy—a forward-thinking brand in grid-scale battery storage and clean energy. The visual style positions sustainability as vibrant, accessible, and worth celebrating.

**Flexibility**: While the style is consistent, each image should be unique. Use `TOPIC-GUIDE.md` as a starting point, not a template. Adapt and customize for your specific post angle.

---

## Questions?

- **"What colors should I use?"** → See Color Palette section in `STYLE-ANALYSIS.md`
- **"How do I generate this style with [tool]?"** → Check the prompt format in `system-prompt.md` and adapt for your tool's syntax
- **"What if my topic isn't in TOPIC-GUIDE.md?"** → Follow the 6-step process in `STYLE-ANALYSIS.md` under "How to Regenerate This Style"
- **"Why does my image look corporate?"** → Check the "Avoid" section in `system-prompt.md` and the "Common Pitfalls" section in `TOPIC-GUIDE.md`
- **"Should I change the colors for different campaigns?"** → No. The palette is core to the brand identity. Use the same colors across all Ampfield visuals for consistency.

---

## Next Steps

1. **Study the sample images** in `sample-images/` to internalize the aesthetic
2. **Read `STYLE-ANALYSIS.md`** to understand the "why"
3. **Pick a topic from `TOPIC-GUIDE.md`** and generate your first image
4. **Iterate** — refine using the checklist and tips above
5. **Build a library** of 3–5 images across different topics for future posts

Good luck! 🎨

---

**Skill Created**: 2026-09-28  
**Visual Reference Base**: 10 diverse urban illustration hybrids  
**Color Palette**: Magenta, Lime Green, Sky Blue, Yellow, Purple, Navy, White  
**Tone**: Optimistic, Energetic, Playful, Modern, Accessible
