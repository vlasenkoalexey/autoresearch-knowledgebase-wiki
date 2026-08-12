---
title: DirectObjectiveManager — batch-editable objective sequences
type: concept
provenance: mixed
concept: agents-objectives-direct_objectives
updated: 2026-08-12
status: fresh
---
# DirectObjectiveManager — batch-editable objective sequences

## Overview

`DirectObjectiveManager` holds the story/battling/dynamics objective sequences (each a `list[DirectObjective]`,
see [`agents-objectives-objective_types`](agents-objectives-objective_types.md)) and exposes
[`replan_category`](../catalog/agents/objectives/direct_objectives.md#DirectObjectiveManager.replan_category) —
*"Apply a batch of index-based edits to a single objective category"* — and
[`add_objectives_to_category`](../catalog/agents/objectives/direct_objectives.md#DirectObjectiveManager.add_objectives_to_category).
This is a second CRUD-shaped surface alongside [`HarnessEvolver`](agents-utils-harness_evolver.md)'s, but
for the game's own task plan rather than the agent's harness components — objectives can be batch-edited
by index, not just appended.

## See also
- [`agents-objectives-objective_types`](agents-objectives-objective_types.md) — the `DirectObjective` type.
- [`server-app`](server-app.md) — the MCP route that reaches this manager.
