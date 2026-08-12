---
title: 'Module: packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/extensions/builtin/`herdr-agent-state.ts`/
symbols:
  herdrAgentStateExtensionImpl: herdrAgentStateExtensionImpl().
  herdrAgentStateExtension: herdrAgentStateExtension.
  createHerdrAgentStateExtension: createHerdrAgentStateExtension().
  hasFileBasedHerdrIntegration: hasFileBasedHerdrIntegration().
  nextReportSeq: nextReportSeq().
  AgentState: AgentState#
  QueuedState.state: QueuedState#state.
  errorHoldMessage: errorHoldMessage().
  reportSeq: reportSeq.
  parseDurationEnv: parseDurationEnv().
  QueuedState: QueuedState#
  QueuedState.message: QueuedState#message.
  QueuedState.seq: QueuedState#seq.
  lastAssistantMessage: lastAssistantMessage().
---
# Module: [`packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts)

## Classes
### `AgentState`
- def: [`packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts:23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L23)
- signature: `type AgentState`
- used by: [`herdrAgentStateExtensionImpl`](herdr-agent-state.ts.md#herdrAgentStateExtensionImpl), [`state`](herdr-agent-state.ts.md#QueuedState.state)

### `QueuedState`
- def: [`packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts:45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L45)
- signature: `interface QueuedState`
- members:
  - `message` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L47)
  - `seq` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L48)
  - `state` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L46)
- uses (calls/refs, reference-scoped): [`AgentState`](herdr-agent-state.ts.md#AgentState)
- used by: [`herdrAgentStateExtensionImpl`](herdr-agent-state.ts.md#herdrAgentStateExtensionImpl)

## Functions
- `createHerdrAgentStateExtension(getLoadedExtensionPaths: () => string[])` — [`L113`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L113) — Build the built-in Herdr reporter factory. `getLoadedExtensionPaths`
- `errorHoldMessage(event: any)` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L83) — Error message of the turn's final assistant message, if it ended in error.
- `hasFileBasedHerdrIntegration(loadedExtensionPaths: string[])` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L38) — True when Herdr's own file-based Pi integration (`herdr integration
- `herdrAgentStateExtensionImpl(pi: ExtensionAPI, getLoadedExtensionPaths: () => string[])` — [`L124`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L124)
- `lastAssistantMessage(messages: unknown[])` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L63)
- `nextReportSeq()` — [`L99`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L99)
- `parseDurationEnv(name: string, fallback: number)` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L51)

## Module values
- `herdrAgentStateExtension` — [`L120`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L120) — Built-in reporter with no file-based deferral, for tests and embedders.
- `reportSeq` — [`L97`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/builtin/herdr-agent-state.ts#L97)

