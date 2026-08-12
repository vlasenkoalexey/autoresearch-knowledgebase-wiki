---
title: 'Module: packages/ai/src/providers/google-shared.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/google-shared.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`google-shared.ts`/
symbols:
  convertMessages: convertMessages().
  convertTools: convertTools().
  isThinkingPart: isThinkingPart().
  retainThoughtSignature: retainThoughtSignature().
  getGoogleThinkingBudget: getGoogleThinkingBudget().
  GoogleThinkingLevel: GoogleThinkingLevel#
  sanitizeForOpenApi: sanitizeForOpenApi().
  mapStopReason: mapStopReason().
  resolveThoughtSignature: resolveThoughtSignature().
  mapToolChoice: mapToolChoice().
  isValidThoughtSignature: isValidThoughtSignature().
  supportsMultimodalFunctionResponse: supportsMultimodalFunctionResponse().
  requiresToolCallId: requiresToolCallId().
  mapStopReasonString: mapStopReasonString().
  GoogleApiType: GoogleApiType#
  GoogleBudgetThinkingLevel: GoogleBudgetThinkingLevel#
  base64SignaturePattern: base64SignaturePattern.
  getGeminiMajorVersion: getGeminiMajorVersion().
  JSON_SCHEMA_META_DECLARATIONS: JSON_SCHEMA_META_DECLARATIONS.
---
# Module: [`packages/ai/src/providers/google-shared.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts)

## Classes
### `GoogleApiType`
- def: [`packages/ai/src/providers/google-shared.ts:10`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L10)
- signature: `type GoogleApiType`
- used by: [`convertMessages`](google-shared.ts.md#convertMessages)

### `GoogleBudgetThinkingLevel`
- def: [`packages/ai/src/providers/google-shared.ts:18`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L18)
- signature: `type GoogleBudgetThinkingLevel`
- used by: [`getGoogleThinkingBudget`](google-shared.ts.md#getGoogleThinkingBudget)

### `GoogleThinkingLevel`
- def: [`packages/ai/src/providers/google-shared.ts:16`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L16)
- doc: Thinking level for Gemini 3 models.
- signature: `type GoogleThinkingLevel`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`google.ts`](google.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google.ts), [`google-vertex.ts`](google-vertex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google-vertex.ts), [`getThinkingLevel`](google.ts.md#getThinkingLevel), [`getGemini3ThinkingLevel`](google-vertex.ts.md#getGemini3ThinkingLevel), [`level`](google-vertex.ts.md#GoogleVertexOptions.thinking.typeLiteral0.level), [`level`](google.ts.md#GoogleOptions.thinking.typeLiteral0.level), [`THINKING_LEVEL_MAP`](google-vertex.ts.md#THINKING_LEVEL_MAP)

## Functions
- `convertMessages(model: Model<T>, context: Context)` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L117) — Convert internal messages to Gemini Content[] format.
- `convertTools(tools: Tool<TSchema>[], useParameters?: boolean)` — [`L298`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L298) — Convert tools to Gemini function declarations format.
- `getGeminiMajorVersion(modelId: string)` — [`L100`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L100)
- `getGoogleThinkingBudget(modelId: string, effort: GoogleBudgetThinkingLevel, customBudgets?: ThinkingBudgets | undefined)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L20)
- `isThinkingPart(part: Pick<Part, "thought" | "thoughtSignature">)` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L59) — Determines whether a streamed Gemini `Part` should be treated as "thinking".
- `isValidThoughtSignature(signature: string | undefined)` — [`L80`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L80)
- `mapStopReason(reason: FinishReason)` — [`L335`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L335) — Map Gemini FinishReason to our StopReason.
- `mapStopReasonString(reason: string)` — [`L367`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L367) — Map string finish reason to our StopReason (for raw API responses).
- `mapToolChoice(choice: string)` — [`L319`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L319) — Map tool choice string to Gemini FunctionCallingConfigMode.
- `requiresToolCallId(modelId: string)` — [`L96`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L96) — Models via Google APIs that require explicit tool call IDs in function calls/responses.
- `resolveThoughtSignature(isSameProviderAndModel: boolean, signature: string | undefined)` — [`L89`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L89) — Only keep signatures from the same provider/model and with valid base64.
- `retainThoughtSignature(existing: string | undefined, incoming: string | undefined)` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L72) — Retain thought signatures during streaming.
- `sanitizeForOpenApi(schema: unknown)` — [`L277`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L277) — Strip meta-declarations from a schema obj
- `supportsMultimodalFunctionResponse(modelId: string)` — [`L106`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L106)

## Module values
- `JSON_SCHEMA_META_DECLARATIONS` — [`L263`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L263)
- `base64SignaturePattern` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/google-shared.ts#L78)

