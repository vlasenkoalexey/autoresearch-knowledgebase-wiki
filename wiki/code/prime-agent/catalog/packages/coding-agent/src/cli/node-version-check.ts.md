---
title: 'Module: packages/coding-agent/src/cli/node-version-check.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/node-version-check.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`node-version-check.ts`/
symbols:
  assertNodeVersion: assertNodeVersion().
  MIN_NODE_VERSION: MIN_NODE_VERSION.
  isSupportedNodeVersion: isSupportedNodeVersion().
  NodeVersionGuardIO.log: NodeVersionGuardIO#log.
  NodeVersionGuardIO.version: NodeVersionGuardIO#version.
  parseVersion: parseVersion().
  MIN_NODE_VERSION_PARTS: MIN_NODE_VERSION_PARTS.
  NodeVersionGuardIO.exit: NodeVersionGuardIO#exit.
  ParsedNodeVersion: ParsedNodeVersion#
  NodeVersionGuardIO: NodeVersionGuardIO#
  ParsedNodeVersion.parts: ParsedNodeVersion#parts.
  ParsedNodeVersion.prerelease: ParsedNodeVersion#prerelease.
---
# Module: [`packages/coding-agent/src/cli/node-version-check.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts)

## Classes
### `NodeVersionGuardIO`
- def: [`packages/coding-agent/src/cli/node-version-check.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L6)
- signature: `interface NodeVersionGuardIO`
- members:
  - `exit` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L9)
  - `log` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L8)
  - `version` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L7)
- used by: [`assertNodeVersion`](node-version-check.ts.md#assertNodeVersion), [`cli.ts`](../cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli.ts)  (1 test-only)

### `ParsedNodeVersion`
- def: [`packages/coding-agent/src/cli/node-version-check.ts:12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L12)
- signature: `interface ParsedNodeVersion`
- members:
  - `parts` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L13)
  - `prerelease` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L14)
- used by: [`isSupportedNodeVersion`](node-version-check.ts.md#isSupportedNodeVersion), [`parseVersion`](node-version-check.ts.md#parseVersion)

## Functions
- `assertNodeVersion(io: NodeVersionGuardIO)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L40)
- `isSupportedNodeVersion(version: ParsedNodeVersion)` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L29)
- `parseVersion(version: string)` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L17)

## Module values
- `MIN_NODE_VERSION` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L4)
- `MIN_NODE_VERSION_PARTS` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/node-version-check.ts#L3)

