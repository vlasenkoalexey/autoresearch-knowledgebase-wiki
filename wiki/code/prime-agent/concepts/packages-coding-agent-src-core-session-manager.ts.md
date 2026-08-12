---
title: SessionManager — conversation history as an append-only tree
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-session-manager.ts
updated: 2026-08-12
status: fresh
---
# SessionManager — conversation history as an append-only tree

## Overview

[`SessionManager`](../catalog/packages/coding-agent/src/core/session-manager.ts.md#SessionManager) —
*"Manages conversation sessions as append-only trees stored in JSONL files"* — is the persistence layer
under [`AgentSession`](packages-coding-agent-src-core-agent-session.ts.md). Its
[`appendMessage`](../catalog/packages/coding-agent/src/core/session-manager.ts.md#SessionManager.appendMessage) —
*"Append a message as child of current leaf, then advance leaf. Returns entry id"* — is the same shape as a
git commit: every new entry is a child of the current position, and the "leaf" pointer advances, so history
is structurally a tree (supporting forks/branches) rather than a flat log.

## See also
- [`packages-coding-agent-src-core-agent-session.ts`](packages-coding-agent-src-core-agent-session.ts.md) —
  the caller.
