---
title: 'Module: packages/ai/test/anthropic-long-cache-retention-e2e.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/anthropic-long-cache-retention-e2e.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`anthropic-long-cache-retention-e2e.test.ts`/
symbols:
  expectLongCacheRetentionAccepted: expectLongCacheRetentionAccepted().
  selectOneCasePerProvider: selectOneCasePerProvider().
  getAnthropicMessagesModels: getAnthropicMessagesModels().
  anthropicMessagesCases: anthropicMessagesCases.
  getProbePriority: getProbePriority().
  getE2EApiKey: getE2EApiKey().
  AnthropicLongCacheRetentionE2ECase.model: AnthropicLongCacheRetentionE2ECase#model.
  probeCases: probeCases.
  withLongCacheRetention: withLongCacheRetention().
  AnthropicLongCacheRetentionE2ECase.provider: AnthropicLongCacheRetentionE2ECase#provider.
  AnthropicLongCacheRetentionE2ECase: AnthropicLongCacheRetentionE2ECase#
  githubCopilotToken: githubCopilotToken.
  AnthropicLongCacheRetentionE2ECase.name: AnthropicLongCacheRetentionE2ECase#name.
  AnthropicLongCacheRetentionE2ECase.apiKey: AnthropicLongCacheRetentionE2ECase#apiKey.
---
# Module: [`packages/ai/test/anthropic-long-cache-retention-e2e.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts)

## Classes
### `AnthropicLongCacheRetentionE2ECase`
- def: [`packages/ai/test/anthropic-long-cache-retention-e2e.test.ts:10`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L10)
- signature: `interface AnthropicLongCacheRetentionE2ECase`
- members:
  - `apiKey` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L14)
  - `model` — [`L13`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L13)
  - `name` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L11)
  - `provider` — [`L12`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L12)
- uses (calls/refs, reference-scoped): [`Model`](../src/types.ts.md#Model), [`KnownProvider`](../src/types.ts.md#KnownProvider)
- used by: (3 test-only callers)

## Functions
- `expectLongCacheRetentionAccepted(model: Model<"anthropic-messages">, apiKey: string | undefined)` — [`L82`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L82)
- `getAnthropicMessagesModels(provider: KnownProvider)` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L24)
- `getE2EApiKey(provider: KnownProvider)` — [`L17`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L17)
- `getProbePriority(model: Model<"anthropic-messages">)` — [`L38`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L38)
- `selectOneCasePerProvider(cases: AnthropicLongCacheRetentionE2ECase[])` — [`L54`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L54)
- `withLongCacheRetention(model: Model<"anthropic-messages">)` — [`L72`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L72)

## Module values
- `anthropicMessagesCases` — [`L29`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L29)
- `githubCopilotToken` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L8)
- `probeCases` — [`L70`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-long-cache-retention-e2e.test.ts#L70)

