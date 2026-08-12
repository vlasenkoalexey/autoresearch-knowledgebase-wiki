---
title: 'Module: packages/ai/src/providers/google.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/google.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`google.ts`/
symbols:
  streamGoogle: streamGoogle.
  streamSimpleGoogle: streamSimpleGoogle.
  buildParams: buildParams().
  GoogleOptions: GoogleOptions#
  getThinkingLevel: getThinkingLevel().
  getDisabledThinkingConfig: getDisabledThinkingConfig().
  GoogleOptions.thinking: GoogleOptions#thinking.
  createClient: createClient().
  isGemma4Model: isGemma4Model().
  isGemini3ProModel: isGemini3ProModel().
  isGemini3FlashModel: isGemini3FlashModel().
  GoogleOptions.thinking.typeLiteral0.level: GoogleOptions#thinking.typeLiteral0:level.
  ClampedThinkingLevel: ClampedThinkingLevel#
  GoogleOptions.toolChoice: GoogleOptions#toolChoice.
  GoogleOptions.thinking.typeLiteral0.enabled: GoogleOptions#thinking.typeLiteral0:enabled.
  GoogleOptions.thinking.typeLiteral0.budgetTokens: GoogleOptions#thinking.typeLiteral0:budgetTokens.
  toolCallCounter: toolCallCounter.
---
# Module: [`packages/ai/src/providers/google.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts)

## Classes
### `ClampedThinkingLevel`
- def: [`packages/ai/src/providers/google.ts:405`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L405)
- signature: `type ClampedThinkingLevel`
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../types.ts.md#ThinkingLevel)
- used by: [`streamSimpleGoogle`](google.ts.md#streamSimpleGoogle), [`getThinkingLevel`](google.ts.md#getThinkingLevel)

### `GoogleOptions`
- def: [`packages/ai/src/providers/google.ts:41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L41)
- signature: `interface GoogleOptions`
- members:
  - `budgetTokens` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L45)
  - `enabled` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L44)
  - `level` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L46)
  - `thinking` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L43)
  - `toolChoice` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L42)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions), [`GoogleThinkingLevel`](google-shared.ts.md#GoogleThinkingLevel)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamGoogle`](google.ts.md#streamGoogle), [`google.ts`](google.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`streamSimpleGoogle`](google.ts.md#streamSimpleGoogle), [`buildParams`](google.ts.md#buildParams), [`loadGoogleProviderModule`](register-builtins.ts.md#loadGoogleProviderModule), [`googleProviderModulePromise`](register-builtins.ts.md#googleProviderModulePromise), [`streamGoogle`](register-builtins.ts.md#GoogleProviderModule.streamGoogle)

## Functions
- `buildParams(model: Model<"google-generative-ai">, context: Context, options?: GoogleOptions)` — [`L345`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L345)
- `createClient(model: Model<"google-generative-ai">, apiKey?: string | undefined, optionsHeaders?: Record<string, string> | undefined)` — [`L325`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L325)
- `getDisabledThinkingConfig(model: Model<"google-generative-ai">)` — [`L419`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L419)
- `getThinkingLevel(effort: ClampedThinkingLevel, model: Model<"google-generative-ai">)` — [`L437`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L437)
- `isGemini3FlashModel(model: Model<"google-generative-ai">)` — [`L415`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L415)
- `isGemini3ProModel(model: Model<"google-generative-ai">)` — [`L411`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L411)
- `isGemma4Model(model: Model<"google-generative-ai">)` — [`L407`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L407)

## Module values
- `streamGoogle` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L53)
- `streamSimpleGoogle` — [`L287`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L287)
- `toolCallCounter` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google.ts#L51)

