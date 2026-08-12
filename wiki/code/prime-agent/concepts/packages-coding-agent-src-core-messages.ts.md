---
title: Message types — the discriminated-union conversation shape
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-messages.ts
updated: 2026-08-12
status: fresh
---
# Message types — the discriminated-union conversation shape

## Overview

`messages.ts` defines the conversation entry types [`SessionManager`](packages-coding-agent-src-core-session-manager.ts.md)
persists — `CustomMessage.`[`role`](../catalog/packages/coding-agent/src/core/messages.ts.md#CustomMessage.role)
(`"custom"`) and `BashExecutionMessage.`[`role`](../catalog/packages/coding-agent/src/core/messages.ts.md#BashExecutionMessage.role)
(`"bashExecution"`) are two of the discriminated-union members `appendMessage` accepts, alongside ordinary
chat messages — the type-level enumeration of everything that can be a node in the session tree.

## See also
- [`packages-coding-agent-src-core-session-manager.ts`](packages-coding-agent-src-core-session-manager.ts.md) —
  the consumer of these types.
