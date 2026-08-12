---
title: 'Module: packages/ai/src/providers/cloudflare.ts'
type: catalog
provenance: extracted
module: packages/ai/src/providers/cloudflare.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/providers/`cloudflare.ts`/
symbols:
  resolveCloudflareBaseUrl: resolveCloudflareBaseUrl().
  isCloudflareProvider: isCloudflareProvider().
  CLOUDFLARE_WORKERS_AI_BASE_URL: CLOUDFLARE_WORKERS_AI_BASE_URL.
  CLOUDFLARE_AI_GATEWAY_COMPAT_BASE_URL: CLOUDFLARE_AI_GATEWAY_COMPAT_BASE_URL.
  CLOUDFLARE_AI_GATEWAY_OPENAI_BASE_URL: CLOUDFLARE_AI_GATEWAY_OPENAI_BASE_URL.
  CLOUDFLARE_AI_GATEWAY_ANTHROPIC_BASE_URL: CLOUDFLARE_AI_GATEWAY_ANTHROPIC_BASE_URL.
---
# Module: [`packages/ai/src/providers/cloudflare.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts)

## Functions
- `isCloudflareProvider(provider: string)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L19)
- `resolveCloudflareBaseUrl(model: Model<Api>)` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L24) — Substitute `{VAR}` placeholders in a Cloudflare baseUrl from process.env.

## Module values
- `CLOUDFLARE_AI_GATEWAY_ANTHROPIC_BASE_URL` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L16) — AI Gateway → Anthropic passthrough.
- `CLOUDFLARE_AI_GATEWAY_COMPAT_BASE_URL` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L8) — AI Gateway Unified API. https://developers.cloudflare.com/ai-gateway/usage/unified-api/
- `CLOUDFLARE_AI_GATEWAY_OPENAI_BASE_URL` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L12) — AI Gateway → OpenAI passthrough. Used until /compat supports /v1/responses.
- `CLOUDFLARE_WORKERS_AI_BASE_URL` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/ai/src/providers/cloudflare.ts#L4) — Workers AI direct endpoint.

