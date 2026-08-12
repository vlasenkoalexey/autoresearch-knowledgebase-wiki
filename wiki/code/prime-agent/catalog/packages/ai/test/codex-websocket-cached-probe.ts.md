---
title: 'Module: packages/ai/test/codex-websocket-cached-probe.ts'
type: catalog
provenance: extracted
module: packages/ai/test/codex-websocket-cached-probe.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`codex-websocket-cached-probe.ts`/
symbols:
  main: main().
  executeTool: executeTool().
  parseArgs: parseArgs().
  textOf: textOf().
  deterministicProbeTool: deterministicProbeTool().
  Args.sessionId: Args#sessionId.
  Args.transport: Args#transport.
  printHelp: printHelp().
  Args.reasoning: Args#reasoning.
  required: required().
  Args.maxTokens: Args#maxTokens.
  Args.turns: Args#turns.
  ThinkingLevel: ThinkingLevel#
  DEFAULT_TURNS: DEFAULT_TURNS.
  DEFAULT_MAX_TOKENS: DEFAULT_MAX_TOKENS.
  percentile: percentile().
  Args: Args#
  buildPrompt: buildPrompt().
  average: average().
  executeTool.call-Extract.typeLiteral45.type: executeTool().(call)Extract:typeLiteral45:type.
---
# Module: [`packages/ai/test/codex-websocket-cached-probe.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts)

## Classes
### `Args`
- def: [`packages/ai/test/codex-websocket-cached-probe.ts:24`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L24)
- signature: `interface Args`
- members:
  - `maxTokens` — [`L27`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L27)
  - `reasoning` — [`L28`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L28)
  - `sessionId` — [`L29`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L29)
  - `transport` — [`L26`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L26)
  - `turns` — [`L25`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L25)
- uses (calls/refs, reference-scoped): [`Transport`](../src/types.ts.md#Transport)  (1 test-only)
- used by: (2 test-only callers)

### `ThinkingLevel`
- def: [`packages/ai/test/codex-websocket-cached-probe.ts:22`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L22)
- signature: `type ThinkingLevel`
- used by: (2 test-only callers)

## Functions
- `average(values: number[])` — [`L147`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L147)
- `buildPrompt(turn: number)` — [`L99`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L99)
- `deterministicProbeTool()` — [`L116`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L116)
- `executeTool(call: ToolCall)` — [`L127`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L127)
- `main()` — [`L157`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L157)
- `parseArgs(argv: string[])` — [`L35`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L35)
- `percentile(values: number[], p: number)` — [`L151`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L151)
- `printHelp()` — [`L87`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L87)
- `required(value: string | undefined, flag: string)` — [`L82`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L82)
- `textOf(message: AssistantMessage)` — [`L139`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L139)

## Module values
- `DEFAULT_MAX_TOKENS` — [`L33`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L33)
- `DEFAULT_TURNS` — [`L32`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L32)
- `type` — [`L127`](../../../../../../../raw/code/prime-agent/packages/ai/test/codex-websocket-cached-probe.ts#L127)

