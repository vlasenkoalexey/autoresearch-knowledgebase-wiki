---
title: 'Module: packages/coding-agent/src/core/session-import-errors.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-import-errors.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-import-errors.ts`/SessionImportFileNotFoundError#
symbols:
  SessionImportFileNotFoundError: ''
  SessionImportFileNotFoundError.-constructor: '`<constructor>`().'
  SessionImportFileNotFoundError.filePath: filePath.
---
# Module: [`packages/coding-agent/src/core/session-import-errors.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-import-errors.ts)

## Classes
### `SessionImportFileNotFoundError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/session-import-errors.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-import-errors.ts#L4)
- doc: Thrown when /import references a JSONL file path that does not exist.
- signature: `class SessionImportFileNotFoundError`
- members:
  - `<constructor>(filePath: string)` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-import-errors.ts#L7) — Thrown when /import references a JSONL file path that does not exist.
  - `filePath` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-import-errors.ts#L5)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`agent-session-runtime.ts`](agent-session-runtime.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session-runtime.ts), [`importFromJsonl`](agent-session-runtime.ts.md#AgentSessionRuntime.importFromJsonl), [`handleImportCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleImportCommand), [`serializeDaemonError`](../modes/daemon/daemon-errors.ts.md#serializeDaemonError), [`daemon-errors.ts`](../modes/daemon/daemon-errors.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-errors.ts), [`deserializeDaemonError`](../modes/daemon/daemon-errors.ts.md#deserializeDaemonError)  (2 test-only)

