---
title: 'Module: packages/coding-agent/src/core/prime-inference-model-selection.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/prime-inference-model-selection.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`prime-inference-model-selection.ts`/
symbols:
  resolvePrimeInferencePostLoginModelAction: resolvePrimeInferencePostLoginModelAction().
  PrimeInferencePostLoginModelAction: PrimeInferencePostLoginModelAction#
  PrimeInferencePostLoginModelAction.openModelPicker: PrimeInferencePostLoginModelAction#openModelPicker.
  PrimeInferencePostLoginModelAction.fallbackModel: PrimeInferencePostLoginModelAction#fallbackModel.
  ProviderLoginResult: ProviderLoginResult#
---
# Module: [`packages/coding-agent/src/core/prime-inference-model-selection.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts)

## Classes
### `PrimeInferencePostLoginModelAction`
- def: [`packages/coding-agent/src/core/prime-inference-model-selection.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts#L10)
- signature: `interface PrimeInferencePostLoginModelAction`
- members:
  - `fallbackModel` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts#L12)
  - `openModelPicker` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts#L11)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api)
- used by: [`prepareForModelSelectionAfterLogin`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.prepareForModelSelectionAfterLogin), [`resolvePrimeInferencePostLoginModelAction`](prime-inference-model-selection.ts.md#resolvePrimeInferencePostLoginModelAction)

### `ProviderLoginResult`
- def: [`packages/coding-agent/src/core/prime-inference-model-selection.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts#L6)
- signature: `type ProviderLoginResult`
- used by: [`resolvePrimeInferencePostLoginModelAction`](prime-inference-model-selection.ts.md#resolvePrimeInferencePostLoginModelAction)

## Functions
- `resolvePrimeInferencePostLoginModelAction(authResult: ProviderLoginResult, currentModel: Model<Api> | undefined, modelRegistry: Pick<ModelRegistry, "find">)` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-model-selection.ts#L15)

