---
title: 'Module: packages/coding-agent/src/modes/rpc/jsonl.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/rpc/jsonl.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/rpc/`jsonl.ts`/
symbols:
  serializeJsonLine: serializeJsonLine().
  attachJsonlLineReader: attachJsonlLineReader().
  JsonlLineReaderOptions: JsonlLineReaderOptions#
  JsonlLineReaderOptions.maxLineLength: JsonlLineReaderOptions#maxLineLength.
  JsonlLineReaderOptions.onLineOverflow: JsonlLineReaderOptions#onLineOverflow.
---
# Module: [`packages/coding-agent/src/modes/rpc/jsonl.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts)

## Classes
### `JsonlLineReaderOptions`
- def: [`packages/coding-agent/src/modes/rpc/jsonl.ts:14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts#L14)
- signature: `interface JsonlLineReaderOptions`
- members:
  - `maxLineLength` — [`L15`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts#L15)
  - `onLineOverflow` — [`L16`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts#L16)
- used by: [`attachJsonlLineReader`](jsonl.ts.md#attachJsonlLineReader)

## Functions
- `attachJsonlLineReader(stream: Readable, onLine: (line: string) => void, options?: JsonlLineReaderOptions)` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts#L26) — Attach an LF-only JSONL reader to a stream.
- `serializeJsonLine(value: unknown)` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/rpc/jsonl.ts#L10) — Serialize a single strict JSONL record.

