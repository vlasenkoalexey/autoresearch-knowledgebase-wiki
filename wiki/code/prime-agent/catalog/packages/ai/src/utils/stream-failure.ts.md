---
title: 'Module: packages/ai/src/utils/stream-failure.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/stream-failure.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`stream-failure.ts`/
symbols:
  recordStreamFailure: recordStreamFailure().
  streamFailureFromStopReason: streamFailureFromStopReason().
  formatStreamFailureMessage: formatStreamFailureMessage().
  extractStreamFailureParts: extractStreamFailureParts().
  StreamFailureInfo.kind: StreamFailureInfo#kind.
  streamFailureMessage: streamFailureMessage().
  extractStreamFailureInfo: extractStreamFailureInfo().
  StreamFailureError.-constructor: StreamFailureError#`<constructor>`().
  classifyStreamFailure: classifyStreamFailure().
  StreamFailureInfo.requestId: StreamFailureInfo#requestId.
  StreamFailureError.info: StreamFailureError#info.
  extractStreamFailureParts.typeLiteral15.info: extractStreamFailureParts().typeLiteral15:info.
  StreamFailureInfo: StreamFailureInfo#
  StreamFailureError: StreamFailureError#
  truncateRawPayload: truncateRawPayload().
  StreamFailureInfo.providerErrorType: StreamFailureInfo#providerErrorType.
  StreamFailureInfo.status: StreamFailureInfo#status.
  KIND_MESSAGES: KIND_MESSAGES.
  log: log.
  StreamFailureKind: StreamFailureKind#
  MAX_RAW_LENGTH: MAX_RAW_LENGTH.
  extractStreamFailureParts.typeLiteral15.detail: extractStreamFailureParts().typeLiteral15:detail.
  StreamFailureInfo.raw: StreamFailureInfo#raw.
  recordStreamFailure.model-typeLiteral79.provider: recordStreamFailure().(model)typeLiteral79:provider.
  recordStreamFailure.model-typeLiteral79.id: recordStreamFailure().(model)typeLiteral79:id.
  recordStreamFailure.model-typeLiteral79.api: recordStreamFailure().(model)typeLiteral79:api.
---
# Module: [`packages/ai/src/utils/stream-failure.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts)

## Classes
### `StreamFailureError`  ·  implements/extends Error
- def: [`packages/ai/src/utils/stream-failure.ts:32`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L32)
- signature: `class StreamFailureError`
- members:
  - `<constructor>(message: string, info: StreamFailureInfo)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L35)
  - `info` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L33)
- uses (calls/refs, reference-scoped): [`StreamFailureInfo`](stream-failure.ts.md#StreamFailureInfo)
- used by: [`anthropic.ts`](../providers/anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-anthropic.ts), [`processResponsesStream`](../providers/openai-responses-shared.ts.md#processResponsesStream), [`openai-responses-shared.ts`](../providers/openai-responses-shared.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-responses-shared.ts), [`streamFailureFromStopReason`](stream-failure.ts.md#streamFailureFromStopReason), [`iterateAnthropicEvents`](../providers/anthropic.ts.md#iterateAnthropicEvents), [`formatStreamFailureMessage`](stream-failure.ts.md#formatStreamFailureMessage), [`extractStreamFailureParts`](stream-failure.ts.md#extractStreamFailureParts), [`anthropicSseError`](../providers/anthropic.ts.md#anthropicSseError)  (1 test-only)

### `StreamFailureInfo`
- def: [`packages/ai/src/utils/stream-failure.ts:22`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L22)
- signature: `interface StreamFailureInfo`
- members:
  - `kind` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L23)
  - `providerErrorType` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L25) — Provider's own error/stop identifier, e.g. "overloaded_error" or "SAFETY".
  - `raw` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L29) — Truncated raw provider payload for post-mortems.
  - `requestId` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L27)
  - `status` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L26)
- uses (calls/refs, reference-scoped): [`StreamFailureKind`](stream-failure.ts.md#StreamFailureKind)
- used by: [`processResponsesStream`](../providers/openai-responses-shared.ts.md#processResponsesStream), [`recordStreamFailure`](stream-failure.ts.md#recordStreamFailure), [`streamFailureFromStopReason`](stream-failure.ts.md#streamFailureFromStopReason), [`iterateAnthropicEvents`](../providers/anthropic.ts.md#iterateAnthropicEvents), [`formatStreamFailureMessage`](stream-failure.ts.md#formatStreamFailureMessage), [`extractStreamFailureParts`](stream-failure.ts.md#extractStreamFailureParts), [`streamFailureMessage`](stream-failure.ts.md#streamFailureMessage), [`extractStreamFailureInfo`](stream-failure.ts.md#extractStreamFailureInfo), [`<constructor>`](stream-failure.ts.md#StreamFailureError.-constructor), [`info`](stream-failure.ts.md#StreamFailureError.info), [`info`](stream-failure.ts.md#extractStreamFailureParts.typeLiteral15.info)  (1 test-only)

### `StreamFailureKind`
- def: [`packages/ai/src/utils/stream-failure.ts:11`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L11)
- doc: Shared classification and reporting for provider stream failures, so no
- signature: `type StreamFailureKind`
- used by: [`kind`](stream-failure.ts.md#StreamFailureInfo.kind), [`classifyStreamFailure`](stream-failure.ts.md#classifyStreamFailure), [`KIND_MESSAGES`](stream-failure.ts.md#KIND_MESSAGES)

## Functions
- `classifyStreamFailure(providerErrorType?: string | undefined, status?: number | undefined)` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L66)
- `extractStreamFailureInfo(error: unknown)` — [`L179`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L179) — Best-effort extraction of structured failure info from any thrown value:
- `extractStreamFailureParts(error: unknown)` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L117)
- `formatStreamFailureMessage(error: unknown)` — [`L189`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L189) — User-facing message for a thrown stream error: a classified one-liner with
- `recordStreamFailure(model: { provider: string; id: string; api: string; }, output: AssistantMessage, error: unknown)` — [`L206`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L206) — Record a terminal stream failure on the message (structured diagnostic that
- `streamFailureFromStopReason(rawStopReason: string | undefined, extra?: Pick<StreamFailureInfo, "requestId"> | undefined)` — [`L95`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L95) — Failure for a stream that terminated with a provider stop/finish reason that
- `streamFailureMessage(info: StreamFailureInfo, detail?: string | undefined)` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L55) — Build a user-facing message like "Provider overloaded (overloaded_error, 529) [request_id: req_abc]".
- `truncateRawPayload(raw: string)` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L113)

## Module values
- `KIND_MESSAGES` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L42)
- `MAX_RAW_LENGTH` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L111)
- `api` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L207)
- `detail` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L117)
- `id` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L207)
- `info` — [`L117`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L117)
- `log` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L198)
- `provider` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/stream-failure.ts#L207)

