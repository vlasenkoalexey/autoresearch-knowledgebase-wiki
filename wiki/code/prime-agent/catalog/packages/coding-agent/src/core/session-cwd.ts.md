---
title: 'Module: packages/coding-agent/src/core/session-cwd.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-cwd.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-cwd.ts`/
symbols:
  getMissingSessionCwdIssue: getMissingSessionCwdIssue().
  MissingSessionCwdError: MissingSessionCwdError#
  formatMissingSessionCwdPrompt: formatMissingSessionCwdPrompt().
  assertSessionCwdExists: assertSessionCwdExists().
  formatMissingSessionCwdError: formatMissingSessionCwdError().
  MissingSessionCwdError.-constructor: MissingSessionCwdError#`<constructor>`().
  SessionCwdIssue: SessionCwdIssue#
  MissingSessionCwdError.issue: MissingSessionCwdError#issue.
  SessionCwdIssue.fallbackCwd: SessionCwdIssue#fallbackCwd.
  SessionCwdIssue.sessionFile: SessionCwdIssue#sessionFile.
  SessionCwdIssue.sessionCwd: SessionCwdIssue#sessionCwd.
  SessionCwdSource: SessionCwdSource#
  SessionCwdSource.getCwd: SessionCwdSource#getCwd().
  SessionCwdSource.getSessionFile: SessionCwdSource#getSessionFile().
---
# Module: [`packages/coding-agent/src/core/session-cwd.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts)

## Classes
### `MissingSessionCwdError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/session-cwd.ts:44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L44)
- signature: `class MissingSessionCwdError`
- members:
  - `<constructor>(issue: SessionCwdIssue)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L47)
  - `issue` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L45)
- uses (calls/refs, reference-scoped): [`formatMissingSessionCwdError`](session-cwd.ts.md#formatMissingSessionCwdError), [`SessionCwdIssue`](session-cwd.ts.md#SessionCwdIssue)
- used by: [`interactive-mode.ts`](../modes/interactive/interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`handleImportCommand`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleImportCommand), [`cancelled`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.handleResumeSession.Promise.typeLiteral3694.cancelled), [`serializeDaemonError`](../modes/daemon/daemon-errors.ts.md#serializeDaemonError), [`daemon-errors.ts`](../modes/daemon/daemon-errors.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-errors.ts), [`deserializeDaemonError`](../modes/daemon/daemon-errors.ts.md#deserializeDaemonError), [`promptForMissingSessionCwd`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.promptForMissingSessionCwd), [`assertSessionCwdExists`](session-cwd.ts.md#assertSessionCwdExists)  (3 test-only)

### `SessionCwdIssue`
- def: [`packages/coding-agent/src/core/session-cwd.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L3)
- signature: `interface SessionCwdIssue`
- members:
  - `fallbackCwd` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L6)
  - `sessionCwd` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L5)
  - `sessionFile` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L4)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`daemon-protocol.ts`](../modes/daemon/daemon-protocol.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-protocol.ts), [`promptForMissingSessionCwd`](../main.ts.md#promptForMissingSessionCwd), [`getMissingSessionCwdIssue`](session-cwd.ts.md#getMissingSessionCwdIssue), [`promptForMissingSessionCwd`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.promptForMissingSessionCwd), [`DaemonErrorInfo`](../modes/daemon/daemon-protocol.ts.md#DaemonErrorInfo), [`formatMissingSessionCwdPrompt`](session-cwd.ts.md#formatMissingSessionCwdPrompt), [`formatMissingSessionCwdError`](session-cwd.ts.md#formatMissingSessionCwdError), [`<constructor>`](session-cwd.ts.md#MissingSessionCwdError.-constructor), [`issue`](session-cwd.ts.md#MissingSessionCwdError.issue)  (1 test-only)

### `SessionCwdSource`
- def: [`packages/coding-agent/src/core/session-cwd.ts:9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L9)
- signature: `interface SessionCwdSource`
- members:
  - `getCwd(method)` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L10)
  - `getSessionFile(method)` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L11)
- used by: [`getMissingSessionCwdIssue`](session-cwd.ts.md#getMissingSessionCwdIssue), [`assertSessionCwdExists`](session-cwd.ts.md#assertSessionCwdExists)

## Functions
- `assertSessionCwdExists(sessionManager: SessionCwdSource, fallbackCwd: string)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L54)
- `formatMissingSessionCwdError(issue: SessionCwdIssue)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L35)
- `formatMissingSessionCwdPrompt(issue: SessionCwdIssue)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L40)
- `getMissingSessionCwdIssue(sessionManager: SessionCwdSource, fallbackCwd: string)` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-cwd.ts#L14)

