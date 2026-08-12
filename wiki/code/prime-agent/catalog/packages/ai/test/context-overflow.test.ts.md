---
title: 'Module: packages/ai/test/context-overflow.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/context-overflow.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`context-overflow.test.ts`/
symbols:
  testContextOverflow: testContextOverflow().
  logResult: logResult().
  OverflowResult.response: OverflowResult#response.
  OverflowResult.stopReason: OverflowResult#stopReason.
  OverflowResult.errorMessage: OverflowResult#errorMessage.
  OverflowResult.usage: OverflowResult#usage.
  oauthTokens: oauthTokens.
  generateOverflowContent: generateOverflowContent().
  OverflowResult.hasUsageData: OverflowResult#hasUsageData.
  LOREM_IPSUM: LOREM_IPSUM.
  OverflowResult: OverflowResult#
  OverflowResult.provider: OverflowResult#provider.
  OverflowResult.model: OverflowResult#model.
  OverflowResult.contextWindow: OverflowResult#contextWindow.
---
# Module: [`packages/ai/test/context-overflow.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts)

## Classes
### `OverflowResult`
- def: [`packages/ai/test/context-overflow.test.ts:43`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L43)
- signature: `interface OverflowResult`
- members:
  - `contextWindow` — [`L46`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L46)
  - `errorMessage` — [`L48`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L48)
  - `hasUsageData` — [`L50`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L50)
  - `model` — [`L45`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L45)
  - `provider` — [`L44`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L44)
  - `response` — [`L51`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L51)
  - `stopReason` — [`L47`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L47)
  - `usage` — [`L49`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L49)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../src/types.ts.md#AssistantMessage), [`Usage`](../src/types.ts.md#Usage)
- used by: (3 test-only callers)

## Functions
- `generateOverflowContent(contextWindow: number)` — [`L36`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L36)
- `logResult(result: OverflowResult)` — [`L84`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L84)
- `testContextOverflow(model: Model<any>, apiKey: string)` — [`L54`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L54)

## Module values
- `LOREM_IPSUM` — [`L32`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L32)
- `oauthTokens` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/test/context-overflow.test.ts#L28)

