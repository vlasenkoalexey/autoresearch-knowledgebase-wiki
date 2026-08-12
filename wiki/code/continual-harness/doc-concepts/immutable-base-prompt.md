---
title: The immutable base prompt boundary
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# The immutable base prompt boundary

## Definition
The README states one hard boundary on self-modification: "The base system prompt is immutable. Everything
built on top of it — memories, skills, sub-agent definitions — is the agent's to rewrite."

## In continual-harness (grounded)
[`agents-prompts-paths`](../concepts/agents-prompts-paths.md)'s
`CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH` is the concrete file this boundary protects — it's passed
into [`agents-utils-harness_evolver`](../concepts/agents-utils-harness_evolver.md)'s `HarnessEvolver`
constructor, but `_evolve_prompt`'s rewrite targets an evolvable *orchestrator policy* layered on top of
that path, not the base path constant itself. The three other evolution passes (subagents, skills, memory)
operate on genuinely separate, explicitly mutable stores
([`utils-stores-subagents`](../concepts/utils-stores-subagents.md)).

## Why it matters / when it applies
This is the same design move [Prime Agent](../../../sources/prime-agent-launch.md)'s launch post describes
independently — *"immutable base prompts"* — for its own `/refine` mechanism, which is built on this exact
paper. A boundary an evolving system cannot cross is what keeps self-modification from drifting into
rewriting its own safety/goal-alignment scaffolding, not just its tactical knowledge.

## Connections
- Code concepts: [`agents-prompts-paths`](../concepts/agents-prompts-paths.md),
  [`agents-utils-harness_evolver`](../concepts/agents-utils-harness_evolver.md)
- Related doc-concepts: [reset-free-harness-evolution](reset-free-harness-evolution.md)
- Wiki: [`sources/prime-agent-launch.md`](../../../sources/prime-agent-launch.md) — the product implementing
  the same boundary.

## Source
Extracted from `README.md` (kept in place).
