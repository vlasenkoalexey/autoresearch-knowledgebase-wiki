---
title: 'Module: packages/ai/test/anthropic-eager-tool-input-e2e.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/anthropic-eager-tool-input-e2e.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`anthropic-eager-tool-input-e2e.test.ts`/
symbols:
  expectToolEnabledRequestAccepted: expectToolEnabledRequestAccepted().
  selectOneCasePerProvider: selectOneCasePerProvider().
  anthropicMessagesCases: anthropicMessagesCases.
  getAnthropicMessagesModels: getAnthropicMessagesModels().
  getProbePriority: getProbePriority().
  echoTool: echoTool.
  forcedEagerProbeCases: forcedEagerProbeCases.
  AnthropicEagerE2ECase.model: AnthropicEagerE2ECase#model.
  getE2EApiKey: getE2EApiKey().
  generatedCompatCases: generatedCompatCases.
  withEagerToolInputStreaming: withEagerToolInputStreaming().
  AnthropicEagerE2ECase.provider: AnthropicEagerE2ECase#provider.
  AnthropicEagerE2ECase: AnthropicEagerE2ECase#
  AnthropicEagerE2ECase.apiKey: AnthropicEagerE2ECase#apiKey.
  githubCopilotToken: githubCopilotToken.
  AnthropicEagerE2ECase.name: AnthropicEagerE2ECase#name.
  echoToolSchema: echoToolSchema.
---
# Module: [`packages/ai/test/anthropic-eager-tool-input-e2e.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts)

## Classes
### `AnthropicEagerE2ECase`
- def: [`packages/ai/test/anthropic-eager-tool-input-e2e.test.ts:21`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L21)
- signature: `interface AnthropicEagerE2ECase`
- members:
  - `apiKey` — [`L25`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L25)
  - `model` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L24)
  - `name` — [`L22`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L22)
  - `provider` — [`L23`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L23)
- uses (calls/refs, reference-scoped): [`Model`](../src/types.ts.md#Model), [`KnownProvider`](../src/types.ts.md#KnownProvider)
- used by: (4 test-only callers)

## Functions
- `expectToolEnabledRequestAccepted(model: Model<"anthropic-messages">, apiKey: string | undefined)` — [`L98`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L98)
- `getAnthropicMessagesModels(provider: KnownProvider)` — [`L35`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L35)
- `getE2EApiKey(provider: KnownProvider)` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L28)
- `getProbePriority(model: Model<"anthropic-messages">)` — [`L49`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L49)
- `selectOneCasePerProvider(cases: AnthropicEagerE2ECase[])` — [`L67`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L67)
- `withEagerToolInputStreaming(model: Model<"anthropic-messages">)` — [`L88`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L88)

## Module values
- `anthropicMessagesCases` — [`L40`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L40)
- `echoTool` — [`L15`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L15)
- `echoToolSchema` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L11)
- `forcedEagerProbeCases` — [`L84`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L84)
- `generatedCompatCases` — [`L83`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L83)
- `githubCopilotToken` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/anthropic-eager-tool-input-e2e.test.ts#L9)

