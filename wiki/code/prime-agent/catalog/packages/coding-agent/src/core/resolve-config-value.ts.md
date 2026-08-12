---
title: 'Module: packages/coding-agent/src/core/resolve-config-value.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/resolve-config-value.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`resolve-config-value.ts`/
symbols:
  executeWithConfiguredShell: executeWithConfiguredShell().
  executeCommandUncached: executeCommandUncached().
  resolveConfigValueUncached: resolveConfigValueUncached().
  resolveConfigValue: resolveConfigValue().
  clearConfigValueCache: clearConfigValueCache().
  executeWithConfiguredShell.typeLiteral3.executed: executeWithConfiguredShell().typeLiteral3:executed.
  executeWithConfiguredShell.typeLiteral3.value: executeWithConfiguredShell().typeLiteral3:value.
  executeCommand: executeCommand().
  resolveConfigValueOrThrow: resolveConfigValueOrThrow().
  resolveHeadersOrThrow: resolveHeadersOrThrow().
  commandResultCache: commandResultCache.
  resolveHeaders: resolveHeaders().
  executeWithDefaultShell: executeWithDefaultShell().
---
# Module: [`packages/coding-agent/src/core/resolve-config-value.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts)

## Functions
- `clearConfigValueCache()` — [`L140`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L140) — Clear the config value command cache. Exported for testing.
- `executeCommand(commandConfig: string)` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L78)
- `executeCommandUncached(commandConfig: string)` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L68)
- `executeWithConfiguredShell(command: string)` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L25)
- `executeWithDefaultShell(command: string)` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L55)
- `resolveConfigValue(config: string)` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L17) — Resolve a config value (API key, header value, etc.) to an actual value.
- `resolveConfigValueOrThrow(config: string, description: string)` — [`L99`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L99)
- `resolveConfigValueUncached(config: string)` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L91) — Resolve all header values using the same resolution logic as API keys.
- `resolveHeaders(headers: Record<string, string> | undefined)` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L115) — Resolve all header values using the same resolution logic as API keys.
- `resolveHeadersOrThrow(headers: Record<string, string> | undefined, description: string)` — [`L127`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L127)

## Module values
- `commandResultCache` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L10)
- `executed` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L25)
- `value` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/resolve-config-value.ts#L25)

