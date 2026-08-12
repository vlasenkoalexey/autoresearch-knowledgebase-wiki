---
title: 'Module: packages/ai/src/env-api-keys.ts'
type: catalog
provenance: extracted
module: packages/ai/src/env-api-keys.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/`env-api-keys.ts`/
symbols:
  getEnvApiKey: getEnvApiKey().
  NODE_PATH_SPECIFIER: NODE_PATH_SPECIFIER.
  getProcEnv: getProcEnv().
  findEnvKeys: findEnvKeys().
  getPrimeTeamId: getPrimeTeamId().
  hasVertexAdcCredentials: hasVertexAdcCredentials().
  _existsSync: _existsSync.
  _homedir: _homedir.
  _join: _join.
  cachedVertexAdcCredentialsExists: cachedVertexAdcCredentialsExists.
  _procEnvCache: _procEnvCache.
  _readFileSync: _readFileSync.
  dynamicImport: dynamicImport.
  DynamicImport: DynamicImport#
  NODE_FS_SPECIFIER: NODE_FS_SPECIFIER.
  NODE_OS_SPECIFIER: NODE_OS_SPECIFIER.
  getApiKeyEnvVars: getApiKeyEnvVars().
---
# Module: [`packages/ai/src/env-api-keys.ts`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts)

## Classes
### `DynamicImport`
- def: [`packages/ai/src/env-api-keys.ts:12`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L12)
- signature: `type DynamicImport`
- used by: [`env-api-keys.ts`](env-api-keys.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-env-api-keys.ts)

## Functions
- `findEnvKeys(provider: KnownProvider)` — [`L147`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L147) — Find configured environment variables that can provide an API key for a provider.
- `getApiKeyEnvVars(provider: string)` — [`L95`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L95)
- `getEnvApiKey(provider: KnownProvider)` — [`L162`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L162) — Get API key for provider from known environment variables, e.g. OPENAI_API_KEY.
- `getPrimeTeamId()` — [`L217`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L217)
- `getProcEnv(key: string)` — [`L40`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L40) — Fallback for https://github.com/oven-sh/bun/issues/27802
- `hasVertexAdcCredentials()` — [`L67`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L67)

## Module values
- `NODE_FS_SPECIFIER` — [`L15`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L15)
- `NODE_OS_SPECIFIER` — [`L16`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L16)
- `NODE_PATH_SPECIFIER` — [`L17`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L17)
- `_existsSync` — [`L7`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L7)
- `_homedir` — [`L9`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L9)
- `_join` — [`L10`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L10)
- `_procEnvCache` — [`L33`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L33)
- `_readFileSync` — [`L8`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L8)
- `cachedVertexAdcCredentialsExists` — [`L65`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L65)
- `dynamicImport` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/src/env-api-keys.ts#L14)

