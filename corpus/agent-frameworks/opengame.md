# OpenGame

**Repo:** [leigest519/OpenGame](https://github.com/leigest519/OpenGame)
**Language:** TypeScript | **First seen:** 2026-04-25 | **Stars (7-day peak):** ~1,127

Open agentic coding framework for end-to-end web game creation from a single text prompt. Uses a specialized GameCoder-27B model and autonomous multi-agent coordination to handle scaffolding, debugging, and multi-file coordination.

## Architecture
- Prompt → full web game pipeline, not just code snippets
- **GameCoder-27B** — a dedicated fine-tuned model for game-specific code generation
- Multi-agent coordination for scaffolding, bug-fixing, and file management
- TypeScript stack, targeting browser-playable web games

## Positioning
Combines a domain-specific model fine-tune with agentic orchestration — a tighter vertical than general-purpose agents like [[browser-harness]] or [[claw-code]]. The specialized model is the key differentiator: rather than prompting a general LLM to write game code, OpenGame ships a purpose-built model.

## Key Takeaways
- Domain-specific model fine-tune + agent orchestration is a pattern likely to repeat across verticals (games → CAD → web apps)
- Contrast with [[text-to-cad]] (also appearing in this cycle) for the same pattern applied to 3D CAD
- Self-contained agentic pipeline: the agent handles the full software development lifecycle, not just code generation
- See also: [[agent-frameworks-overview]]
