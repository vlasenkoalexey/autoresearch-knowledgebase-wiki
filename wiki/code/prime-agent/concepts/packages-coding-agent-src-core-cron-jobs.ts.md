---
title: AgentCronJob — scheduled agent invocations, including RLM heartbeats
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-cron-jobs.ts
updated: 2026-08-12
status: fresh
---
# AgentCronJob — scheduled agent invocations, including RLM heartbeats

## Overview

`AgentCronJobStore.`[`createHeartbeat`](../catalog/packages/coding-agent/src/core/cron-jobs.ts.md#AgentCronJobStore.createHeartbeat)
creates a scheduled [`AgentCronJob`](../catalog/packages/coding-agent/src/core/cron-jobs.ts.md#AgentCronJob);
a sibling `createRlmHeartbeat` (named in this module's seeds) confirms the scheduling mechanism is used to
periodically re-invoke the agent, including RLM-specific scheduled runs — the persistent-goals/schedules
feature the README lists ("persistent goals, heartbeats, schedules, autonomous mode... preserve progress
across turns and terminal sessions").

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  the session a scheduled job ultimately drives.
