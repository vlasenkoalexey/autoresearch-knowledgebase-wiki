---
title: 'Module: packages/ai/test/oauth.ts'
type: catalog
provenance: extracted
module: packages/ai/test/oauth.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 test/`oauth.ts`/
symbols:
  resolveApiKey: resolveApiKey().
  AuthCredential: AuthCredential#
  loadAuthStorage: loadAuthStorage().
  saveAuthStorage: saveAuthStorage().
  AUTH_PATH: AUTH_PATH.
  AuthStorage: AuthStorage#
  OAuthCredentialEntry: OAuthCredentialEntry#
  ApiKeyCredential.typeLiteral0.type: ApiKeyCredential#typeLiteral0:type.
  ApiKeyCredential: ApiKeyCredential#
  ApiKeyCredential.typeLiteral0.key: ApiKeyCredential#typeLiteral0:key.
---
# Module: [`packages/ai/test/oauth.ts`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts)

## Classes
### `ApiKeyCredential`
- def: [`packages/ai/test/oauth.ts:16`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L16)
- signature: `type ApiKeyCredential`
- members:
  - `key` — [`L18`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L18)
  - `type` — [`L17`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L17)
- used by: (2 test-only callers)

### `AuthCredential`
- def: [`packages/ai/test/oauth.ts:25`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L25)
- signature: `type AuthCredential`
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `AuthStorage`
- def: [`packages/ai/test/oauth.ts:27`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L27)
- signature: `type AuthStorage`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `OAuthCredentialEntry`
- def: [`packages/ai/test/oauth.ts:21`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L21)
- signature: `type OAuthCredentialEntry`
- uses (calls/refs, reference-scoped): [`OAuthCredentials`](../src/utils/oauth/types.ts.md#OAuthCredentials)
- used by: (1 test-only callers)

## Functions
- `loadAuthStorage()` — [`L29`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L29)
- `resolveApiKey(provider: string)` — [`L57`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L57) — Resolve API key for a provider from ~/.pi/agent/auth.json
- `saveAuthStorage(storage: AuthStorage)` — [`L41`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L41)

## Module values
- `AUTH_PATH` — [`L14`](../../../../../../../raw/code/prime-agent/packages/ai/test/oauth.ts#L14)

