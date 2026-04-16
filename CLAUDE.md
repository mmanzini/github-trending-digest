# GitHub Trends – Project Instructions

## Git Workflow

**Always commit and push directly to `main`.** Do not create feature branches. Every run should end with a push to `origin main`.

```
git add <files>
git commit -m "..."
git push -u origin main
```

## What This Repo Does

Generates a daily GitHub trending digest at `trending/YYYY-MM-DD-trending.md`. Each file covers:
- Top 10 repos created in the last 7 days (sorted by stars)
- Top 5 repos created in the last 30 days (sorted by stars)

Repos relevant to AI agents, Claude Code, LLM tooling, or developer experience are flagged `[AI/DEV]`.
