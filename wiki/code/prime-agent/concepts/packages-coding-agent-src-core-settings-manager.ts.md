---
title: SettingsManager — layered configuration
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-settings-manager.ts
updated: 2026-08-12
status: fresh
---
# SettingsManager — layered configuration

## Overview

[`SettingsManager.create`](../catalog/packages/coding-agent/src/core/settings-manager.ts.md#SettingsManager.create) —
*"Create a SettingsManager that loads from files"* — resolves configuration from `cwd` and `agentDir`,
distinct from an in-memory variant used in tests — the general project-settings layer underneath
per-session config, orthogonal to the RLM/Continual-Harness mechanisms.

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  a consumer via `AgentSessionConfig`.
