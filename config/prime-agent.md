---
slug: prime-agent
repo: raw/code/prime-agent
acquire: submodule
docs: [README.md]
synthesis_focus: the two core abstractions — RLM (context as a REPL variable, rlm(...) subagent calls as ordinary function calls inside a persistent Python/IPython kernel) and Continual Harness (/refine, CRUD self-editing of prompt/subagents/skills/memory with an immutable base prompt) — and how they compose into one coding/research agent
coverage_collapse:
  - packages/coding-agent/examples/**
  - packages/coding-agent/src/themes/**
  - packages/tui/**
---

## Concepts
- packages-coding-agent-src-core-refinement-refinement.ts
- packages-coding-agent-src-core-kernel-index.ts
