---
title: 'Module: packages/coding-agent/test/interactive-mode-traces-command.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/interactive-mode-traces-command.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`interactive-mode-traces-command.test.ts`/
symbols:
  makeContext: makeContext().
  prototype: prototype.
  TracesCommandContext.uploadCurrentTraceOnce: TracesCommandContext#uploadCurrentTraceOnce.
  TracesCommandContext.uploadAllTraces: TracesCommandContext#uploadAllTraces.
  TracesCommandContext.showStatus: TracesCommandContext#showStatus.
  TracesCommandPrototype.handleTracesCommand: TracesCommandPrototype#handleTracesCommand().
  TracesCommandContext.modelRegistry.typeLiteral8.authStorage: TracesCommandContext#modelRegistry.typeLiteral8:authStorage.
  TracesCommandContext.formatTraceUploadResult: TracesCommandContext#formatTraceUploadResult.
  TracesCommandPrototype: TracesCommandPrototype#
  TracesCommandContext.traceUploadAllAbortController: TracesCommandContext#traceUploadAllAbortController.
  TracesCommandContext: TracesCommandContext#
  TracesCommandContext.settingsManager: TracesCommandContext#settingsManager.
  TracesCommandContext.settingsManager.typeLiteral5.setAgentTracesEnabled: TracesCommandContext#settingsManager.typeLiteral5:setAgentTracesEnabled.
  TracesCommandContext.previewCurrentTrace: TracesCommandContext#previewCurrentTrace.
  TracesCommandContext.agentConnection: TracesCommandContext#agentConnection.
  TracesCommandContext.agentConnection.typeLiteral0.getState: TracesCommandContext#agentConnection.typeLiteral0:getState.
  TracesCommandContext.settingsManager.typeLiteral5.getAgentTracesEnabled: TracesCommandContext#settingsManager.typeLiteral5:getAgentTracesEnabled.
  TracesCommandContext.settingsManager.typeLiteral5.flush: TracesCommandContext#settingsManager.typeLiteral5:flush.
  TracesCommandContext.modelRegistry: TracesCommandContext#modelRegistry.
  TracesCommandContext.showWarning: TracesCommandContext#showWarning.
  TracesCommandContext.showError: TracesCommandContext#showError.
---
# Module: [`packages/coding-agent/test/interactive-mode-traces-command.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts)

## Classes
### `TracesCommandContext`
- def: [`packages/coding-agent/test/interactive-mode-traces-command.test.ts:7`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L7)
- signature: `interface TracesCommandContext`
- members:
  - `agentConnection` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L9)
  - `authStorage` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L15)
  - `flush` — [`L13`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L13)
  - `formatTraceUploadResult` — [`L19`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L19)
  - `getAgentTracesEnabled` — [`L11`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L11)
  - `getState` — [`L9`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L9)
  - `modelRegistry` — [`L15`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L15)
  - `previewCurrentTrace` — [`L16`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L16)
  - `setAgentTracesEnabled` — [`L12`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L12)
  - `settingsManager` — [`L10`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L10)
  - `showError` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L22)
  - `showStatus` — [`L20`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L20)
  - `showWarning` — [`L21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L21)
  - `traceUploadAllAbortController` — [`L8`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L8)
  - `uploadAllTraces` — [`L18`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L18)
  - `uploadCurrentTraceOnce` — [`L17`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L17)
- uses (calls/refs, reference-scoped): [`AuthStorage`](../src/core/auth-storage.ts.md#AuthStorage), [`AgentTraceUploadResult`](../src/core/agent-traces.ts.md#AgentTraceUploadResult), [`AgentTraceUploadAllResult`](../src/core/agent-traces.ts.md#AgentTraceUploadAllResult)
- used by: (3 test-only callers)

### `TracesCommandPrototype`
- def: [`packages/coding-agent/test/interactive-mode-traces-command.test.ts:25`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L25)
- signature: `interface TracesCommandPrototype`
- members:
  - `handleTracesCommand(method)` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L26)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

## Functions
- `makeContext(enabled?: boolean)` — [`L31`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L31)

## Module values
- `prototype` — [`L29`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/interactive-mode-traces-command.test.ts#L29)

