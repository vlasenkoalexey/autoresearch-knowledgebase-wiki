---
title: AgentSessionMessage — cross-session messages between family members
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-agent-messages.ts
updated: 2026-08-12
status: fresh
---
# AgentSessionMessage — cross-session messages between family members

## Overview

[`createAgentSessionMessage`](../catalog/packages/coding-agent/src/core/agent-messages.ts.md#createAgentSessionMessage)
builds an `AgentSessionMessage` — a message one session sends to another related session (parent, RLM
child, or named agent) — from a `from`/`target`/`fromRelationship` payload;
[`createAgentSessionMessagePrompt`](../catalog/packages/coding-agent/src/core/agent-messages.ts.md#createAgentSessionMessagePrompt)
renders it as the literal `"[task from parent]\n\n..."`-style prefixed text a receiving session sees in its
transcript, and [`isAgentSessionMessage`](../catalog/packages/coding-agent/src/core/agent-messages.ts.md#isAgentSessionMessage)
is the runtime type guard `AgentSession._startRlmChildRun` and `InteractiveMode.handleEvent` use to detect
one. `buildAgentFamilyRoster` walks an `AgentFamilyCatalogEntry` tree by `depth` and shared-parent identity
to compute which other live sessions a given session may address — the addressing layer underneath
cross-session RLM communication, distinct from the in-process `rlm(...)` call inside one kernel.

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  `_startRlmChildRun`, the RLM spawn site that tags its child's first message this way.
- [`packages-coding-agent-src-core-messages.ts`](packages-coding-agent-src-core-messages.ts.md) —
  the base `AgentMessage` union `AgentSessionMessage` is a member of.
