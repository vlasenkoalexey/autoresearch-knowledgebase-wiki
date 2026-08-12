---
title: SessionAction — the queued-turn/command model behind the agent pump
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-session-action-store.ts
updated: 2026-08-12
status: fresh
---
# SessionAction — the queued-turn/command model behind the agent pump

## Overview

`SessionAction.`[`payload`](../catalog/packages/coding-agent/src/core/session-action-store.ts.md#SessionAction.payload)
and `.`[`lifecycle`](../catalog/packages/coding-agent/src/core/session-action-store.ts.md#SessionAction.lifecycle)
back every queued unit of work `AgentSession` admits — either a
[`SessionTurnPayload`](../catalog/packages/coding-agent/src/core/session-action-store.ts.md#SessionTurnPayload.kind)
(`kind: "turn"`, a user/steer/follow-up prompt) or a
[`SessionCommandPayload`](../catalog/packages/coding-agent/src/core/session-action-store.ts.md#SessionCommandPayload.kind)
(`kind: "session_command"`, e.g. compact, fork, refine). `AgentSession._pumpSessionInputs` selects the next
admissible action by lifecycle state and dispatches it to `_startPreparedTurnActions` or
`_executeSelectedSessionCommand`; `_cancelSessionActions` and `restoreSessionActions` handle abort and
crash-recovery replay of the same queue.

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  the session that owns and pumps this action queue.
