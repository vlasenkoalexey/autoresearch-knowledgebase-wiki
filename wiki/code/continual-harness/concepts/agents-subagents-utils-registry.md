---
title: Local subagent registry — the specs behind built-in subagent tools
type: concept
provenance: mixed
concept: agents-subagents-utils-registry
updated: 2026-08-12
status: fresh
---
# Local subagent registry — the specs behind built-in subagent tools

## Overview

`LOCAL_SUBAGENT_SPECS` is a static tuple of `LocalSubagentSpec` entries (per-game via `_EMERALD_PUZZLE_SPEC`/
`_RED_PUZZLE_SPEC`), and
[`build_local_subagent_tool_declarations`](../catalog/agents/subagents/utils/registry.md#build_local_subagent_tool_declarations)
turns them into callable tool schemas — the built-in counterpart
[`agents-tools-registry`](agents-tools-registry.md)'s `build_tools_for_scaffold` merges alongside the static
tool registry, and the baseline every *evolved* subagent from
[`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) is added on top of.

## See also
- [`agents-tools-registry`](agents-tools-registry.md) — where these specs get merged into the final tool list.
