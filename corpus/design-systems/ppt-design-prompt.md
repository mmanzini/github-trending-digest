# PPT Design Prompt

**Repo:** [Russell-cell/PPT-Design-Prompt](https://github.com/Russell-cell/PPT-Design-Prompt)
**Language:** Python | **First seen:** 2026-04-27 | **Stars (7-day peak):** ~759

Converts brand design guidelines into presentation-image prompts optimized for AI image generation models and design agents. Bridges the gap between a brand's design system and the prompt format needed by image models.

## What It Does
- Takes brand design guidelines (colors, typography, spacing, tone) as input
- Outputs structured prompts calibrated for AI image generation (e.g., GPT-Image-2)
- Target output: slides and presentation visuals that are on-brand, not generic

## Positioning in the Design-Systems Cluster
PPT-Design-Prompt is a bridge tool: it connects the "extract / define design system" layer (see [[design-extract]], [[awesome-design-md]]) to the "generate images from prompts" layer (see [[awesome-gpt-image-2-prompts]], [[awesome-gpt-image-2]]). Most design-system tools target code generation (CSS, Tailwind); this one targets image generation specifically for presentations.

Companion tools from the same April 2026 wave:
- [[guizang-ppt-skill]] — prompts → full HTML deck (no image model involved)
- [[kami]] — document design system (typography, layout for print-quality output)
- [[huashu-design]] — HTML-native prototypes with MP4 export

## Key Takeaways
- Brand guidelines → structured image prompts is an underserved pipeline step
- Positions design systems as the upstream input for image generation, not just for code agents
- Small star count (759) suggests it's early but the pattern (structured prompts from design systems) is sound
- See also: [[design-systems-overview]]
