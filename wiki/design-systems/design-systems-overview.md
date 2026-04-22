# Design Systems for AI — Overview

A small but coherent trending category: tooling and conventions that let coding agents produce on-brand, design-system-aware UI. The pattern that emerged in the 2026-04 trending data has three layers:

1. **A markdown convention** — `DESIGN.md`, popularised by [[awesome-design-md]]. Hand-curated brand snapshots that any file-reading agent can consume.
2. **Automated extraction** — [[design-extract]] pulls the same kind of token set automatically from any live website, emitting DTCG tokens, MCP server, and multi-platform code (SwiftUI, Compose, Flutter, Tailwind v4, shadcn/ui).
3. **Expressive output formats** — [[html-ppt-skill]], [[fireworks-tech-graph]], [[diagram-design]], [[huashu-design]], and [[kami]] live in the [[agent-skills-overview|skills folder]] but belong here too: they're how design-aware agents *render* output.
4. **Productised wrappers** — [[open-codesign]] packages the workflow as a multi-model desktop app; [[awesome-claude-design]] is VoltAgent's Claude-Code-branded cut of the DESIGN.md collection.

A distinct Claude Code design micro-ecosystem crystallised during 2026-04 — four of the top-10 trending 2026-04-22 repos were Claude Code design extensions ([[huashu-design]], [[diagram-design]], [[awesome-claude-design]], [[open-codesign]]). The cluster's shared stance: HTML/SVG output, no Mermaid, editorial taste over framework conventions.

## Why It Matters
- "Vibe-design" / "vibe-coding" are the trending vocabulary — design-by-conversation is now a recognised mode.
- Markdown conventions can be **platforms**: any agent that reads files participates without integration code.
- Multi-platform emitters (one extraction → SwiftUI, Compose, Flutter, web) signal that design tokens are becoming a portable interchange format, not just a web concern.

## Key Takeaways
- Hand-curated (`DESIGN.md`) and automated (extract from URL) approaches are complementary, not competitive.
- DTCG tokens are the trending interchange format.
- WCAG-aware extraction (see [[design-extract]]) means accessibility is inheriting the same agent UX.
- Pairs with [[agent-skills-overview]]: visual-output skills (presentations, diagrams) consume design-system inputs.

## Related
- [[awesome-design-md]]
- [[design-extract]]
- [[agent-skills-overview]]
- [[html-ppt-skill]]
- [[fireworks-tech-graph]]
