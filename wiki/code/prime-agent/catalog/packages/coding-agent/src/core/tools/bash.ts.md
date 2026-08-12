---
title: 'Module: packages/coding-agent/src/core/tools/bash.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/tools/bash.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/tools/`bash.ts`/
symbols:
  createBashToolDefinition: createBashToolDefinition().
  rebuildBashResultRenderComponent.result-typeLiteral96.details: rebuildBashResultRenderComponent().(result)typeLiteral96:details.
  createBashTool: createBashTool().
  createLocalBashOperations: createLocalBashOperations().
  BashOperations: BashOperations#
  formatBashCall: formatBashCall().
  BashOperations.exec: BashOperations#exec.
  resolveSpawnContext: resolveSpawnContext().
  BashResultRenderComponent: BashResultRenderComponent#
  BashToolDetails: BashToolDetails#
  BashResultRenderState.typeLiteral73.cachedSkipped: BashResultRenderState#typeLiteral73:cachedSkipped.
  BashToolInput: BashToolInput#
  BashSpawnHook: BashSpawnHook#
  BashSpawnContext: BashSpawnContext#
  BashResultRenderState.typeLiteral73.cachedLines: BashResultRenderState#typeLiteral73:cachedLines.
  bashSchema: bashSchema.
  BashRenderState.typeLiteral72.interval: BashRenderState#typeLiteral72:interval.
  BashToolDetails.truncation: BashToolDetails#truncation.
  BashSpawnContext.command: BashSpawnContext#command.
  BashSpawnContext.cwd: BashSpawnContext#cwd.
  BashSpawnContext.env: BashSpawnContext#env.
  BashToolOptions: BashToolOptions#
  BashRenderState.typeLiteral72.startedAt: BashRenderState#typeLiteral72:startedAt.
  BashResultRenderState.typeLiteral73.cachedWidth: BashResultRenderState#typeLiteral73:cachedWidth.
  BashToolOptions.operations: BashToolOptions#operations.
  BashToolOptions.spawnHook: BashToolOptions#spawnHook.
  rebuildBashResultRenderComponent: rebuildBashResultRenderComponent().
  BashRenderState.typeLiteral72.endedAt: BashRenderState#typeLiteral72:endedAt.
  BashRenderState: BashRenderState#
  BashToolDetails.fullOutputPath: BashToolDetails#fullOutputPath.
  createLocalBashOperations.options-typeLiteral26.shellPath: createLocalBashOperations().(options)typeLiteral26:shellPath.
  BashToolOptions.commandPrefix: BashToolOptions#commandPrefix.
  BashToolOptions.shellPath: BashToolOptions#shellPath.
  BASH_PREVIEW_LINES: BASH_PREVIEW_LINES.
  BASH_UPDATE_THROTTLE_MS: BASH_UPDATE_THROTTLE_MS.
  BashResultRenderState: BashResultRenderState#
  BashResultRenderComponent.state: BashResultRenderComponent#state.
  formatDuration: formatDuration().
  rebuildBashResultRenderComponent.result-typeLiteral96.content: rebuildBashResultRenderComponent().(result)typeLiteral96:content.
  rebuildBashResultRenderComponent.result-typeLiteral96.content.Array.typeLiteral97.type: rebuildBashResultRenderComponent().(result)typeLiteral96:content.Array:typeLiteral97:type.
  rebuildBashResultRenderComponent.result-typeLiteral96.content.Array.typeLiteral97.text: rebuildBashResultRenderComponent().(result)typeLiteral96:content.Array:typeLiteral97:text.
  rebuildBashResultRenderComponent.result-typeLiteral96.content.Array.typeLiteral97.data: rebuildBashResultRenderComponent().(result)typeLiteral96:content.Array:typeLiteral97:data.
  rebuildBashResultRenderComponent.result-typeLiteral96.content.Array.typeLiteral97.mimeType: rebuildBashResultRenderComponent().(result)typeLiteral96:content.Array:typeLiteral97:mimeType.
---
# Module: [`packages/coding-agent/src/core/tools/bash.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts)

## Classes
### `BashOperations`
- def: [`packages/coding-agent/src/core/tools/bash.ts:40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L40)
- doc: Pluggable operations for the bash tool.
- signature: `interface BashOperations`
- members:
  - `exec` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L48) — Execute a command and stream output.
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`createLocalBashOperations`](bash.ts.md#createLocalBashOperations), [`executeBashWithOperations`](../bash-executor.ts.md#executeBashWithOperations), [`bash-executor.ts`](../bash-executor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-bash-executor.ts), [`operations`](../agent-session.ts.md#AgentSession.executeBash.options-typeLiteral4128.operations), [`operations`](../extensions/types.ts.md#UserBashEventResult.operations), [`operations`](bash.ts.md#BashToolOptions.operations)  (8 test-only)

### `BashRenderState`
- def: [`packages/coding-agent/src/core/tools/bash.ts:157`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L157)
- signature: `type BashRenderState`
- members:
  - `endedAt` — [`L159`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L159)
  - `interval` — [`L160`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L160)
  - `startedAt` — [`L158`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L158)
- used by: [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition)

### `BashResultRenderComponent`  ·  implements/extends Component, Container
- def: [`packages/coding-agent/src/core/tools/bash.ts:169`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L169)
- signature: `class BashResultRenderComponent`
- members:
  - `state` — [`L170`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L170)
- uses (calls/refs, reference-scoped): [`Container`](../../../../tui/src/tui.ts.md#Container), [`cachedSkipped`](bash.ts.md#BashResultRenderState.typeLiteral73.cachedSkipped), [`cachedLines`](bash.ts.md#BashResultRenderState.typeLiteral73.cachedLines), [`cachedWidth`](bash.ts.md#BashResultRenderState.typeLiteral73.cachedWidth), [`BashResultRenderState`](bash.ts.md#BashResultRenderState)
- used by: [`Component`](../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../tui/src/tui.ts.md#Container), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`details`](bash.ts.md#rebuildBashResultRenderComponent.result-typeLiteral96.details), [`rebuildBashResultRenderComponent`](bash.ts.md#rebuildBashResultRenderComponent)

### `BashResultRenderState`
- def: [`packages/coding-agent/src/core/tools/bash.ts:163`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L163)
- signature: `type BashResultRenderState`
- members:
  - `cachedLines` — [`L165`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L165)
  - `cachedSkipped` — [`L166`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L166)
  - `cachedWidth` — [`L164`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L164)
- used by: [`details`](bash.ts.md#rebuildBashResultRenderComponent.result-typeLiteral96.details), [`BashResultRenderComponent`](bash.ts.md#BashResultRenderComponent)

### `BashSpawnContext`
- def: [`packages/coding-agent/src/core/tools/bash.ts:130`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L130)
- signature: `interface BashSpawnContext`
- members:
  - `command` — [`L131`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L131)
  - `cwd` — [`L132`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L132)
  - `env` — [`L133`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L133)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`resolveSpawnContext`](bash.ts.md#resolveSpawnContext), [`BashSpawnHook`](bash.ts.md#BashSpawnHook)  (1 test-only)

### `BashSpawnHook`
- def: [`packages/coding-agent/src/core/tools/bash.ts:136`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L136)
- signature: `type BashSpawnHook`
- uses (calls/refs, reference-scoped): [`BashSpawnContext`](bash.ts.md#BashSpawnContext)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`resolveSpawnContext`](bash.ts.md#resolveSpawnContext), [`spawnHook`](bash.ts.md#BashToolOptions.spawnHook)

### `BashToolDetails`
- def: [`packages/coding-agent/src/core/tools/bash.ts:31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L31)
- signature: `interface BashToolDetails`
- members:
  - `fullOutputPath` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L33)
  - `truncation` — [`L32`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L32)
- uses (calls/refs, reference-scoped): [`TruncationResult`](truncate.ts.md#TruncationResult)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`details`](bash.ts.md#rebuildBashResultRenderComponent.result-typeLiteral96.details), [`BashToolResultEvent`](../extensions/types.ts.md#BashToolResultEvent)  (1 test-only)

### `BashToolInput`
- def: [`packages/coding-agent/src/core/tools/bash.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L29)
- signature: `type BashToolInput`
- uses (calls/refs, reference-scoped): [`bashSchema`](bash.ts.md#bashSchema)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`types.ts`](../extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`BashToolCallEvent`](../extensions/types.ts.md#BashToolCallEvent)

### `BashToolOptions`
- def: [`packages/coding-agent/src/core/tools/bash.ts:143`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L143)
- signature: `interface BashToolOptions`
- members:
  - `commandPrefix` — [`L147`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L147) — Command prefix prepended to every command (for example shell setup commands)
  - `operations` — [`L145`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L145) — Custom operations for command execution. Default: local shell
  - `shellPath` — [`L149`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L149) — Optional explicit shell path from settings
  - `spawnHook` — [`L151`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L151) — Hook to adjust command, cwd, or env before execution
- uses (calls/refs, reference-scoped): [`BashOperations`](bash.ts.md#BashOperations), [`BashSpawnHook`](bash.ts.md#BashSpawnHook)
- used by: [`index.ts`](../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`createBashToolDefinition`](bash.ts.md#createBashToolDefinition), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-index.ts), [`createBashTool`](bash.ts.md#createBashTool)

## Functions
- `createBashTool(cwd: string, options?: BashToolOptions | undefined)` — [`L453`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L453)
- `createBashToolDefinition(cwd: string, options?: BashToolOptions | undefined)` — [`L276`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L276)
- `createLocalBashOperations(options?: { shellPath?: string | undefined; } | undefined)` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L66) — Create bash operations using pi's built-in local shell execution backend.
- `formatBashCall(args: { command?: string | undefined; timeout?: number | undefined; } | undefined)` — [`L181`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L181)
- `formatDuration(ms: number)` — [`L177`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L177)
- `rebuildBashResultRenderComponent(component: BashResultRenderComponent, result: { content: { type: string; text?: string | undefined; data?: string | undefined; mimeType?: string | undefined; }[]; details?: BashToolDetails | undefined; }, options: ToolRenderResultOptions, showImages: boolean, includeImageDimensions: boolean, showExpandHint: boolean, startedAt: number | undefined, endedAt: number | undefined)` — [`L198`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L198)
- `resolveSpawnContext(command: string, cwd: string, spawnHook?: BashSpawnHook | undefined)` — [`L138`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L138)

## Module values
- `BASH_PREVIEW_LINES` — [`L154`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L154)
- `BASH_UPDATE_THROTTLE_MS` — [`L155`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L155)
- `bashSchema` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L24)
- `content` — [`L201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L201)
- `data` — [`L201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L201)
- `details` — [`L202`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L202)
- `mimeType` — [`L201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L201)
- `shellPath` — [`L66`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L66)
- `text` — [`L201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L201)
- `type` — [`L201`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/tools/bash.ts#L201)

