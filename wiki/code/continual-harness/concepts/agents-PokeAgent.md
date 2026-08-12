---
title: PokeAgent — the orchestrator loop that calls the evolver
type: concept
provenance: mixed
concept: agents-PokeAgent
updated: 2026-08-12
status: fresh
---
# PokeAgent — the orchestrator loop that calls the evolver

## Overview

`PokeAgent` is the top-level agent class; [`run`](../catalog/agents/PokeAgent.md#PokeAgent.run) — *"Run the
autonomous agent loop"* — drives repeated calls to
[`run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step) — *"Run a single agent step"* — which is
where [`harness_evolver.evolve`](agents-utils-harness_evolver.md) is actually invoked. Two specialized loop
variants exist alongside the main step function:
[`_run_planner_loop`](../catalog/agents/PokeAgent.md#PokeAgent._run_planner_loop) and
[`_run_battler_loop`](../catalog/agents/PokeAgent.md#PokeAgent._run_battler_loop) — separate execution paths
for planning-mode and battle-mode play, both routing through the same subagent-dispatch machinery
(`_handle_vlm_function_calls`, `call_tool`, `get_query`).

## Design rationale (why it's built this way)

**`harness_evolver` is a per-instance attribute holding the `HarnessEvolver`**, constructed alongside the
agent's own `vlm` and `run_data_manager` — the evolution mechanism is wired into the agent, not invoked as
an external process, so `run_step` can call `evolve` directly on its own generation counter.

**Planner and battler are distinct code paths, not the same loop with a mode flag.** `_run_planner_loop`
and `_run_battler_loop` share most of their machinery (subagent VLM, trajectory-window clamping in the
battler path, MCP tool calls) but are separately named methods — this repo treats the battle/exploration
split as structurally different enough to warrant its own loop function rather than branching inside one.

## Entry points
- [`PokeAgent.run`](../catalog/agents/PokeAgent.md#PokeAgent.run) — the top-level autonomous loop.
- [`PokeAgent.run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step) — one step; this is where
  [`HarnessEvolver.evolve`](agents-utils-harness_evolver.md) gets called (the packet's own subgraph cites
  `run_step`'s reference to `harness_evolver`/`evolve`).

## See also
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — the mechanism `run_step` invokes.
- [`utils-stores-subagents`](utils-stores-subagents.md) — the store `_evolve_subagents` and the
  planner/battler loops both read from.
