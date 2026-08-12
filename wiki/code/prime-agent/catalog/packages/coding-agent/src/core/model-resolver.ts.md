---
title: 'Module: packages/coding-agent/src/core/model-resolver.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/model-resolver.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`model-resolver.ts`/
symbols:
  findInitialModel.options-typeLiteral257.modelRegistry: findInitialModel().(options)typeLiteral257:modelRegistry.
  resolveCliModel.options-typeLiteral175.modelRegistry: resolveCliModel().(options)typeLiteral175:modelRegistry.
  parseModelPattern: parseModelPattern().
  resolveModelScopeFromModels: resolveModelScopeFromModels().
  ParsedModelResult.model: ParsedModelResult#model.
  restoreModelFromSession: restoreModelFromSession().
  ResolveCliModelResult.model: ResolveCliModelResult#model.
  ParsedModelResult.warning: ParsedModelResult#warning.
  ParsedModelResult.thinkingLevel: ParsedModelResult#thinkingLevel.
  findInitialModel: findInitialModel().
  InitialModelResult.model: InitialModelResult#model.
  ResolveCliModelResult.error: ResolveCliModelResult#error.
  resolveCliModel: resolveCliModel().
  ScopedModel.model: ScopedModel#model.
  findPreferredDefaultModel: findPreferredDefaultModel().
  defaultModelPerProvider: defaultModelPerProvider.
  buildFallbackModel: buildFallbackModel().
  findInitialModel.options-typeLiteral257.scopedModels: findInitialModel().(options)typeLiteral257:scopedModels.
  tryMatchModel: tryMatchModel().
  findExactModelReferenceMatch: findExactModelReferenceMatch().
  findInitialModel.options-typeLiteral257.isContinuing: findInitialModel().(options)typeLiteral257:isContinuing.
  resolveModelScope: resolveModelScope().
  resolveCliModel.options-typeLiteral175.cliModel: resolveCliModel().(options)typeLiteral175:cliModel.
  ResolveCliModelResult.thinkingLevel: ResolveCliModelResult#thinkingLevel.
  ScopedModel.thinkingLevel: ScopedModel#thinkingLevel.
  ResolveCliModelResult.warning: ResolveCliModelResult#warning.
  PRIME_INFERENCE_DEFAULT_MODEL_ID: PRIME_INFERENCE_DEFAULT_MODEL_ID.
  ScopedModel: ScopedModel#
  findInitialModel.options-typeLiteral257.defaultProvider: findInitialModel().(options)typeLiteral257:defaultProvider.
  findInitialModel.options-typeLiteral257.defaultModelId: findInitialModel().(options)typeLiteral257:defaultModelId.
  log: log.
  resolveCliModel.options-typeLiteral175.cliProvider: resolveCliModel().(options)typeLiteral175:cliProvider.
  restoreModelFromSession.Promise.typeLiteral310.model: restoreModelFromSession().Promise:typeLiteral310:model.
  findInitialModel.options-typeLiteral257.defaultThinkingLevel: findInitialModel().(options)typeLiteral257:defaultThinkingLevel.
  InitialModelResult.thinkingLevel: InitialModelResult#thinkingLevel.
  isAlias: isAlias().
  findInitialModel.options-typeLiteral257.cliProvider: findInitialModel().(options)typeLiteral257:cliProvider.
  findInitialModel.options-typeLiteral257.cliModel: findInitialModel().(options)typeLiteral257:cliModel.
  ParsedModelResult: ParsedModelResult#
  parseModelPattern.options-typeLiteral103.allowInvalidThinkingLevelFallback: parseModelPattern().(options)typeLiteral103:allowInvalidThinkingLevelFallback.
  ResolveCliModelResult: ResolveCliModelResult#
  InitialModelResult: InitialModelResult#
  restoreModelFromSession.Promise.typeLiteral310.fallbackMessage: restoreModelFromSession().Promise:typeLiteral310:fallbackMessage.
  InitialModelResult.fallbackMessage: InitialModelResult#fallbackMessage.
---
# Module: [`packages/coding-agent/src/core/model-resolver.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts)

## Classes
### `InitialModelResult`
- def: [`packages/coding-agent/src/core/model-resolver.ts:501`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L501)
- signature: `interface InitialModelResult`
- members:
  - `fallbackMessage` — [`L504`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L504)
  - `model` — [`L502`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L502)
  - `thinkingLevel` — [`L503`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L503)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel)
- used by: [`createAgentSession`](sdk.ts.md#createAgentSession), [`modelRegistry`](model-resolver.ts.md#findInitialModel.options-typeLiteral257.modelRegistry), [`modelFallbackMessage`](../main.ts.md#resolvePreparedStartupModel.Promise.typeLiteral217.modelFallbackMessage)  (3 test-only)

### `ParsedModelResult`
- def: [`packages/coding-agent/src/core/model-resolver.ts:159`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L159)
- signature: `interface ParsedModelResult`
- members:
  - `model` — [`L160`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L160)
  - `thinkingLevel` — [`L162`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L162) — Thinking level if explicitly specified in pattern, undefined otherwise
  - `warning` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L163)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel)
- used by: [`modelRegistry`](model-resolver.ts.md#resolveCliModel.options-typeLiteral175.modelRegistry), [`parseModelPattern`](model-resolver.ts.md#parseModelPattern), [`resolveModelScopeFromModels`](model-resolver.ts.md#resolveModelScopeFromModels)  (1 test-only)

### `ResolveCliModelResult`
- def: [`packages/coding-agent/src/core/model-resolver.ts:347`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L347)
- signature: `interface ResolveCliModelResult`
- members:
  - `error` — [`L355`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L355) — Error message suitable for CLI display.
  - `model` — [`L348`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L348)
  - `thinkingLevel` — [`L349`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L349)
  - `warning` — [`L350`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L350)
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel)
- used by: [`modelRegistry`](model-resolver.ts.md#findInitialModel.options-typeLiteral257.modelRegistry), [`diagnostics`](../main.ts.md#buildSessionOptions.typeLiteral122.diagnostics), [`modelRegistry`](model-resolver.ts.md#resolveCliModel.options-typeLiteral175.modelRegistry)  (1 test-only)

### `ScopedModel`
- def: [`packages/coding-agent/src/core/model-resolver.ts:55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L55)
- signature: `interface ScopedModel`
- members:
  - `model` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L56)
  - `thinkingLevel` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L58) — Thinking level if explicitly specified in pattern (e.g., "model:high"), undefined otherwise
- uses (calls/refs, reference-scoped): [`Model`](../../../ai/src/types.ts.md#Model), [`Api`](../../../ai/src/types.ts.md#Api), [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`modelRegistry`](model-resolver.ts.md#findInitialModel.options-typeLiteral257.modelRegistry), [`diagnostics`](../main.ts.md#buildSessionOptions.typeLiteral122.diagnostics), [`showModelsSelector`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.showModelsSelector), [`resolveModelScopeFromModels`](model-resolver.ts.md#resolveModelScopeFromModels), [`scopedModels`](model-resolver.ts.md#findInitialModel.options-typeLiteral257.scopedModels), [`resolveModelScope`](model-resolver.ts.md#resolveModelScope), [`buildSessionOptions`](../main.ts.md#buildSessionOptions), [`scopedModels`](../main.ts.md#PreparedRuntimeServices.scopedModels)  (1 test-only)

## Functions
- `buildFallbackModel(provider: string, modelId: string, availableModels: Model<Api>[])` — [`L166`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L166)
- `findExactModelReferenceMatch(modelReference: string, availableModels: Model<Api>[])` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L79) — Find an exact model reference match.
- `findInitialModel(options: { cliProvider?: string | undefined; cliModel?: string | undefined; scopedModels: ScopedModel[]; isContinuing: boolean; defaultProvider?: string | undefined; defaultModelId?: string | undefined; defaultThinkingLevel?: ThinkingLevel | undefined; modelRegistry: ModelRegistry; })` — [`L515`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L515) — Find the initial model to use based on priority:
- `findPreferredDefaultModel(availableModels: Model<Api>[])` — [`L182`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L182)
- `isAlias(id: string)` — [`L65`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L65) — Helper to check if a model ID looks like an alias (no date suffix)
- `parseModelPattern(pattern: string, availableModels: Model<Api>[], options?: { allowInvalidThinkingLevelFallback?: boolean | undefined; } | undefined)` — [`L214`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L214) — Parse a pattern to extract model and thinking level.
- `resolveCliModel(options: { cliProvider?: string | undefined; cliModel?: string | undefined; modelRegistry: ModelRegistry; })` — [`L369`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L369) — Resolve a single model from CLI flags.
- `resolveModelScope(patterns: string[], modelRegistry: ModelRegistry)` — [`L342`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L342)
- `resolveModelScopeFromModels(patterns: string[], availableModels: Model<Api>[])` — [`L280`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L280) — Resolve model patterns to actual Model objects with optional thinking levels
- `restoreModelFromSession(savedProvider: string, savedModelId: string, currentModel: Model<Api> | undefined, shouldPrintMessages: boolean, modelRegistry: ModelRegistry)` — [`L622`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L622) — Restore model from session, with fallback to available models
- `tryMatchModel(modelPattern: string, availableModels: Model<Api>[])` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L127) — Try to match a pattern to a model from the available models list.

## Module values
- `PRIME_INFERENCE_DEFAULT_MODEL_ID` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L17)
- `allowInvalidThinkingLevelFallback` — [`L217`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L217)
- `cliModel` — [`L371`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L371)
- `cliModel` — [`L517`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L517)
- `cliProvider` — [`L370`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L370)
- `cliProvider` — [`L516`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L516)
- `defaultModelId` — [`L521`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L521)
- `defaultModelPerProvider` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L20) — Default model IDs for each known provider
- `defaultProvider` — [`L520`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L520)
- `defaultThinkingLevel` — [`L522`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L522)
- `fallbackMessage` — [`L628`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L628)
- `isContinuing` — [`L519`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L519)
- `log` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L15)
- `model` — [`L628`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L628)
- `modelRegistry` — [`L372`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L372)
- `modelRegistry` — [`L523`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L523)
- `scopedModels` — [`L518`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/model-resolver.ts#L518)

