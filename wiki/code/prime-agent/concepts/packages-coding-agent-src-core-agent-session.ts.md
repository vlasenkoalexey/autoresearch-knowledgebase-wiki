---
title: AgentSession — the root session and where rlm(...) spawns a child
type: concept
provenance: mixed
concept: packages-coding-agent-src-core-agent-session.ts
updated: 2026-08-12
status: fresh
---
# AgentSession — the root session and where rlm(...) spawns a child

## Overview

`AgentSession` is the top-level object driving one agent conversation —
[`prompt`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession.prompt) (*"Send a
prompt to the agent"*) is the entry point every turn goes through. Its
[`_startRlmChildRun`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession._startRlmChildRun)
method is the concrete site where a model-generated `rlm(...)` call in the REPL becomes a real child agent
run, returning an `RlmSpawnHandle` — the TypeScript analog of
[`RLM._subcall`](../../rlm/concepts/rlm-core-rlm.md) in the Python reference implementation.

## Design rationale (why it's built this way)

**The spawn call returns a handle, not a completion.** `_startRlmChildRun`'s return type,
`Promise<RlmSpawnHandle>`, matches the video's own framing of this mechanism precisely: *"the call returns
immediately, not with an answer, with a handle"* — the child works elsewhere and the parent's turn can end
without blocking on it, which is what lets one line of generated code fire off several sub-agent calls and
move on.

**Session identity is threaded through construction, not assembled ad hoc per call.** The
[`<constructor>`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession.-constructor)
takes a full `AgentSessionConfig` and resolves the [`agent`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession.agent)
property once — every subsequent `prompt()` call and every `_startRlmChildRun` reuses that same resolved
agent/session identity rather than re-deriving it per turn.

## Entry points
- [`AgentSession.prompt`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession.prompt) —
  the ordinary conversational entry point.
- [`AgentSession._startRlmChildRun`](../catalog/packages/coding-agent/src/core/agent-session.ts.md#AgentSession._startRlmChildRun) —
  reached from model-generated code inside the [`KernelManager`](packages-coding-agent-src-core-kernel-index.ts.md)
  REPL when it calls `rlm(...)`.

## See also
- [`packages-coding-agent-src-core-kernel-index.ts`](packages-coding-agent-src-core-kernel-index.ts.md) —
  the REPL execution substrate this session's kernel-backed code runs in.
- [`rlm-core-rlm`](../../rlm/concepts/rlm-core-rlm.md) — the Python reference implementation's `_subcall`,
  the closest structural analog.
