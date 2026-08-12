---
title: 'Module: packages/ai/test/google-thinking-disable.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/google-thinking-disable.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`google-thinking-disable.test.ts`/
symbols:
  expectThinkingDisabledE2E: expectThinkingDisabledE2E().
  runWithoutReasoning: runWithoutReasoning().
  makeContext: makeContext().
  SimpleOptionsWithExtras: SimpleOptionsWithExtras#
  DisableExpectations.requestOptions: DisableExpectations#requestOptions.
  DisableExpectations.maxOutputTokens: DisableExpectations#maxOutputTokens.
  RunResult: RunResult#
  RunResult.thinkingEventCount: RunResult#thinkingEventCount.
  RunResult.thinkingCharCount: RunResult#thinkingCharCount.
  RunResult.text: RunResult#text.
  RunResult.outputTokens: RunResult#outputTokens.
  RunResult.contentTypes: RunResult#contentTypes.
  DisableExpectations: DisableExpectations#
  DisableExpectations.minPongs: DisableExpectations#minPongs.
  countPongs: countPongs().
---
# Module: [`packages/ai/test/google-thinking-disable.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts)

## Classes
### `DisableExpectations`
- def: [`packages/ai/test/google-thinking-disable.test.ts:16`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L16)
- signature: `interface DisableExpectations`
- members:
  - `maxOutputTokens` — [`L19`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L19)
  - `minPongs` — [`L18`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L18)
  - `requestOptions` — [`L17`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L17)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `RunResult`
- def: [`packages/ai/test/google-thinking-disable.test.ts:8`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L8)
- signature: `interface RunResult`
- members:
  - `contentTypes` — [`L13`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L13)
  - `outputTokens` — [`L12`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L12)
  - `text` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L11)
  - `thinkingCharCount` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L10)
  - `thinkingEventCount` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L9)
- used by: (2 test-only callers)

### `SimpleOptionsWithExtras`
- def: [`packages/ai/test/google-thinking-disable.test.ts:6`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L6)
- signature: `type SimpleOptionsWithExtras`
- uses (calls/refs, reference-scoped): [`SimpleStreamOptions`](../src/types.ts.md#SimpleStreamOptions)
- used by: (3 test-only callers)

## Functions
- `countPongs(text: string)` — [`L36`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L36)
- `expectThinkingDisabledE2E(model: Model<TApi>, expectations?: DisableExpectations)` — [`L81`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L81)
- `makeContext()` — [`L22`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L22)
- `runWithoutReasoning(model: Model<TApi>, options?: SimpleOptionsWithExtras)` — [`L40`](../../../../../../../raw/code/prime-agent/packages/ai/test/google-thinking-disable.test.ts#L40)

