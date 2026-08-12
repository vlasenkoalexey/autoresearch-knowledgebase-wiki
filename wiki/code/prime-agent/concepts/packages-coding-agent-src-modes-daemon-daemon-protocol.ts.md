---
title: Daemon protocol — the RPC contract between CLI and background daemon
type: concept
provenance: mixed
concept: packages-coding-agent-src-modes-daemon-daemon-protocol.ts
updated: 2026-08-12
status: fresh
---
# Daemon protocol — the RPC contract between CLI and background daemon

## Overview

[`DaemonCommand`](../catalog/packages/coding-agent/src/modes/daemon/daemon-protocol.ts.md#DaemonCommand)
(inbound) and [`DaemonOutbound`](../catalog/packages/coding-agent/src/modes/daemon/daemon-protocol.ts.md#DaemonOutbound)
(outbound, wrapping `AgentConnectionSessionEvent`/`AgentMessage`/`SessionSummary`) define the wire protocol
between a CLI client and the background daemon process — the concrete mechanism behind the README's
"daemon-backed agents keep running when the terminal disconnects."

## See also
- [`packages-coding-agent-src-modes-agent-connection-types.ts`](packages-coding-agent-src-modes-agent-connection-types.ts.md) —
  the session-event types this protocol wraps.
