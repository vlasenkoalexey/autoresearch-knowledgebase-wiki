---
title: 'Module: packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`sdk-codex-cache-probe-tool-loop.ts`/
symbols:
  main: main().
  createMinimalResourceLoader: createMinimalResourceLoader().
  getWebSocketStatsSnapshot: getWebSocketStatsSnapshot().
  parseArgs: parseArgs().
  deterministicProbeTool: deterministicProbeTool().
  diffWebSocketStats: diffWebSocketStats().
  formatWebSocketStats: formatWebSocketStats().
  getAssistantText: getAssistantText().
  printHelp: printHelp().
  Args.transport: Args#transport.
  SubrequestRecord.usage: SubrequestRecord#usage.
  WebSocketStatsSnapshot.requests: WebSocketStatsSnapshot#requests.
  SubrequestRecord.stopReason: SubrequestRecord#stopReason.
  Args.sessionPath: Args#sessionPath.
  WebSocketStatsSnapshot: WebSocketStatsSnapshot#
  WebSocketStatsSnapshot.connectionsCreated: WebSocketStatsSnapshot#connectionsCreated.
  WebSocketStatsSnapshot.connectionsReused: WebSocketStatsSnapshot#connectionsReused.
  WebSocketStatsSnapshot.cachedContextRequests: WebSocketStatsSnapshot#cachedContextRequests.
  WebSocketStatsSnapshot.storeTrueRequests: WebSocketStatsSnapshot#storeTrueRequests.
  WebSocketStatsSnapshot.fullContextRequests: WebSocketStatsSnapshot#fullContextRequests.
  WebSocketStatsSnapshot.deltaRequests: WebSocketStatsSnapshot#deltaRequests.
  Args.turns: Args#turns.
  Args.maxTokens: Args#maxTokens.
  MIN_TURNS: MIN_TURNS.
  MAX_TURNS: MAX_TURNS.
  Transport: Transport#
  SubrequestRecord: SubrequestRecord#
  SubrequestRecord.turn: SubrequestRecord#turn.
  SubrequestRecord.subrequest: SubrequestRecord#subrequest.
  DEFAULT_TURNS: DEFAULT_TURNS.
  DEFAULT_MAX_TOKENS: DEFAULT_MAX_TOKENS.
  percentile: percentile().
  deterministicProbeParameters: deterministicProbeParameters.
  Args: Args#
  SubrequestRecord.elapsedMs: SubrequestRecord#elapsedMs.
  SubrequestRecord.text: SubrequestRecord#text.
  estimateTokens: estimateTokens().
  buildPrompt: buildPrompt().
  average: average().
---
# Module: [`packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts)

## Classes
### `Args`
- def: [`packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts:39`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L39)
- signature: `interface Args`
- members:
  - `maxTokens` — [`L43`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L43)
  - `sessionPath` — [`L41`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L41)
  - `transport` — [`L42`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L42)
  - `turns` — [`L40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L40)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `SubrequestRecord`
- def: [`packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts:56`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L56)
- signature: `interface SubrequestRecord`
- members:
  - `elapsedMs` — [`L59`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L59)
  - `stopReason` — [`L61`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L61)
  - `subrequest` — [`L58`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L58)
  - `text` — [`L62`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L62)
  - `turn` — [`L57`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L57)
  - `usage` — [`L60`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L60)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../../ai/src/types.ts.md#AssistantMessage), [`stopReason`](../../ai/src/types.ts.md#AssistantMessage.stopReason), [`usage`](../../ai/src/types.ts.md#AssistantMessage.usage)
- used by: (1 test-only callers)

### `Transport`
- def: [`packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts:37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L37)
- signature: `type Transport`
- used by: (2 test-only callers)

### `WebSocketStatsSnapshot`
- def: [`packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts:46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L46)
- signature: `interface WebSocketStatsSnapshot`
- members:
  - `cachedContextRequests` — [`L50`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L50)
  - `connectionsCreated` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L48)
  - `connectionsReused` — [`L49`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L49)
  - `deltaRequests` — [`L53`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L53)
  - `fullContextRequests` — [`L52`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L52)
  - `requests` — [`L47`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L47)
  - `storeTrueRequests` — [`L51`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L51)
- used by: (3 test-only callers)

## Functions
- `average(values: number[])` — [`L187`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L187)
- `buildPrompt(turn: number)` — [`L148`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L148)
- `createMinimalResourceLoader(systemPrompt: string)` — [`L173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L173)
- `deterministicProbeTool()` — [`L248`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L248)
- `diffWebSocketStats(after: WebSocketStatsSnapshot, before: WebSocketStatsSnapshot)` — [`L211`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L211)
- `estimateTokens(text: string)` — [`L144`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L144)
- `formatWebSocketStats(label: string, stats: WebSocketStatsSnapshot)` — [`L223`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L223)
- `getAssistantText(message: AssistantMessage)` — [`L235`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L235)
- `getWebSocketStatsSnapshot(sessionId: string)` — [`L198`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L198)
- `main()` — [`L273`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L273)
- `parseArgs(argv: string[])` — [`L70`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L70)
- `percentile(values: number[], percentileValue: number)` — [`L191`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L191)
- `printHelp()` — [`L125`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L125)

## Module values
- `DEFAULT_MAX_TOKENS` — [`L68`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L68)
- `DEFAULT_TURNS` — [`L65`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L65)
- `MAX_TURNS` — [`L67`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L67)
- `MIN_TURNS` — [`L66`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L66)
- `deterministicProbeParameters` — [`L243`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/sdk-codex-cache-probe-tool-loop.ts#L243)

