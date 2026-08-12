---
title: 'Module: packages/ai/src/log.ts'
type: catalog
provenance: extracted
module: packages/ai/src/log.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/`log.ts`/
symbols:
  getLogger: getLogger().
  emit: emit().
  stringifyLogEntry: stringifyLogEntry().
  setLogSink: setLogSink().
  LogEntry: LogEntry#
  Logger.warn: Logger#warn().
  Logger.error: Logger#error().
  LogEntry.level: LogEntry#level.
  sink: sink.
  LogSink: LogSink#
  LogEntry.ts: LogEntry#ts.
  Logger.debug: Logger#debug().
  LogEntry.component: LogEntry#component.
  LogEntry.msg: LogEntry#msg.
  Logger.info: Logger#info().
  LogLevel: LogLevel#
  Logger: Logger#
  jsonReplacer: jsonReplacer().
---
# Module: [`packages/ai/src/log.ts`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts)

## Classes
### `LogEntry`
- def: [`packages/ai/src/log.ts:10`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L10)
- signature: `interface LogEntry`
- members:
  - `component` — [`L13`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L13)
  - `level` — [`L12`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L12)
  - `msg` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L14)
  - `ts` — [`L11`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L11)
- uses (calls/refs, reference-scoped): [`LogLevel`](log.ts.md#LogLevel)
- used by: [`emit`](log.ts.md#emit), [`stringifyLogEntry`](log.ts.md#stringifyLogEntry), [`installFileLogSink`](../../coding-agent/src/core/logging.ts.md#installFileLogSink), [`logging.ts`](../../coding-agent/src/core/logging.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-logging.ts), [`LogSink`](log.ts.md#LogSink)  (1 test-only)

### `LogLevel`
- def: [`packages/ai/src/log.ts:8`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L8)
- doc: Minimal structured logger shared by pi-ai and its consumers. The library
- signature: `type LogLevel`
- used by: [`emit`](log.ts.md#emit), [`level`](log.ts.md#LogEntry.level)

### `LogSink`
- def: [`packages/ai/src/log.ts:18`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L18)
- signature: `type LogSink`
- uses (calls/refs, reference-scoped): [`LogEntry`](log.ts.md#LogEntry)
- used by: [`setLogSink`](log.ts.md#setLogSink), [`sink`](log.ts.md#sink)

### `Logger`
- def: [`packages/ai/src/log.ts:20`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L20)
- signature: `interface Logger`
- members:
  - `debug(method)` — [`L21`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L21)
  - `error(method)` — [`L24`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L24)
  - `info(method)` — [`L22`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L22)
  - `warn(method)` — [`L23`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L23)
- used by: [`modelRegistry`](../../coding-agent/src/core/model-resolver.ts.md#findInitialModel.options-typeLiteral257.modelRegistry), [`recordStreamFailure`](utils/stream-failure.ts.md#recordStreamFailure), [`log`](../../coding-agent/src/modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.log), [`resolveModelScopeFromModels`](../../coding-agent/src/core/model-resolver.ts.md#resolveModelScopeFromModels), [`loadSkillsFromDirInternal`](../../coding-agent/src/core/skills.ts.md#loadSkillsFromDirInternal), [`log`](../../coding-agent/src/modes/daemon/daemon-mode.ts.md#AgentDaemon.log), [`restoreModelFromSession`](../../coding-agent/src/core/model-resolver.ts.md#restoreModelFromSession), [`getLogger`](log.ts.md#getLogger), [`printTimings`](../../coding-agent/src/core/timings.ts.md#printTimings)  (1 test-only)

## Functions
- `emit(level: LogLevel, component: string, msg: string, fields?: Record<string, unknown> | undefined)` — [`L61`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L61)
- `getLogger(component: string)` — [`L81`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L81)
- `jsonReplacer()` — [`L34`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L34)
- `setLogSink(next: LogSink | undefined)` — [`L30`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L30) — Install the process-wide log sink. Pass undefined to restore the default.
- `stringifyLogEntry(entry: LogEntry)` — [`L47`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L47) — JSON.stringify that never throws: circular refs and BigInts degrade instead of dropping the entry.

## Module values
- `sink` — [`L27`](../../../../../../../raw/code/prime-agent/packages/ai/src/log.ts#L27)

