---
title: Long-running continuity — daemons, heartbeats, goals, bounded autonomy
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# Long-running continuity — daemons, heartbeats, goals, bounded autonomy

## Definition
The README lists a cluster of features aimed at survival across turns and disconnects: "daemon-backed
agents keep running when the terminal disconnects and can be reattached later"; "`/heartbeat`,
`rlm_heartbeat`, and `prime-agent schedule` can re-enter a session periodically or at a specific time";
"`/goal` keeps an objective and its progress active across turns until it is completed, paused, or
cleared"; and "`/autonomous` continues within configured turn, token, and time budgets and can run
user-defined quality gates" — with an explicit caveat: "a passed gate checks only what that gate verifies;
reaching a limit does not imply task success."

## In prime-agent (grounded)
The daemon-process layer is concrete: [`AgentDaemon`](../concepts/packages-coding-agent-src-modes-daemon-daemon-mode.ts.md)
hosts one [`ActiveSessionState`](../concepts/packages-coding-agent-src-modes-daemon-active-session-state.ts.md)
per running session inside a worker process, [`DaemonSupervisor`](../concepts/packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md)
launches and relaunches those workers so a crash doesn't lose session state, and
[`AgentCronJobStore.createHeartbeat`/`createRlmHeartbeat`](../concepts/packages-coding-agent-src-core-cron-jobs.ts.md)
is the scheduling primitive behind `/heartbeat` and `rlm_heartbeat`. The
[`SessionSummary`](../concepts/packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md) a client
reads back (`rlmDepth`, `hasRunningRlmChildren`, `taskState`) is how a reattaching terminal or the
[`AgentsViewMode`](../concepts/packages-coding-agent-src-modes-agents-view-agents-view-mode.ts.md) dashboard
recovers what a detached session was doing.

## Why it matters / when it applies
This is the systems-engineering counterpart to the RLM/Continual-Harness mechanisms: those two give the
agent a way to *reason* over a long task; the daemon/heartbeat/goal stack gives it a way to *survive* one —
terminal disconnects, process crashes, and multi-day evaluation runs. The explicit "reaching a limit does
not imply task success" caveat is worth carrying into any evaluation of autonomous-mode runs reported
elsewhere in this wiki (e.g. [ARC-AGI-3](../../../sources/arc-agi-3.md) benchmark runs) — a bounded budget
is a stopping condition, not a correctness signal.

## Connections
- Code concepts: [`packages-coding-agent-src-modes-daemon-daemon-mode.ts`](../concepts/packages-coding-agent-src-modes-daemon-daemon-mode.ts.md),
  [`packages-coding-agent-src-modes-daemon-daemon-supervisor.ts`](../concepts/packages-coding-agent-src-modes-daemon-daemon-supervisor.ts.md),
  [`packages-coding-agent-src-core-cron-jobs.ts`](../concepts/packages-coding-agent-src-core-cron-jobs.ts.md),
  [`packages-coding-agent-src-modes-daemon-daemon-session-list.ts`](../concepts/packages-coding-agent-src-modes-daemon-daemon-session-list.ts.md)
- Wiki: [`sources/prime-agent-launch.md`](../../../sources/prime-agent-launch.md),
  [`sources/arc-agi-3.md`](../../../sources/arc-agi-3.md)

## Source
Extracted from `README.md` (kept in place).
