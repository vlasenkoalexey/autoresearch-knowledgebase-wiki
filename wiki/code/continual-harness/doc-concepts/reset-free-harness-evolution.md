---
title: Reset-free harness evolution — the paper's headline claim
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Reset-free harness evolution — the paper's headline claim

## Definition
The README states the `continualharness` scaffold "starts from the minimalist interface (frames, ASCII
text map, button inputs) and lets the model evolve its own harness in place during a single continuous
episode — no resets between updates," running four passes every `--optimization-window-length` steps: a
system-prompt rewrite, and CRUD over sub-agents, skills, and memory.

## In continual-harness (grounded)
This maps directly onto [`agents-utils-harness_evolver`](../concepts/agents-utils-harness_evolver.md)'s
`HarnessEvolver.evolve`, which runs the four passes (`_evolve_prompt`, `_evolve_subagents`,
`_evolve_skills`, `_evolve_memory`) against a trajectory window, each independently fault-isolated. The
CRUD operations land in [`utils-stores-subagents`](../concepts/utils-stores-subagents.md)'s
`BaseStore.add`/`.update`/`.remove` — real persisted store mutations, not just prompt text changes.
`evolve_harness` (the README's named tool exposing this to the agent) corresponds to the same
`HarnessEvolver.evolve` call, reached via `--enable-prompt-optimization`.

## Why it matters / when it applies
"Reset-free" is the load-bearing claim distinguishing this from ordinary prompt-optimization methods, which
the README states explicitly require episode resets. The practical consequence, grounded in
`should_evolve`'s adaptive schedule (every 25 steps for the first 200, then every 100), is that the harness
is expected to still be adapting well into a long-running episode, not just once at the start.

## Connections
- Code concepts: [`agents-utils-harness_evolver`](../concepts/agents-utils-harness_evolver.md),
  [`utils-stores-subagents`](../concepts/utils-stores-subagents.md),
  [`agents-PokeAgent`](../concepts/agents-PokeAgent.md)
- Module catalogs: [`agents/utils/harness_evolver`](../catalog/agents/utils/harness_evolver.md)
- Related doc-concepts: [immutable-base-prompt](immutable-base-prompt.md)
- Wiki: [`sources/continual-harness.md`](../../../sources/continual-harness.md) — the paper this
  implements; [`concepts/self-referential-code-rewriting.md`](../../../concepts/self-referential-code-rewriting.md) —
  the vocabulary key this mechanism plausibly connects to (a candidate for the connect step).

## Source
Extracted from `README.md` (kept in place).
