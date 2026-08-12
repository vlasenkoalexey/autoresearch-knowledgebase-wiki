---
title: 'Module: packages/coding-agent/src/core/rlm-max-depth.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/rlm-max-depth.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`rlm-max-depth.ts`/
symbols:
  RlmMaxDepthStatus: RlmMaxDepthStatus#
  SetRlmMaxDepthResult: SetRlmMaxDepthResult#
  RlmMaxDepthSource: RlmMaxDepthSource#
  RlmMaxDepthStatus.maxDepth: RlmMaxDepthStatus#maxDepth.
  SetRlmMaxDepthResult.globalError: SetRlmMaxDepthResult#globalError.
  RlmMaxDepthStatus.source: RlmMaxDepthStatus#source.
  SetRlmMaxDepthResult.globalSaved: SetRlmMaxDepthResult#globalSaved.
---
# Module: [`packages/coding-agent/src/core/rlm-max-depth.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts)

## Classes
### `RlmMaxDepthSource`
- def: [`packages/coding-agent/src/core/rlm-max-depth.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L3)
- doc: Wire-safe types for the immediate /rlm-max-depth state APIs.
- signature: `type RlmMaxDepthSource`
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`_resolveRlmMaxDepth`](agent-session.ts.md#AgentSession._resolveRlmMaxDepth), [`RlmMaxDepthStatus`](rlm-max-depth.ts.md#RlmMaxDepthStatus), [`_rlmMaxDepthSource`](agent-session.ts.md#AgentSession._rlmMaxDepthSource)

### `RlmMaxDepthStatus`
- def: [`packages/coding-agent/src/core/rlm-max-depth.ts:5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L5)
- signature: `interface RlmMaxDepthStatus`
- members:
  - `maxDepth` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L6)
  - `source` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L7)
- uses (calls/refs, reference-scoped): [`RlmMaxDepthSource`](rlm-max-depth.ts.md#RlmMaxDepthSource)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`handleRlmMaxDepthCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleRlmMaxDepthCommand), [`getRlmMaxDepthStatus`](agent-session.ts.md#AgentSession.getRlmMaxDepthStatus), [`getRlmMaxDepthStatus`](../modes/agent-connection/types.ts.md#AgentConnection.getRlmMaxDepthStatus), [`SetRlmMaxDepthResult`](rlm-max-depth.ts.md#SetRlmMaxDepthResult)

### `SetRlmMaxDepthResult`
- def: [`packages/coding-agent/src/core/rlm-max-depth.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L10)
- signature: `interface SetRlmMaxDepthResult`
- members:
  - `globalError` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L12)
  - `globalSaved` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/rlm-max-depth.ts#L11)
- uses (calls/refs, reference-scoped): [`RlmMaxDepthStatus`](rlm-max-depth.ts.md#RlmMaxDepthStatus)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../modes/agent-connection/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-agent-connection-types.ts), [`setRlmMaxDepth`](agent-session.ts.md#AgentSession.setRlmMaxDepth), [`handleRlmMaxDepthCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleRlmMaxDepthCommand), [`global`](../modes/agent-connection/types.ts.md#AgentConnection.setRlmMaxDepth.options-typeLiteral140.global)  (1 test-only)

