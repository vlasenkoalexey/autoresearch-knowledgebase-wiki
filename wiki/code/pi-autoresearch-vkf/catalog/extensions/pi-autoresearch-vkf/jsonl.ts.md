---
title: 'Module: extensions/pi-autoresearch-vkf/jsonl.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/jsonl.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`jsonl.ts`/
symbols:
  appendLog: appendLog().
  LogEntry: LogEntry#
  readLog: readLog().
  LogEntry.ts: LogEntry#ts.
  LogEntry.event: LogEntry#event.
---
# Module: [`extensions/pi-autoresearch-vkf/jsonl.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts)

## Classes
### `LogEntry`
- def: [`extensions/pi-autoresearch-vkf/jsonl.ts:12`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts#L12) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- doc: A single log entry. `event` discriminates the kind of action.
- signature: `interface LogEntry`
- members:
  - `event` — [`L14`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts#L14)
  - `ts` — [`L13`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts#L13)
- used by: [`buildDashboardPayload`](index.ts.md#buildDashboardPayload), [`dashboard.ts`](dashboard.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-dashboard.ts), [`buildFullscreenLines`](dashboard.ts.md#buildFullscreenLines), [`appendLog`](jsonl.ts.md#appendLog), [`readUpdates`](dashboard.ts.md#readUpdates), [`readLog`](jsonl.ts.md#readLog)

## Functions
- `appendLog(logPath: string, entry: Omit<LogEntry, "ts"> & { ts?: string | undefined; })` — [`L19`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts#L19) — Append one entry, stamping `ts` if the caller did not provide one. — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `readLog(logPath: string)` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/jsonl.ts#L28) — Read all entries, skipping blank or unparseable lines.

