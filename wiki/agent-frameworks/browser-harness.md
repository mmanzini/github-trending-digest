# browser-harness

A self-healing browser harness that lets LLMs complete arbitrary web tasks. When a needed capability is missing, **the agent writes the helper function itself mid-task** — no framework overhead, ~592 lines total.

- **Repo:** [browser-use/browser-harness](https://github.com/browser-use/browser-harness)
- **Stars:** ~4.6K (2026-04-22, 5 days after launch — up from ~2.6K on 2026-04-20)
- **Created:** 2026-04-17
- **Language:** Python

## Why It Matters
- **Novel architecture pattern**: instead of pre-specifying every browser action, the LLM authors missing helpers on demand. Frees the framework from chasing every site quirk.
- Tiny codebase (~592 lines) — readable in one sitting, hackable, no opinionated API surface.
- Strong content angle for autonomous-agent explainers: "self-healing" is the headline.

## How It Works (At a Glance)
- Agent attempts a task; if no existing helper fits, it writes one in-context, then calls it.
- New helpers can be persisted, raising future-task success rates without code changes from the maintainer.
- Effectively an open-ended action space, bounded only by what the LLM can synthesize.

## Key Takeaways
- 592 lines = the framework is the prompt + a bit of glue.
- The pattern generalizes: any agent with code-execution can write its own missing tools.
- Pairs naturally with [[mempalace]] (persist learned helpers) and [[darwin-skill]] (evolve them).

## Related
- [[agent-frameworks-overview]]
- [[video-use]] — same authors
- [[mempalace]]
- [[darwin-skill]]
