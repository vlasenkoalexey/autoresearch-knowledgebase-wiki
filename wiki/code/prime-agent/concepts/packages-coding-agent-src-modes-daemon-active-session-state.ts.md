---
title: ActiveSessionState — the daemon's in-memory session record
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-daemon-active-session-state.ts
updated: 2026-08-12
status: fresh
---
# ActiveSessionState — the daemon's in-memory session record

## Overview

[`ActiveSessionState`](../catalog/packages/coding-agent/src/modes/daemon/active-session-state.ts.md#ActiveSessionState) —
`activeSessionId`, `.`[`runtime`](../catalog/packages/coding-agent/src/modes/daemon/active-session-state.ts.md#ActiveSessionState.runtime)
(an `AgentSessionRuntime`), `clients`, `clientEnv` — is the record
[`AgentDaemon`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) keeps per live session, and
[`DaemonSocketClient`](../catalog/packages/coding-agent/src/modes/daemon/active-session-state.ts.md#DaemonSocketClient)
is the matching record per attached socket (`attachedActiveSessionIds`, `catchupActiveSessionIds`,
`capabilities`). `summaryForActiveSession`, `handleCommand`, and `createRuntime`/`createRlmSubagentRuntime`
all take an `ActiveSessionState` as their unit of work — the daemon-mode module's central in-memory type,
distinct from the on-disk `SessionInfo` a saved-but-inactive session is represented by.

## See also
- [`packages-coding-agent-src-modes-daemon-daemon-mode.ts`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) —
  owns the `Map` of `ActiveSessionState` this module's types describe.
- [`packages-coding-agent-src-modes-daemon-daemon-session-list.ts`](packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) —
  projects `ActiveSessionState` into the client-facing `SessionSummary`.
