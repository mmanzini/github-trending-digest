# mempalace

Open-source AI memory system claiming the **best benchmarks** in its category. MCP-compatible, built on ChromaDB, designed for persistent agent memory across LLM sessions. Free and self-hostable.

- **Repo:** [MemPalace/mempalace](https://github.com/MemPalace/mempalace)
- **Stars:** ~49.1K (2026-04-23) — hit ~46K in 11 days post-launch
- **Created:** 2026-04-05
- **Language:** Python
- **Topics:** ai, chromadb, llm, mcp, memory, python

## Why It Matters
- Persistent memory is the community's **sharpest current pain point** for agents — the velocity here (46K stars in 11 days) signals it.
- MCP-native = drops into Claude Code, Cursor, Windsurf, and any other MCP-aware harness without integration code.
- ChromaDB underneath means standard vector-store ops (no exotic infra), so the differentiation is in retrieval/eviction strategy.

## Key Takeaways
- "Best benchmarked" is a strong claim — verify the methodology before relying on it for a specific workload.
- Self-hostable + free = no vendor lock-in for memory state, important for serious agent products.
- Pairs naturally with [[browser-harness]] (persist learned helpers) and [[hermes-hudui]] (UI for memory observability).

## Related
- [[hermes-hudui]]
- [[claude-code-overview]]
- [[browser-harness]]
- [[weft]] — durable execution often pairs with durable memory state
