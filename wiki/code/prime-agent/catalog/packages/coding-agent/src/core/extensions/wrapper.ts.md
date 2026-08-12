---
title: 'Module: packages/coding-agent/src/core/extensions/wrapper.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/extensions/wrapper.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/extensions/`wrapper.ts`/
symbols:
  wrapRegisteredTools: wrapRegisteredTools().
  wrapRegisteredTool: wrapRegisteredTool().
  toRunnerGetter: toRunnerGetter().
  RunnerSource: RunnerSource#
---
# Module: [`packages/coding-agent/src/core/extensions/wrapper.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/wrapper.ts)

## Classes
### `RunnerSource`
- def: [`packages/coding-agent/src/core/extensions/wrapper.ts:13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/wrapper.ts#L13)
- signature: `type RunnerSource`
- uses (calls/refs, reference-scoped): [`ExtensionRunner`](runner.ts.md#ExtensionRunner)
- used by: [`wrapRegisteredTools`](wrapper.ts.md#wrapRegisteredTools), [`wrapRegisteredTool`](wrapper.ts.md#wrapRegisteredTool), [`toRunnerGetter`](wrapper.ts.md#toRunnerGetter)

## Functions
- `toRunnerGetter(source: RunnerSource)` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/wrapper.ts#L15)
- `wrapRegisteredTool(registeredTool: RegisteredTool, runner: RunnerSource)` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/wrapper.ts#L23) — Wrap a RegisteredTool into an AgentTool.
- `wrapRegisteredTools(registeredTools: RegisteredTool[], runner: RunnerSource)` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/extensions/wrapper.ts#L32) — Wrap all registered tools into AgentTools.

