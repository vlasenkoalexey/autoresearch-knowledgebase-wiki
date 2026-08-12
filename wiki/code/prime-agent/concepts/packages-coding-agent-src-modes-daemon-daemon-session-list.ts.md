---
title: SessionSummary — the daemon's session-list projection
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-daemon-daemon-session-list.ts
updated: 2026-08-12
status: fresh
---
# SessionSummary — the daemon's session-list projection

## Overview

[`summaryForActiveSession`](../catalog/packages/coding-agent/src/modes/daemon/daemon-session-list.ts.md#summaryForActiveSession)
projects a live [`ActiveSessionState`](packages-coding-agent-src-modes-daemon-active-session-state.ts.md)
into a [`SessionSummary`](../catalog/packages/coding-agent/src/modes/daemon/daemon-session-list.ts.md#SessionSummary) —
`id`, `activeSessionId`, `sessionId`, `rlmDepth`, `hasRunningRlmChildren`, `taskState`, `spawnCode` (the
IPython cell that spawned an RLM subagent) — the read model
[`AgentDaemon.handleCommand`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md)'s `list` case and
the agents-view mode render from, without exposing the full message history. A sibling
`summaryForInactiveSession` builds the same shape from a saved-but-not-running `SessionInfo`.

## See also
- [`packages-coding-agent-src-modes-daemon-daemon-mode.ts`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) —
  the daemon whose `list` command returns these summaries.
- [`packages-coding-agent-src-modes-daemon-daemon-supervisor.ts`](packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md) —
  aggregates summaries across multiple daemon workers.
