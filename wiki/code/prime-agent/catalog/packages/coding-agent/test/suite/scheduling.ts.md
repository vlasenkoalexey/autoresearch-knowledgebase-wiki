---
title: 'Module: packages/coding-agent/test/suite/scheduling.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/scheduling.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`scheduling.ts`/
symbols:
  createDeferred: createDeferred().
  Deferred.promise: Deferred#promise.
  Deferred.resolve: Deferred#resolve.
  createWaitingHarness: createWaitingHarness().
  withStreaming: withStreaming().
  gatedHook.typeLiteral22.runs: gatedHook().typeLiteral22:runs.
  gatedHook.typeLiteral22.factory: gatedHook().typeLiteral22:factory.
  gatedHook: gatedHook().
  gatedHook.typeLiteral22.reached: gatedHook().typeLiteral22:reached.
  gatedHook.typeLiteral22.release: gatedHook().typeLiteral22:release.
  WaitingHarness.harness: WaitingHarness#harness.
  WaitingHarness.releaseToolExecution: WaitingHarness#releaseToolExecution.
  WaitingHarness.promptPromise: WaitingHarness#promptPromise.
  WaitingHarness.waitForToolStart: WaitingHarness#waitForToolStart.
  Deferred: Deferred#
  createWaitingHarness.options-typeLiteral47.tools: createWaitingHarness().(options)typeLiteral47:tools.
  Deferred.reject: Deferred#reject.
  gatedHook.options-typeLiteral21.prompt: gatedHook().(options)typeLiteral21:prompt.
  WaitingHarness: WaitingHarness#
  createWaitingHarness.options-typeLiteral47.extensionFactories: createWaitingHarness().(options)typeLiteral47:extensionFactories.
---
# Module: [`packages/coding-agent/test/suite/scheduling.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts)

## Classes
### `Deferred`
- def: [`packages/coding-agent/test/suite/scheduling.ts:7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L7)
- doc: A promise with its resolve/reject functions exposed.
- signature: `interface Deferred`
- members:
  - `promise` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L8)
  - `reject` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L10)
  - `resolve` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L9)
- used by: (10 test-only callers)

### `WaitingHarness`
- def: [`packages/coding-agent/test/suite/scheduling.ts:57`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L57)
- signature: `interface WaitingHarness`
- members:
  - `harness` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L58)
  - `promptPromise` — [`L60`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L60)
  - `releaseToolExecution` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L59)
  - `waitForToolStart` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L61)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (3 test-only callers)

## Functions
- `createDeferred()` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L13)
- `createWaitingHarness(options?: { tools?: AgentTool<TSchema, any>[] | undefined; extensionFactories?: ((pi: ExtensionAPI) => void)[] | undefined; })` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L68) — Harness whose first turn calls a gated "wait" tool: the run stays streaming
- `gatedHook(options?: { prompt?: string | undefined; })` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L28) — A before_agent_start gate as an extension factory: `reached` resolves when the
- `withStreaming(harness: Harness, on: boolean)` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L53) — Force the harness agent's streaming flag, replacing the `as { isStreaming: boolean }` cast idiom.

## Module values
- `extensionFactories` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L69)
- `factory` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L29)
- `prompt` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L28)
- `reached` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L30)
- `release` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L31)
- `runs` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L32)
- `tools` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/scheduling.ts#L69)

