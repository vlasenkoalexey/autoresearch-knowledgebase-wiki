---
title: 'Module: packages/coding-agent/src/utils/paths.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/utils/paths.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/utils/`paths.ts`/
symbols:
  canonicalizePath: canonicalizePath().
  isLocalPath: isLocalPath().
  getCwdRelativePath: getCwdRelativePath().
  formatPathRelativeToCwdOrAbsolute: formatPathRelativeToCwdOrAbsolute().
  resolveAgainstCwd: resolveAgainstCwd().
---
# Module: [`packages/coding-agent/src/utils/paths.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts)

## Functions
- `canonicalizePath(path: string)` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts#L10) — Resolve a path to its canonical (real) form, following symlinks.
- `formatPathRelativeToCwdOrAbsolute(filePath: string, cwd: string)` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts#L54)
- `getCwdRelativePath(filePath: string, cwd: string)` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts#L43)
- `isLocalPath(value: string)` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts#L23) — Returns true if the value is NOT a package source (npm:, git:, etc.)
- `resolveAgainstCwd(filePath: string, cwd: string)` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/utils/paths.ts#L39)

