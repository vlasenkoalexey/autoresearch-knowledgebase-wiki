---
title: Tool registry — scaffold-gated tool assembly
type: concept
provenance: mixed
concept: agents-tools-registry
updated: 2026-08-12
status: fresh
---
# Tool registry — scaffold-gated tool assembly

## Overview

`agents/tools/registry.py` is where the fixed set of tools an agent can call gets assembled per scaffold —
`build_tools_for_scaffold` combines a static `TOOL_REGISTRY` with dynamically-built local-subagent tool
declarations, filtered by which scaffold is running. This is the mechanism
[`agents-utils-harness_evolver`](agents-utils-harness_evolver.md)'s `_ALWAYS_AVAILABLE_TOOLS` set (in
`harness_evolver.py`) has to match against — an evolved subagent can only be given tools this registry
actually exposes for the `continualharness` scaffold.

## Design rationale (why it's built this way)

**Tool availability is scaffold-conditional, not global.** `_tool_available` checks each registry entry's
declared `scaffolds` set against the scaffold currently running — a tool entry defaults to `ALL_SCAFFOLDS`
but can be restricted, which is what lets the minimal `simple`/`simplest` baselines and the full
`continualharness` scaffold share one registry file while exposing different tool surfaces.

**Subagent tools are a second, structurally distinct layer on top of the static registry.**
`build_tools_for_scaffold` explicitly separates "1) Static registry tools" from "2) Local subagent tools" —
the `simplest` scaffold gets none of the subagent layer at all, and even within scaffolds that do get it,
`include_builtins` further restricts which built-in subagent tools are exposed based on whether the
scaffold is one of the `EXPERT_SCAFFOLDS`. This tiered gating is what keeps a deliberately minimal baseline
minimal — it isn't just a smaller prompt, it structurally cannot call tools the richer scaffolds can.

## Entry points
- `build_tools_for_scaffold` — the single function that assembles a scaffold's full tool declaration list;
  the resulting schema is what a scaffold's model turn (e.g.
  [`PokeAgent.run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step)) is given as its callable tools.

## Mechanism (step-by-step)
1. `build_tools_for_scaffold(scaffold)` iterates the static `TOOL_REGISTRY`, keeping only entries where
   `_tool_available` returns true for this scaffold — the schema
   [`PokeAgent.run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step) ultimately calls tools against.
2. Unless `scaffold == "simplest"`, it appends local-subagent tool declarations from `LOCAL_SUBAGENT_SPECS`
   (see [`agents-subagents-utils-registry`](agents-subagents-utils-registry.md)) — the same specs
   [`PokeAgent.run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step) dispatches against when a
   subagent tool is called — additionally gating any `BUILTIN_SUBAGENT_TOOL_NAMES` entries behind
   `scaffold in EXPERT_SCAFFOLDS`.
3. The combined list — each entry's `name`, `description`, `parameters` — is what gets handed to
   [`PokeAgent.run_step`](../catalog/agents/PokeAgent.md#PokeAgent.run_step) as the model's callable tool
   schema for that run.

## See also
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — the evolved-subagent tool-name
  validation this registry's availability rules bound.
- [`agents-subagents-utils-registry`](agents-subagents-utils-registry.md) — the local-subagent specs merged
  in at step 2.
