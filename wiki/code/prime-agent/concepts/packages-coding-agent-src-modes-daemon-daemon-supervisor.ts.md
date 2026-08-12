---
title: DaemonSupervisor — multiplexing daemon worker processes
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-daemon-daemon-supervisor.ts
updated: 2026-08-12
status: fresh
---
# DaemonSupervisor — multiplexing daemon worker processes

## Overview

`DaemonSupervisor.`[`launchWorker`](../catalog/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.launchWorker)
spawns a detached child process (`--mode daemon --daemon-socket <path>`) per resident
[`AgentDaemon`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) worker, recording its
[`descriptor`](../catalog/packages/coding-agent/src/modes/daemon/daemon-supervisor.ts.md#ResidentWorker.descriptor)
(socket path, auth token, recovery-journal path) so a crashed worker can be relaunched and reattached.
`handleCommand` is the supervisor-level [`DaemonCommand`](packages-coding-agent-src-modes-daemon-daemon-protocol.ts.md)
dispatcher — routing `create`/`attach` to the right worker and handling `cancel_prompt_admission` locally —
while `handleWorkerFrame` relays a worker's `session_snapshot_begin` frames back out as
[`DaemonOutbound`](packages-coding-agent-src-modes-daemon-daemon-protocol.ts.md) events. This is the
process-supervision layer above individual daemon workers: one supervisor process, many resident session
workers, survivable worker crashes.

## See also
- [`packages-coding-agent-src-modes-daemon-daemon-mode.ts`](packages-coding-agent-src-modes-daemon-daemon-mode.ts.md) —
  the per-worker `AgentDaemon` this supervisor launches and relays frames from.
- [`packages-coding-agent-src-modes-daemon-active-session-state.ts`](packages-coding-agent-src-modes-daemon-active-session-state.ts.md) —
  referenced in prior packets as the `ActiveSessionState` shape the supervisor and workers share.
