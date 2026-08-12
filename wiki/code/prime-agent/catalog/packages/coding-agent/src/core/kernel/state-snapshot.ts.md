---
title: 'Module: packages/coding-agent/src/core/kernel/state-snapshot.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/kernel/state-snapshot.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/kernel/`state-snapshot.ts`/
symbols:
  parseSnapshotResult: parseSnapshotResult().
  parseRestoreResult: parseRestoreResult().
  pyStr: pyStr().
  parseListNamesResult: parseListNamesResult().
  RestoreResult: RestoreResult#
  RESULT_MARKER: RESULT_MARKER.
  snapshotPathIn: snapshotPathIn().
  buildSnapshotCode: buildSnapshotCode().
  buildRestoreCode: buildRestoreCode().
  buildListNamesCode: buildListNamesCode().
  manifestPathIn: manifestPathIn().
  RestoreResult.restored: RestoreResult#restored.
  parseMarkerLine: parseMarkerLine().
  DEFAULT_SNAPSHOT_MAX_BYTES: DEFAULT_SNAPSHOT_MAX_BYTES.
  RestoreResult.failed: RestoreResult#failed.
  SnapshotResult: SnapshotResult#
  SnapshotResult.saved: SnapshotResult#saved.
  asStringArray: asStringArray().
  KERNEL_STATE_BASENAME: KERNEL_STATE_BASENAME.
  RawSnapshot.bytes: RawSnapshot#bytes.
  asReasonArray: asReasonArray().
  SnapshotResult.skipped: SnapshotResult#skipped.
  RestoreResult.path: RestoreResult#path.
  RawListNames: RawListNames#
  RawListNames.names: RawListNames#names.
  RawListNames.error: RawListNames#error.
  RawSnapshot: RawSnapshot#
  RawSnapshot.saved: RawSnapshot#saved.
  RawSnapshot.skipped: RawSnapshot#skipped.
  RawSnapshot.error: RawSnapshot#error.
  RawRestore: RawRestore#
  RawRestore.restored: RawRestore#restored.
  RawRestore.failed: RawRestore#failed.
  RawRestore.error: RawRestore#error.
  SnapshotResult.bytes: SnapshotResult#bytes.
  SnapshotResult.path: SnapshotResult#path.
---
# Module: [`packages/coding-agent/src/core/kernel/state-snapshot.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts)

## Classes
### `RawListNames`
- def: [`packages/coding-agent/src/core/kernel/state-snapshot.ts:224`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L224)
- signature: `interface RawListNames`
- members:
  - `error` — [`L226`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L226)
  - `names` — [`L225`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L225)
- used by: [`parseListNamesResult`](state-snapshot.ts.md#parseListNamesResult)

### `RawRestore`
- def: [`packages/coding-agent/src/core/kernel/state-snapshot.ts:236`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L236)
- signature: `interface RawRestore`
- members:
  - `error` — [`L239`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L239)
  - `failed` — [`L238`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L238)
  - `restored` — [`L237`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L237)
- used by: [`parseRestoreResult`](state-snapshot.ts.md#parseRestoreResult)

### `RawSnapshot`
- def: [`packages/coding-agent/src/core/kernel/state-snapshot.ts:229`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L229)
- signature: `interface RawSnapshot`
- members:
  - `bytes` — [`L232`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L232)
  - `error` — [`L233`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L233)
  - `saved` — [`L230`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L230)
  - `skipped` — [`L231`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L231)
- used by: [`parseSnapshotResult`](state-snapshot.ts.md#parseSnapshotResult)

### `RestoreResult`
- def: [`packages/coding-agent/src/core/kernel/state-snapshot.ts:29`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L29)
- signature: `interface RestoreResult`
- members:
  - `failed` — [`L33`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L33) — Names present in the snapshot that failed to revive, with a short reason.
  - `path` — [`L34`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L34)
  - `restored` — [`L31`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L31) — Names successfully revived into the kernel namespace.
- used by: [`agent-session.ts`](../agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`startKernel`](../tools/ipython.ts.md#IpythonKernelProvisioner.startKernel), [`ipython.ts`](../tools/ipython.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-tools-ipython.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-index.ts), [`restoreState`](index.ts.md#KernelManager.restoreState), [`parseRestoreResult`](state-snapshot.ts.md#parseRestoreResult), [`_onIpythonStateRestored`](../agent-session.ts.md#AgentSession._onIpythonStateRestored), [`<get>lastRestore`](../tools/ipython.ts.md#IpythonKernelProvisioner.-get-lastRestore), [`_lastRestore`](../tools/ipython.ts.md#IpythonKernelProvisioner._lastRestore), [`onRestore`](../tools/ipython.ts.md#IpythonToolOptions.onRestore)  (3 test-only)

### `SnapshotResult`
- def: [`packages/coding-agent/src/core/kernel/state-snapshot.ts:19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L19)
- signature: `interface SnapshotResult`
- members:
  - `bytes` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L25) — Payload size on disk, in bytes.
  - `path` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L26)
  - `saved` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L21) — Top-level names successfully serialized into the payload.
  - `skipped` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L23) — Names that could not be serialized, with a short reason.
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-kernel-index.ts), [`snapshotState`](index.ts.md#KernelManager.snapshotState), [`parseSnapshotResult`](state-snapshot.ts.md#parseSnapshotResult)  (2 test-only)

## Functions
- `asReasonArray(value: unknown)` — [`L246`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L246)
- `asStringArray(value: unknown)` — [`L242`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L242)
- `buildListNamesCode()` — [`L197`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L197) — Marker-line list of live user-defined names, filtered like the snapshot. Never raises.
- `buildRestoreCode(inPath: string)` — [`L146`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L146) — Python that loads the payload at `inPath` (if present) into the user namespace,
- `buildSnapshotCode(outPath: string, manifestPath: string, maxBytes: number)` — [`L56`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L56) — Python that serializes the user namespace to `outPath` (atomic write) and a
- `manifestPathIn(artifactDir: string)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L43) — Absolute path to the JSON manifest within a session's artifact directory.
- `parseListNamesResult(stdout: string)` — [`L293`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L293) — Sorted list of live user-defined names, or null if the marker was absent/invalid.
- `parseMarkerLine(stdout: string)` — [`L258`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L258) — Pull the marker line out of cell stdout and parse it, or null if absent/invalid.
- `parseRestoreResult(stdout: string, path: string)` — [`L282`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L282)
- `parseSnapshotResult(stdout: string, path: string)` — [`L271`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L271)
- `pyStr(value: string)` — [`L48`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L48) — Render a JS string as a Python string literal (JSON's escaping is a valid subset).
- `snapshotPathIn(artifactDir: string)` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L38) — Absolute path to the dill payload within a session's artifact directory.

## Module values
- `DEFAULT_SNAPSHOT_MAX_BYTES` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L11) — Default ceiling on a snapshot payload. Over-cap variables are skipped + reported.
- `KERNEL_STATE_BASENAME` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L14) — Base filename for the kernel snapshot within a session's artifact directory.
- `RESULT_MARKER` — [`L17`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/kernel/state-snapshot.ts#L17) — Marker the Python helpers print so the host can recover the JSON result line.

