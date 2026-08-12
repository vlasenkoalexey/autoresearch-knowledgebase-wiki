---
title: 'Module: packages/coding-agent/src/core/auth-guidance.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/auth-guidance.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`auth-guidance.ts`/
symbols:
  formatNoModelsAvailableMessage: formatNoModelsAvailableMessage().
  formatNoApiKeyFoundMessage: formatNoApiKeyFoundMessage().
  formatNoModelSelectedMessage: formatNoModelSelectedMessage().
  isNoModelsAvailableMessage: isNoModelsAvailableMessage().
  getProviderLoginHelp: getProviderLoginHelp().
  formatAuthenticationFailedMessage: formatAuthenticationFailedMessage().
  addLoginGuidanceToAuthError: addLoginGuidanceToAuthError().
  LOGIN_RECOVERY_MESSAGE: LOGIN_RECOVERY_MESSAGE.
  isLikelyAuthenticationError: isLikelyAuthenticationError().
  UNKNOWN_PROVIDER: UNKNOWN_PROVIDER.
---
# Module: [`packages/coding-agent/src/core/auth-guidance.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts)

## Functions
- `addLoginGuidanceToAuthError(message: string)` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L56)
- `formatAuthenticationFailedMessage(provider: string)` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L40)
- `formatNoApiKeyFoundMessage(provider: string)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L35)
- `formatNoModelSelectedMessage()` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L31)
- `formatNoModelsAvailableMessage()` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L15)
- `getProviderLoginHelp()` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L7)
- `isLikelyAuthenticationError(message: string)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L47)
- `isNoModelsAvailableMessage(message: string | undefined)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L27) — Whether a model fallback message is the "no models available" warning.

## Module values
- `LOGIN_RECOVERY_MESSAGE` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L5)
- `UNKNOWN_PROVIDER` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/auth-guidance.ts#L4)

