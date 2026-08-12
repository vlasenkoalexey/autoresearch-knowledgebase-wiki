---
title: AgentConnection types — the mode-agnostic session event contract
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-agent-connection-types.ts
updated: 2026-08-12
status: fresh
---
# AgentConnection types — the mode-agnostic session event contract

## Overview

[`AgentConnectionModel`](../catalog/packages/coding-agent/src/modes/agent-connection/types.ts.md#AgentConnectionModel)
and `AgentConnectionSessionEvent`/`AgentConnectionSessionEntry` define the wire contract every front end
(interactive terminal, daemon, RPC) consumes identically — the session's history is exposed as a
tree-flattened node list (`entry`, `id`) rather than each mode reaching into `SessionManager` directly.

## See also
- [`packages-coding-agent-src-modes-interactive-interactive-mode.ts`](packages-coding-agent-src-modes-interactive-interactive-mode.ts.md) —
  one consumer.
- [`packages-coding-agent-src-core-session-manager.ts`](packages-coding-agent-src-core-session-manager.ts.md) —
  the underlying tree these events are derived from.
