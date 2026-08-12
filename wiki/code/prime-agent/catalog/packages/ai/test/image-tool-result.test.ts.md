---
title: 'Module: packages/ai/test/image-tool-result.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/image-tool-result.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`image-tool-result.test.ts`/
symbols:
  handleToolWithImageResult: handleToolWithImageResult().
  handleToolWithTextAndImageResult: handleToolWithTextAndImageResult().
  oauthTokens: oauthTokens.
  StreamOptionsWithExtras: StreamOptionsWithExtras#
---
# Module: [`packages/ai/test/image-tool-result.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/image-tool-result.test.ts)

## Classes
### `StreamOptionsWithExtras`
- def: [`packages/ai/test/image-tool-result.test.ts:10`](../../../../../../../raw/code/prime-agent/packages/ai/test/image-tool-result.test.ts#L10)
- signature: `type StreamOptionsWithExtras`
- uses (calls/refs, reference-scoped): [`StreamOptions`](../src/types.ts.md#StreamOptions)
- used by: (2 test-only callers)

## Functions
- `handleToolWithImageResult(model: Model<TApi>, options?: StreamOptionsWithExtras | undefined)` — [`L31`](../../../../../../../raw/code/prime-agent/packages/ai/test/image-tool-result.test.ts#L31) — Test that tool results containing only images work correctly across all providers.
- `handleToolWithTextAndImageResult(model: Model<TApi>, options?: StreamOptionsWithExtras | undefined)` — [`L119`](../../../../../../../raw/code/prime-agent/packages/ai/test/image-tool-result.test.ts#L119) — Test that tool results containing both text and images work correctly across all providers.

## Module values
- `oauthTokens` — [`L17`](../../../../../../../raw/code/prime-agent/packages/ai/test/image-tool-result.test.ts#L17)

