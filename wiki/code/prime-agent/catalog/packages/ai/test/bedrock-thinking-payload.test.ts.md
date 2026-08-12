---
title: 'Module: packages/ai/test/bedrock-thinking-payload.test.ts'
type: catalog
provenance: extracted
module: packages/ai/test/bedrock-thinking-payload.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`bedrock-thinking-payload.test.ts`/
symbols:
  makeContext: makeContext().
  capturePayload: capturePayload().
  BedrockThinkingPayload.additionalModelRequestFields: BedrockThinkingPayload#additionalModelRequestFields.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.thinking: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:thinking.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.output_config: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:output_config.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.anthropic_beta: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:anthropic_beta.
  BedrockThinkingPayload: BedrockThinkingPayload#
  BedrockThinkingPayload.inferenceConfig: BedrockThinkingPayload#inferenceConfig.
  BedrockThinkingPayload.inferenceConfig.typeLiteral0.temperature: BedrockThinkingPayload#inferenceConfig.typeLiteral0:temperature.
  BedrockThinkingPayload.inferenceConfig.typeLiteral0.maxTokens: BedrockThinkingPayload#inferenceConfig.typeLiteral0:maxTokens.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.thinking.typeLiteral2.type: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:thinking.typeLiteral2:type.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.thinking.typeLiteral2.budget_tokens: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:thinking.typeLiteral2:budget_tokens.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.thinking.typeLiteral2.display: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:thinking.typeLiteral2:display.
  BedrockThinkingPayload.additionalModelRequestFields.typeLiteral1.output_config.typeLiteral3.effort: BedrockThinkingPayload#additionalModelRequestFields.typeLiteral1:output_config.typeLiteral3:effort.
---
# Module: [`packages/ai/test/bedrock-thinking-payload.test.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts)

## Classes
### `BedrockThinkingPayload`
- def: [`packages/ai/test/bedrock-thinking-payload.test.ts:6`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L6)
- signature: `interface BedrockThinkingPayload`
- members:
  - `additionalModelRequestFields` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L8)
  - `anthropic_beta` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L11)
  - `budget_tokens` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L9)
  - `display` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L9)
  - `effort` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L10)
  - `inferenceConfig` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L7)
  - `maxTokens` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L7)
  - `output_config` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L10)
  - `temperature` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L7)
  - `thinking` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L9)
  - `type` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L9)
- used by: (2 test-only callers)

## Functions
- `capturePayload(model: Model<"bedrock-converse-stream">, options?: BedrockOptions | undefined)` — [`L21`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L21)
- `makeContext()` — [`L15`](../../../../../../../raw/code/prime-agent/packages/ai/test/bedrock-thinking-payload.test.ts#L15)

