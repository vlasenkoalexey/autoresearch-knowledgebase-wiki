---
title: server/app — the MCP surface for CLI-driven agents
type: concept
provenance: mixed
concept: server-app
updated: 2026-08-12
status: fresh
---
# server/app — the MCP surface for CLI-driven agents

## Overview

`server/app.py` exposes the game as an MCP-style HTTP server —
[`mcp_complete_direct_objective`](../catalog/server/app.md#mcp_complete_direct_objective) (*"MCP Tool:
Complete current direct objective"*) and `mcp_get_game_state` are the tool surface an external CLI backend
(see [`utils-agent_infrastructure-cli_agent_backends`](utils-agent_infrastructure-cli_agent_backends.md))
calls into via its own MCP proxy, rather than driving the agent's Python objects in-process. `env` and
`direct_objectives_manager` are the module-level singletons every route handler reads and mutates.

## See also
- [`agents-objectives-objective_types`](agents-objectives-objective_types.md) — `DirectObjective`, the type
  these routes serialize.
- [`utils-agent_infrastructure-cli_agent_backends`](utils-agent_infrastructure-cli_agent_backends.md) — the
  client side of this server.
