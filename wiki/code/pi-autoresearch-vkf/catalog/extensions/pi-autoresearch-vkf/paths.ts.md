---
title: 'Module: extensions/pi-autoresearch-vkf/paths.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/paths.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`paths.ts`/
symbols:
  sessionPaths: sessionPaths().
  memoryPaths: memoryPaths().
  LifecycleDir: LifecycleDir#
  lifecycleDir: lifecycleDir().
  hasGlobalMemory: hasGlobalMemory().
  hasSession: hasSession().
  hasMemory: hasMemory().
  ensureSessionDirs: ensureSessionDirs().
  ensureMemoryDirs: ensureMemoryDirs().
  globalRoot: globalRoot().
  PKG_DIR: PKG_DIR.
  LIFECYCLE_DIRS: LIFECYCLE_DIRS.
  pkgDir: pkgDir().
  SESSION_SUBDIR: SESSION_SUBDIR.
  MEMORY_SUBDIR: MEMORY_SUBDIR.
---
# Module: [`extensions/pi-autoresearch-vkf/paths.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts)

## Classes
### `LifecycleDir`
- def: [`extensions/pi-autoresearch-vkf/paths.ts:32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L32) — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- signature: `type LifecycleDir`
- uses (calls/refs, reference-scoped): [`LIFECYCLE_DIRS`](paths.ts.md#LIFECYCLE_DIRS)
- used by: [`cards.ts`](cards.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-cards.ts), [`readCardFile`](cards.ts.md#readCardFile), [`writeCard`](cards.ts.md#writeCard), [`bucket`](cards.ts.md#STATE_MAP.Record.typeLiteral9.bucket), [`lifecycleDir`](paths.ts.md#lifecycleDir), [`bucket`](cards.ts.md#Card.bucket), [`bucket`](cards.ts.md#listCards.filter-typeLiteral135.bucket)

## Functions
- `ensureMemoryDirs(root: string)` — [`L114`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L114) — Create the memory bundle tree if absent. Idempotent. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `ensureSessionDirs(root: string)` — [`L107`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L107) — Create the session directory tree if absent. Idempotent. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `globalRoot()` — [`L86`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L86) — The root of the global, cross-project memory. The global bundle then lives at
- `hasGlobalMemory()` — [`L92`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L92) — True when the global memory bundle has been created. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `hasMemory(root: string)` — [`L102`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L102) — True when a memory bundle already exists at the given root. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `hasSession(root: string)` — [`L97`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L97) — True when a session already exists at the given root. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `lifecycleDir(root: string, bucket: "staging" | "verified" | "deprecated")` — [`L77`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L77) — Resolve the absolute directory for a given lifecycle bucket. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `memoryPaths(root: string)` — [`L64`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L64) — Absolute paths of the memory bundle (`.autoresearch-vkf/memory/`). — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `pkgDir(root: string)` — [`L35`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L35) — Absolute path of the package's namespaced directory for a given root.
- `sessionPaths(root: string)` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L40) — Absolute paths of the session contract (`.autoresearch-vkf/session/`). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)

## Module values
- `LIFECYCLE_DIRS` — [`L31`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L31) — The three lifecycle directories inside the memory bundle. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `MEMORY_SUBDIR` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L28) — Subdirectory of {@link PKG_DIR} holding the durable VKF memory bundle. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `PKG_DIR` — [`L24`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L24) — The single namespaced directory the package owns inside a root. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)
- `SESSION_SUBDIR` — [`L26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/paths.ts#L26) — Subdirectory of {@link PKG_DIR} holding ephemeral per-run session state. — documented in [extensions-pi-autoresearch-vkf-paths.ts](../../../concepts/extensions-pi-autoresearch-vkf-paths.ts.md)

