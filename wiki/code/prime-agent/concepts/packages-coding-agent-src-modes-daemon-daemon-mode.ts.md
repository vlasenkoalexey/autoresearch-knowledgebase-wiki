---
title: AgentDaemon — the worker-process session host
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-daemon-daemon-mode.ts
updated: 2026-08-12
status: fresh
---
# AgentDaemon — the worker-process session host

## Overview

`AgentDaemon.`[`handleCommand`](../catalog/packages/coding-agent/src/modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand)
dispatches every [`DaemonCommand`](packages-coding-agent-src-modes-daemon-daemon-protocol.ts.md) — `list`,
`create`, `attach`, `steer`, `follow_up`, and more — against the daemon's live `Map` of
[`ActiveSessionState`](packages-coding-agent-src-modes-daemon-active-session-state.ts.md)s. `createRuntime`
resolves a `create` command into a running session, joining an in-flight open rather than racing a second
one if another client is already opening the same session path.

`createRlmSubagentRuntime` is the daemon-side RLM spawn path: it builds a fresh
[`SessionManager`](packages-coding-agent-src-core-session-manager.ts.md) rooted at the parent's cwd,
tags the new session with `rlmDepth`, and wires an `rlmHeartbeatController` back through `this.cronStore`
so a subagent session can register its own [`AgentCronJob`](packages-coding-agent-src-core-cron-jobs.ts.md)
heartbeats — the daemon-mode counterpart to
[`AgentSession._startRlmChildRun`](packages-coding-agent-src-core-agent-session.ts.md), used when the
subagent must survive as an independently attachable daemon session rather than an in-process child.

## See also
- [`packages-coding-agent-src-modes-daemon-daemon-supervisor.ts`](packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md) —
  the process that launches and multiplexes `AgentDaemon` workers.
- [`packages-coding-agent-src-modes-daemon-daemon-session-list.ts`](packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) —
  builds the `list` command's response from this daemon's active sessions.
