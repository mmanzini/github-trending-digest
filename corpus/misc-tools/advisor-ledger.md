# advisor-ledger

A permanent mirror of a crowdsourced "Academic Advisor Red Flags" document that snapshots every few minutes, preserves deletion history, and uses a local LLM to review changes for sensitive content.

- **Repo:** [the-hidden-fish/advisor-ledger](https://github.com/the-hidden-fish/advisor-ledger)
- **Stars:** ~1,037 (2026-04-24, 5 days after launch)
- **Created:** 2026-04-19
- **Language:** Python
- **Topics:** none

## Why It Matters
- Illustrates a "LLM as change guardian" pattern: automated snapshots + AI content review to catch moderation or censorship of a sensitive public document.
- Community accountability tooling — stars signal there is pent-up demand for tools that preserve crowdsourced institutional red-flag data.
- Lightweight architecture (local LLM + snapshot loop) is easy to replicate for other living-document monitoring use cases.

## Key Takeaways
- Pattern: high-frequency snapshot → LLM diff review → permanent history. Applicable to any contested or at-risk public document.
- "Preservation over curation" ethos — the tool trusts the crowd more than any single moderator.
- Local LLM for change review keeps sensitive content off third-party APIs.
- Trending without any declared topic tags — word-of-mouth driven.

## Related
- [[hop]]
