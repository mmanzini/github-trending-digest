# Clawsweeper

**Repo:** [openclaw/clawsweeper](https://github.com/openclaw/clawsweeper)
**Language:** JavaScript | **First seen:** 2026-04-26 | **Stars (7-day peak):** ~1,057

LLM-powered GitHub maintenance bot that runs on a weekly schedule. Scans all open issues and pull requests in a repository, uses GPT-5.5 to assess closure eligibility with evidence-based reasoning, and auto-closes only when confidence is high. Maintainer-owned items are never auto-closed.

## Design Principles
- **Evidence-based reasoning** — the model generates a justification chain before proposing a closure, not just a binary yes/no
- **Confidence threshold** — closures only trigger above a set confidence score; borderline cases are surfaced for human review
- **Maintainer exemption** — issues/PRs opened by repo maintainers are excluded from automated closure
- **Weekly cadence** — lightweight background job, not a real-time webhook

## Use Case
Addresses the triaging backlog problem for popular open-source repos where issue/PR volume outpaces human review capacity. Positions LLMs as "triage auditors" rather than primary maintainers.

## Key Takeaways
- The pattern (LLM as triage auditor with confidence gating) is applicable beyond GitHub to any ticketing system
- Explicit maintainer exemption is a trust signal: the tool knows what it shouldn't touch
- Uses GPT-5.5 (not Claude), making it a cross-vendor agent deployment
- See also: [[advisor-ledger]] for a related LLM-as-document-guardian pattern
