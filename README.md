# Claude Certified Architect — Foundations · Interactive Study Guide

A single-page, no-build interactive study guide for the **Claude Certified Architect — Foundations**
exam, plus twelve hands-on deep-dive pages with annotated, verified sample code and interactive demos.

**Live:** https://bradvatne.github.io/claude-architect-study-guide/

## What's inside

- **Overview & the six decision principles** — the judgment tie-breakers the exam keeps testing.
- **Five domain modules** (D1–D5) with checkable "nail this" points (progress saved in your browser),
  weighted by exam blueprint.
- **Flashcards** (per-domain decks + a decision-principle deck), a **scenario quiz**, a
  **distractor deck** ("what doesn't exist"), the study plan, and canonical sources.
- **12 deep dives** (`deep-dives.html`) — one per topic, each with sample code, an interactive widget,
  and a "how this shows up on the exam" mapping:
  - **D1** — the agentic loop & `stop_reason`, subagents & the coordinator pattern, deterministic gates & hooks
  - **D2** — tool design (descriptions, `tool_choice`, structured errors), MCP integration
  - **D3** — `CLAUDE.md`/rules/commands/skills, Claude Code in CI / headless
  - **D4** — structured output, Message Batches API, prompt engineering for judgment
  - **D5** — context management, escalation/errors/provenance

## Running locally

It's a static site — no build step. From this directory:

```sh
python3 -m http.server 8090 --bind 127.0.0.1
# then open http://127.0.0.1:8090/
```

## Accuracy note

Code samples were checked against the current Claude API / Anthropic SDK reference (default model
`claude-opus-4-8`). Version-sensitive Claude Code specifics (CLI flags, frontmatter keys) are hedged
on-page — treat the exam guide as authoritative for the test and the live docs as authoritative for
reality. Built from the official exam guide v0.1.
