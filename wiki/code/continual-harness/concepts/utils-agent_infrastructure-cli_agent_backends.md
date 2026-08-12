---
title: CLI agent backends — running external CLI harnesses inside this scaffold
type: concept
provenance: mixed
concept: utils-agent_infrastructure-cli_agent_backends
updated: 2026-08-12
status: fresh
---
# CLI agent backends — running external CLI harnesses inside this scaffold

## Overview

This module lets the repo drive external coding-agent CLIs (Claude Code, and a "Hermes" backend among
others) as playable agents, matching the README's stated support for *"External CLI harnesses — Claude
Code, Gemini CLI, Codex, and Hermes via an MCP proxy."* Each backend
([`ClaudeCodeBackend`](../catalog/utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.handle_stream_event),
`HermesCliBackend`) implements its own `handle_stream_event`, parsing that CLI's own streaming protocol
into a shared [`CliSessionMetrics`](../catalog/utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics) —
*"Metrics collected from a single CLI agent session (e.g. stream-json result event)"* — capturing tokens,
cost, tool-use counts uniformly across otherwise-incompatible CLI tools.

## See also
- [`agents-PokeAgent`](agents-PokeAgent.md) — the orchestrator these backends can stand in for.
