---
title: Prompt paths — where the immutable base prompt actually lives
type: concept
provenance: mixed
concept: agents-prompts-paths
updated: 2026-08-12
status: fresh
---
# Prompt paths — where the immutable base prompt actually lives

## Overview

[`CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH`](../catalog/agents/prompts/paths.md#CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH)
is the concrete file path grounding the paper's stated immutable-base-prompt boundary: it is passed as
`base_prompt_path` into [`HarnessEvolver.__init__`](agents-utils-harness_evolver.md) (via the composed
`PromptOptimizer`), and `PROMPTS_ROOT`/`GAME_NAME`-derived paths like `POKEAGENT_PROMPT_PATH` resolve which
game's prompt set is loaded. The Refiner's `_evolve_prompt` pass rewrites the *orchestrator policy* content
this path points at, not this constant itself.

## See also
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — the consumer of this path at construction.
