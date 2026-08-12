---
title: DirectObjective — the structured task unit
type: concept
provenance: mixed
concept: agents-objectives-objective_types
updated: 2026-08-12
status: fresh
---
# DirectObjective — the structured task unit

## Overview

[`DirectObjective`](../catalog/agents/objectives/objective_types.md#DirectObjective) — *"Single direct
objective with specific guidance"* — is the structured unit the game's story/battling/dynamics sequences are
built from: `id`, `description`, `action_type`, `category`, `target_location`, `completion_condition`,
`navigation_hint`, `priority`, and `prerequisite_story_objective`. This is the vocabulary
[`server-app`](server-app.md)'s MCP routes (`mcp_complete_direct_objective`) and
[`agents-PokeAgent`](agents-PokeAgent.md) both operate over — a task the agent is working toward has this
shape regardless of which layer is currently consuming it.

## See also
- [`server-app`](server-app.md) — where objectives are served and completed via MCP tools.
