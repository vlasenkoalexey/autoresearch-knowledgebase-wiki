---
title: pi-agent-core types — AgentMessage and the base agent-loop vocabulary
type: concept
provenance: mixed
concept: packages-agent-src-types.ts
updated: 2026-08-12
status: fresh
---
# pi-agent-core types — AgentMessage and the base agent-loop vocabulary

## Overview

`packages/agent` is the model-agnostic agent-loop package underneath `packages/coding-agent`.
[`AgentMessage`](../catalog/packages/agent/src/types.ts.md#AgentMessage) —
*"Union of LLM messages + custom messages"* — is the base type
[`packages-coding-agent-src-core-messages.ts`](packages-coding-agent-src-core-messages.ts.md)'s
`CustomMessage`/`BashExecutionMessage` extend, and `AgentState.`[`<get>messages`](../catalog/packages/agent/src/types.ts.md#AgentState.-get-messages)/[`<set>messages`](../catalog/packages/agent/src/types.ts.md#AgentState.-set-messages) —
*"Conversation transcript. Assigning a new array copies the top-level array"* — is the state slice
`AgentSession.`[`<get>messages`](packages-coding-agent-src-core-agent-session.ts.md) wraps.
[`ThinkingLevel`](../catalog/packages/agent/src/types.ts.md#ThinkingLevel) —
*"Thinking/reasoning level for models that support it"* (`"off" | "minimal" | "low" | "medium" | "high" |
"xhigh" | "max"`) — is the coding-agent's reasoning-effort dial, threaded through
[`DaemonCommand`](packages-coding-agent-src-modes-daemon-daemon-protocol.ts.md) and session config alike.

## See also
- [`packages-ai-src-types.ts`](packages-ai-src-types.ts.md) — the sibling `Model`/`AssistantMessage`
  vocabulary from `packages/ai`, one layer below `packages/agent`.
- [`packages-coding-agent-src-core-messages.ts`](packages-coding-agent-src-core-messages.ts.md) —
  the coding-agent's own message-type extensions to `AgentMessage`.
