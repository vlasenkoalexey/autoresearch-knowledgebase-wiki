---
title: 'Module: packages/coding-agent/src/core/session-resolver.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/session-resolver.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`session-resolver.ts`/
symbols:
  resolveSessionPath: resolveSessionPath().
  findClosestSessionId: findClosestSessionId().
  resolveExactMatch: resolveExactMatch().
  resolvePartialMatch: resolvePartialMatch().
  SessionSelectorError: SessionSelectorError#
  SessionSelectorNotFoundError: SessionSelectorNotFoundError#
  SessionSelectorAmbiguousError.-constructor: SessionSelectorAmbiguousError#`<constructor>`().
  resolveUniqueMatch: resolveUniqueMatch().
  SessionSelectorAmbiguousError: SessionSelectorAmbiguousError#
  looksLikeSessionPath: looksLikeSessionPath().
  editDistance: editDistance().
  ResolvedSession: ResolvedSession#
  SessionSelectorNotFoundError.-constructor: SessionSelectorNotFoundError#`<constructor>`().
  SessionSelectorError.-constructor: SessionSelectorError#`<constructor>`().
---
# Module: [`packages/coding-agent/src/core/session-resolver.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts)

## Classes
### `ResolvedSession`
- def: [`packages/coding-agent/src/core/session-resolver.ts:5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L5)
- signature: `type ResolvedSession`
- used by: [`resolveSessionPath`](session-resolver.ts.md#resolveSessionPath)

### `SessionSelectorAmbiguousError`  ·  implements/extends Error, SessionSelectorError
- def: [`packages/coding-agent/src/core/session-resolver.ts:30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L30)
- signature: `class SessionSelectorAmbiguousError`
- members:
  - `<constructor>(selector: string, matches: readonly SessionInfo[])` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L31)
- uses (calls/refs, reference-scoped): [`SessionInfo`](session-manager.ts.md#SessionInfo), [`id`](session-manager.ts.md#SessionInfo.id), [`name`](session-manager.ts.md#SessionInfo.name), [`SessionSelectorError`](session-resolver.ts.md#SessionSelectorError)
- used by: [`SessionSelectorError`](session-resolver.ts.md#SessionSelectorError), [`resolveUniqueMatch`](session-resolver.ts.md#resolveUniqueMatch)  (1 test-only)

### `SessionSelectorError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/session-resolver.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L10)
- signature: `class SessionSelectorError`
- members:
  - `<constructor>(message: string, selector: string)` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L11)
- uses (calls/refs, reference-scoped): [`SessionSelectorNotFoundError`](session-resolver.ts.md#SessionSelectorNotFoundError), [`SessionSelectorAmbiguousError`](session-resolver.ts.md#SessionSelectorAmbiguousError)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`SessionSelectorNotFoundError`](session-resolver.ts.md#SessionSelectorNotFoundError), [`SessionSelectorAmbiguousError`](session-resolver.ts.md#SessionSelectorAmbiguousError)

### `SessionSelectorNotFoundError`  ·  implements/extends Error, SessionSelectorError
- def: [`packages/coding-agent/src/core/session-resolver.ts:20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L20)
- signature: `class SessionSelectorNotFoundError`
- members:
  - `<constructor>(selector: string, suggestion?: string | undefined)` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L21)
- uses (calls/refs, reference-scoped): [`SessionSelectorError`](session-resolver.ts.md#SessionSelectorError)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`resolveSessionPath`](session-resolver.ts.md#resolveSessionPath), [`SessionSelectorError`](session-resolver.ts.md#SessionSelectorError)  (2 test-only)

## Functions
- `editDistance(left: string, right: string)` — [`L131`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L131)
- `findClosestSessionId(selector: string, sessions: readonly Pick<SessionInfo, "id">[])` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L79)
- `looksLikeSessionPath(selector: string)` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L45)
- `resolveExactMatch(selector: string, sessions: readonly SessionInfo[])` — [`L111`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L111)
- `resolvePartialMatch(selector: string, sessions: readonly SessionInfo[])` — [`L119`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L119)
- `resolveSessionPath(selector: string, cwd: string, sessionDir?: string | undefined)` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L49)
- `resolveUniqueMatch(selector: string, matches: readonly SessionInfo[])` — [`L124`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/session-resolver.ts#L124)

