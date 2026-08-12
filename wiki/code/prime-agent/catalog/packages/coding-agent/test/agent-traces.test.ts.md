---
title: 'Module: packages/coding-agent/test/agent-traces.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/agent-traces.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`agent-traces.test.ts`/
symbols:
  createAssistantMessage: createAssistantMessage().
  writeSession: writeSession().
  createFetchRecorder: createFetchRecorder().
  FetchCall: FetchCall#
  FetchCall.url: FetchCall#url.
  FetchCall.init: FetchCall#init.
  createUserMessage: createUserMessage().
  advanceTimersUntil: advanceTimersUntil().
---
# Module: [`packages/coding-agent/test/agent-traces.test.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts)

## Classes
### `FetchCall`
- def: [`packages/coding-agent/test/agent-traces.test.ts:21`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L21)
- signature: `interface FetchCall`
- members:
  - `init` — [`L23`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L23)
  - `url` — [`L22`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L22)
- used by: (2 test-only callers)

## Functions
- `advanceTimersUntil(condition: () => boolean)` — [`L77`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L77)
- `createAssistantMessage(text: string)` — [`L26`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L26)
- `createFetchRecorder(calls: FetchCall[])` — [`L54`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L54)
- `createUserMessage(text: string)` — [`L46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L46)
- `writeSession(cwd: string, sessionDir: string, id: string, parentSession?: string | undefined)` — [`L69`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/agent-traces.test.ts#L69)

