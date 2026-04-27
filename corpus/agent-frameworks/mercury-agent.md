# Mercury Agent

**Repo:** [cosmicstack-labs/mercury-agent](https://github.com/cosmicstack-labs/mercury-agent)
**Language:** TypeScript | **First seen:** 2026-04-26 | **Stars (7-day peak):** ~1,173

A "soul-driven" AI agent framework designed for persistent, multi-channel deployment. Runs 24/7 as a background process reachable via CLI or Telegram.

## Key Design Choices
- **Permission-hardened tools** — tools are gated with explicit capability grants rather than open access
- **Token budgets** — enforced at the framework level, not left to the calling code
- **Multi-channel access** — same agent serves CLI and Telegram simultaneously
- **Persistent runtime** — designed to run continuously, not as a one-shot script

## Positioning in the Landscape
Mercury-agent sits between a lightweight script harness (like [[claw-code]]) and a full orchestration framework. The "soul-driven" framing suggests a focus on consistent agent identity/behavior across sessions — adjacent to the persistent memory work in [[mempalace]] and [[openchronicle]], but at the harness layer rather than the storage layer.

## Key Takeaways
- Permission-hardened tools and token budgets at the framework level address two of the most common production pain points for deployed agents
- Telegram channel support makes it a user-facing deployment target, not just a developer tool
- 24/7 persistent runtime contrasts with the ephemeral session model of most coding agents
- See also: [[agent-frameworks-overview]] for broader harness design patterns
