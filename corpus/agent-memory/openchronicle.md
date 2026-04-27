# OpenChronicle

**Repo:** [Einsia/OpenChronicle](https://github.com/Einsia/OpenChronicle)
**Language:** Python | **First seen:** 2026-04-25 | **Stars (7-day peak):** ~1,486

Local-first, open-source AI memory system for macOS. Captures structured context from a user's live environment — open applications, active documents, ongoing work — and makes it queryable by any tool-capable LLM agent via MCP.

## How It Works
- Uses macOS **accessibility trees** to extract structured context from foreground apps (e.g., what file is open, what text is selected, what browser tab is active)
- Captures screenshots alongside structured data
- Stores memories as **Markdown files** (human-readable) backed by SQLite for querying
- Exposes all captured context through an **MCP interface**, so any agent that supports MCP (Claude Code, Claude Desktop, custom harnesses) can query it

## Compatibility
- Works with OpenAI, Anthropic, and local models
- MCP server surface means it slots into existing agent workflows without code changes

## Differentiation from [[mempalace]]
| Feature | OpenChronicle | MemPalace |
|---|---|---|
| Input source | macOS accessibility tree + screenshots | Explicit memories you provide |
| Storage format | Markdown + SQLite | ChromaDB (vector DB) |
| Platform | macOS only | Cross-platform |
| MCP support | Yes | Yes |
| Cloud dependency | None | None |

## Key Takeaways
- Captures *implicit* context (what you're doing) rather than relying on explicit memory writes — fills a gap that closed-source products own today
- Accessibility-tree approach gives structured, semantic context that raw screenshot approaches can't match
- Local-first and open-source: no cloud lock-in, data never leaves the machine
- Slower to break out than [[mempalace]] (1,486 vs ~50K stars) but solves a distinct problem
- The pairing of [[openchronicle]] + [[mempalace]] covers both implicit capture and explicit long-term storage
