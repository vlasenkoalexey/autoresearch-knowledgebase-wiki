---
title: 'Module: packages/ai/src/models.ts'
type: catalog
provenance: extracted
module: packages/ai/src/models.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/`models.ts`/
symbols:
  getModel: getModel().
  calculateCost: calculateCost().
  getSupportedThinkingLevels: getSupportedThinkingLevels().
  clampThinkingLevel: clampThinkingLevel().
  getModels: getModels().
  modelsAreEqual: modelsAreEqual().
  supportsFastMode: supportsFastMode().
  getProviders: getProviders().
  modelRegistry: modelRegistry.
  ModelApi: ModelApi#
  EXTENDED_THINKING_LEVELS: EXTENDED_THINKING_LEVELS.
  CostOverrides: CostOverrides#
  CostOverrides.cacheWrite: CostOverrides#cacheWrite.
---
# Module: [`packages/ai/src/models.ts`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts)

## Classes
### `CostOverrides`
- def: [`packages/ai/src/models.ts:47`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L47)
- signature: `interface CostOverrides`
- members:
  - `cacheWrite` — [`L48`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L48)
- used by: [`calculateCost`](models.ts.md#calculateCost)

### `ModelApi`
- def: [`packages/ai/src/models.ts:15`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L15)
- signature: `type ModelApi`
- uses (calls/refs, reference-scoped): [`Api`](types.ts.md#Api), [`KnownProvider`](types.ts.md#KnownProvider), [`MODELS`](models.generated.ts.md#MODELS)
- used by: [`getModel`](models.ts.md#getModel), [`getModels`](models.ts.md#getModels)

## Functions
- `calculateCost(model: Model<TApi>, usage: Usage, overrides?: CostOverrides | undefined)` — [`L51`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L51)
- `clampThinkingLevel(model: Model<TApi>, level: ModelThinkingLevel)` — [`L77`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L77)
- `getModel(typeof MODELS)` — [`L20`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L20)
- `getModels(provider: TProvider)` — [`L32`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L32)
- `getProviders()` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L28)
- `getSupportedThinkingLevels(model: Model<TApi>)` — [`L66`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L66)
- `modelsAreEqual(a: Model<TApi> | null | undefined, b: Model<TApi> | null | undefined)` — [`L102`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L102) — Check if two models are equal by comparing both their id and provider.
- `supportsFastMode(model: Model<TApi>)` — [`L39`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L39)

## Module values
- `EXTENDED_THINKING_LEVELS` — [`L64`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L64)
- `modelRegistry` — [`L4`](../../../../../../../raw/code/prime-agent/packages/ai/src/models.ts#L4)

