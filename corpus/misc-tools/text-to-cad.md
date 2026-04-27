# Text-to-CAD

**Repo:** [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad)
**Language:** JavaScript | **First seen:** 2026-04-27 | **Stars (7-day peak):** ~738

Open-source harness for generating CAD models using AI agents. Text prompt → 3D CAD model, running in the browser via WebAssembly.

## Architecture
- Browser-based: WASM runtime, no desktop CAD software required
- Agent-harness approach: the AI agent orchestrates CAD geometry construction, not a direct model-to-mesh conversion
- JavaScript/TypeScript stack, targeting web deployment

## Pattern: Domain-Specific Agentic Coding
Text-to-CAD applies the same "specialized agentic pipeline" pattern as [[opengame]] (text → game) but for 3D engineering geometry. Both repos arrived in the same week, suggesting the "text prompt → domain artifact via agent" pattern is broadening beyond web apps and code.

The WASM-in-browser constraint is notable: it means the CAD kernel runs locally without requiring expensive native tooling, lowering the barrier to experimentation significantly.

## Key Takeaways
- First CAD-specific agent harness in this corpus; a new vertical for agentic coding
- Browser + WASM architecture makes it accessible without CAD software installation
- The agent-harness framing (orchestrate geometry construction) is more flexible than direct model weights for 3D generation
- Compare with [[lingbot-map]] for a different approach to 3D (feed-forward foundation model reconstruction vs. agent-driven CAD generation)
- See also: [[opengame]] for the domain-specific agentic pipeline pattern applied to games
