---
title: 'Module: packages/coding-agent/src/core/prime-inference-models.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/prime-inference-models.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`prime-inference-models.ts`/
symbols:
  PRIVATE_PRIME_INFERENCE_MODELS: PRIVATE_PRIME_INFERENCE_MODELS.
  isPrivatePrimeInferenceModel: isPrivatePrimeInferenceModel().
  getPrivatePrimeInferenceModels: getPrivatePrimeInferenceModels().
  fetchAuthorizedPrivatePrimeInferenceModelIds: fetchAuthorizedPrivatePrimeInferenceModelIds().
  PRIME_INFERENCE_BASE_URL: PRIME_INFERENCE_BASE_URL.
  PRIVATE_MODEL_REFRESH_TIMEOUT_MS: PRIVATE_MODEL_REFRESH_TIMEOUT_MS.
---
# Module: [`packages/coding-agent/src/core/prime-inference-models.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts)

## Functions
- `fetchAuthorizedPrivatePrimeInferenceModelIds(apiKey: string, teamHeaders: Record<string, string>, fetchFn?: (input: string | URL | Request, init?: RequestInit | undefined) => Promise<Response>, timeoutMs?: number)` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L39)
- `getPrivatePrimeInferenceModels()` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L30)
- `isPrivatePrimeInferenceModel(model: Pick<Model<string>, "id" | "provider">)` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L26)

## Module values
- `PRIME_INFERENCE_BASE_URL` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L3)
- `PRIVATE_MODEL_REFRESH_TIMEOUT_MS` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L4)
- `PRIVATE_PRIME_INFERENCE_MODELS` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prime-inference-models.ts#L6)

