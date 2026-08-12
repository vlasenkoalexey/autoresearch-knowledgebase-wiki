---
title: 'Module: packages/ai/src/providers/google-vertex.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/google-vertex.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`google-vertex.ts`/
symbols:
  streamGoogleVertex: streamGoogleVertex.
  buildParams: buildParams().
  streamSimpleGoogleVertex: streamSimpleGoogleVertex.
  GoogleVertexOptions: GoogleVertexOptions#
  buildHttpOptions: buildHttpOptions().
  resolveApiKey: resolveApiKey().
  getGemini3ThinkingLevel: getGemini3ThinkingLevel().
  GoogleVertexOptions.thinking: GoogleVertexOptions#thinking.
  createClient: createClient().
  createClientWithApiKey: createClientWithApiKey().
  getDisabledThinkingConfig: getDisabledThinkingConfig().
  isGemini3ProModel: isGemini3ProModel().
  isGemini3FlashModel: isGemini3FlashModel().
  resolveProject: resolveProject().
  resolveLocation: resolveLocation().
  GoogleVertexOptions.thinking.typeLiteral0.level: GoogleVertexOptions#thinking.typeLiteral0:level.
  ClampedThinkingLevel: ClampedThinkingLevel#
  THINKING_LEVEL_MAP: THINKING_LEVEL_MAP.
  GoogleVertexOptions.toolChoice: GoogleVertexOptions#toolChoice.
  GoogleVertexOptions.thinking.typeLiteral0.enabled: GoogleVertexOptions#thinking.typeLiteral0:enabled.
  GoogleVertexOptions.thinking.typeLiteral0.budgetTokens: GoogleVertexOptions#thinking.typeLiteral0:budgetTokens.
  API_VERSION: API_VERSION.
  GoogleVertexOptions.project: GoogleVertexOptions#project.
  GoogleVertexOptions.location: GoogleVertexOptions#location.
  GCP_VERTEX_CREDENTIALS_MARKER: GCP_VERTEX_CREDENTIALS_MARKER.
  toolCallCounter: toolCallCounter.
  resolveCustomBaseUrl: resolveCustomBaseUrl().
  baseUrlIncludesApiVersion: baseUrlIncludesApiVersion().
  isPlaceholderApiKey: isPlaceholderApiKey().
---
# Module: [`packages/ai/src/providers/google-vertex.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts)

## Classes
### `ClampedThinkingLevel`
- def: [`packages/ai/src/providers/google-vertex.ts:495`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L495)
- signature: `type ClampedThinkingLevel`
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../types.ts.md#ThinkingLevel)
- used by: [`streamSimpleGoogleVertex`](google-vertex.ts.md#streamSimpleGoogleVertex), [`getGemini3ThinkingLevel`](google-vertex.ts.md#getGemini3ThinkingLevel)

### `GoogleVertexOptions`
- def: [`packages/ai/src/providers/google-vertex.ts:43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L43)
- signature: `interface GoogleVertexOptions`
- members:
  - `budgetTokens` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L47)
  - `enabled` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L46)
  - `level` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L48)
  - `location` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L51)
  - `project` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L50)
  - `thinking` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L45)
  - `toolChoice` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L44)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions), [`GoogleThinkingLevel`](google-shared.ts.md#GoogleThinkingLevel)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamGoogleVertex`](google-vertex.ts.md#streamGoogleVertex), [`google-vertex.ts`](google-vertex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google-vertex.ts), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`buildParams`](google-vertex.ts.md#buildParams), [`streamSimpleGoogleVertex`](google-vertex.ts.md#streamSimpleGoogleVertex), [`loadGoogleVertexProviderModule`](register-builtins.ts.md#loadGoogleVertexProviderModule), [`resolveApiKey`](google-vertex.ts.md#resolveApiKey), [`googleVertexProviderModulePromise`](register-builtins.ts.md#googleVertexProviderModulePromise), [`resolveLocation`](google-vertex.ts.md#resolveLocation), [`resolveProject`](google-vertex.ts.md#resolveProject), [`streamGoogleVertex`](register-builtins.ts.md#GoogleVertexProviderModule.streamGoogleVertex)

## Functions
- `baseUrlIncludesApiVersion(baseUrl: string)` — [`L397`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L397)
- `buildHttpOptions(model: Model<"google-vertex">, optionsHeaders?: Record<string, string> | undefined)` — [`L368`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L368)
- `buildParams(model: Model<"google-vertex">, context: Context, options?: GoogleVertexOptions)` — [`L436`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L436)
- `createClient(model: Model<"google-vertex">, project: string, location: string, optionsHeaders?: Record<string, string> | undefined)` — [`L340`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L340)
- `createClientWithApiKey(model: Model<"google-vertex">, apiKey: string, optionsHeaders?: Record<string, string> | undefined)` — [`L355`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L355)
- `getDisabledThinkingConfig(model: Model<"google-vertex">)` — [`L505`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L505)
- `getGemini3ThinkingLevel(effort: ClampedThinkingLevel, model: Model<"google-generative-ai">)` — [`L521`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L521)
- `isGemini3FlashModel(model: Model<"google-generative-ai">)` — [`L501`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L501)
- `isGemini3ProModel(model: Model<"google-generative-ai">)` — [`L497`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L497)
- `isPlaceholderApiKey(apiKey: string)` — [`L414`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L414)
- `resolveApiKey(options?: GoogleVertexOptions | undefined)` — [`L406`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L406)
- `resolveCustomBaseUrl(baseUrl: string)` — [`L389`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L389)
- `resolveLocation(options?: GoogleVertexOptions | undefined)` — [`L428`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L428)
- `resolveProject(options?: GoogleVertexOptions | undefined)` — [`L418`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L418)

## Module values
- `API_VERSION` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L54)
- `GCP_VERTEX_CREDENTIALS_MARKER` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L55)
- `THINKING_LEVEL_MAP` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L57)
- `streamGoogleVertex` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L68)
- `streamSimpleGoogleVertex` — [`L304`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L304)
- `toolCallCounter` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-vertex.ts#L66)

