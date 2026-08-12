---
title: 'Module: packages/ai/src/providers/azure-openai-responses.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/azure-openai-responses.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`azure-openai-responses.ts`/
symbols:
  streamAzureOpenAIResponses: streamAzureOpenAIResponses.
  buildParams: buildParams().
  streamSimpleAzureOpenAIResponses: streamSimpleAzureOpenAIResponses.
  resolveAzureConfig.typeLiteral129.apiVersion: resolveAzureConfig().typeLiteral129:apiVersion.
  createClient: createClient().
  AzureOpenAIResponsesOptions: AzureOpenAIResponsesOptions#
  resolveDeploymentName: resolveDeploymentName().
  resolveAzureConfig: resolveAzureConfig().
  AzureOpenAIResponsesOptions.reasoningEffort: AzureOpenAIResponsesOptions#reasoningEffort.
  AzureOpenAIResponsesOptions.reasoningSummary: AzureOpenAIResponsesOptions#reasoningSummary.
  AzureOpenAIResponsesOptions.azureDeploymentName: AzureOpenAIResponsesOptions#azureDeploymentName.
  resolveAzureConfig.typeLiteral129.baseUrl: resolveAzureConfig().typeLiteral129:baseUrl.
  DEFAULT_AZURE_API_VERSION: DEFAULT_AZURE_API_VERSION.
  AZURE_TOOL_CALL_PROVIDERS: AZURE_TOOL_CALL_PROVIDERS.
  parseDeploymentNameMap: parseDeploymentNameMap().
  AzureOpenAIResponsesOptions.azureApiVersion: AzureOpenAIResponsesOptions#azureApiVersion.
  AzureOpenAIResponsesOptions.azureResourceName: AzureOpenAIResponsesOptions#azureResourceName.
  AzureOpenAIResponsesOptions.azureBaseUrl: AzureOpenAIResponsesOptions#azureBaseUrl.
  normalizeAzureBaseUrl: normalizeAzureBaseUrl().
  buildDefaultBaseUrl: buildDefaultBaseUrl().
---
# Module: [`packages/ai/src/providers/azure-openai-responses.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts)

## Classes
### `AzureOpenAIResponsesOptions`
- def: [`packages/ai/src/providers/azure-openai-responses.ts:49`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L49)
- signature: `interface AzureOpenAIResponsesOptions`
- members:
  - `azureApiVersion` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L52)
  - `azureBaseUrl` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L54)
  - `azureDeploymentName` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L55)
  - `azureResourceName` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L53)
  - `reasoningEffort` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L50)
  - `reasoningSummary` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L51)
- uses (calls/refs, reference-scoped): [`StreamOptions`](../types.ts.md#StreamOptions)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-index.ts), [`streamAzureOpenAIResponses`](azure-openai-responses.ts.md#streamAzureOpenAIResponses), [`register-builtins.ts`](register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`azure-openai-responses.ts`](azure-openai-responses.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-azure-openai-responses.ts), [`buildParams`](azure-openai-responses.ts.md#buildParams), [`streamSimpleAzureOpenAIResponses`](azure-openai-responses.ts.md#streamSimpleAzureOpenAIResponses), [`apiVersion`](azure-openai-responses.ts.md#resolveAzureConfig.typeLiteral129.apiVersion), [`loadAzureOpenAIResponsesProviderModule`](register-builtins.ts.md#loadAzureOpenAIResponsesProviderModule), [`createClient`](azure-openai-responses.ts.md#createClient), [`resolveDeploymentName`](azure-openai-responses.ts.md#resolveDeploymentName), [`azureOpenAIResponsesProviderModulePromise`](register-builtins.ts.md#azureOpenAIResponsesProviderModulePromise), [`resolveAzureConfig`](azure-openai-responses.ts.md#resolveAzureConfig), [`streamAzureOpenAIResponses`](register-builtins.ts.md#AzureOpenAIResponsesProviderModule.streamAzureOpenAIResponses)

## Functions
- `buildDefaultBaseUrl(resourceName: string)` — [`L181`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L181)
- `buildParams(model: Model<"azure-openai-responses">, context: Context, options: AzureOpenAIResponsesOptions | undefined, deploymentName: string)` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L243)
- `createClient(model: Model<"azure-openai-responses">, apiKey: string, options?: AzureOpenAIResponsesOptions | undefined)` — [`L216`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L216)
- `normalizeAzureBaseUrl(baseUrl: string)` — [`L158`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L158)
- `parseDeploymentNameMap(value: string | undefined)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L27)
- `resolveAzureConfig(model: Model<"azure-openai-responses">, options?: AzureOpenAIResponsesOptions | undefined)` — [`L185`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L185)
- `resolveDeploymentName(model: Model<"azure-openai-responses">, options?: AzureOpenAIResponsesOptions | undefined)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L40)

## Module values
- `AZURE_TOOL_CALL_PROVIDERS` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L25)
- `DEFAULT_AZURE_API_VERSION` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L24)
- `apiVersion` — [`L188`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L188)
- `baseUrl` — [`L188`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L188)
- `streamAzureOpenAIResponses` — [`L61`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L61) — Generate function for Azure OpenAI Responses API
- `streamSimpleAzureOpenAIResponses` — [`L138`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/azure-openai-responses.ts#L138)

