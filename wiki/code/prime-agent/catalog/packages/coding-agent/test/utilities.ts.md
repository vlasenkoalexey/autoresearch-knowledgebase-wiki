---
title: 'Module: packages/coding-agent/test/utilities.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/utilities.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/`utilities.ts`/
symbols:
  createTestResourceLoader: createTestResourceLoader().
  createTestSession: createTestSession().
  userMsg: userMsg().
  assistantMsg: assistantMsg().
  createTestExtensionsResult: createTestExtensionsResult().
  buildTestTree: buildTestTree().
  resolveApiKey: resolveApiKey().
  TestSessionContext.session: TestSessionContext#session.
  TestSessionContext.sessionManager: TestSessionContext#sessionManager.
  getRealAuthStorage: getRealAuthStorage().
  loadAuthStorage: loadAuthStorage().
  AUTH_PATH: AUTH_PATH.
  AuthCredential: AuthCredential#
  saveAuthStorage: saveAuthStorage().
  AuthStorageData: AuthStorageData#
  API_KEY: API_KEY.
  TestSessionContext: TestSessionContext#
  OAuthCredentialEntry: OAuthCredentialEntry#
  CreateTestExtensionsResultInput.factory: CreateTestExtensionsResultInput#factory.
  CreateTestResourceLoaderOptions: CreateTestResourceLoaderOptions#
  CreateTestResourceLoaderOptions.extensionsResult: CreateTestResourceLoaderOptions#extensionsResult.
  ApiKeyCredential.typeLiteral0.type: ApiKeyCredential#typeLiteral0:type.
  TestSessionContext.cleanup: TestSessionContext#cleanup.
  CreateTestExtensionsResultInput: CreateTestExtensionsResultInput#
  buildTestTree.structure-typeLiteral95.messages.Array.typeLiteral96.text: buildTestTree().(structure)typeLiteral95:messages.Array:typeLiteral96:text.
  buildTestTree.structure-typeLiteral95.messages.Array.typeLiteral96.branchFrom: buildTestTree().(structure)typeLiteral95:messages.Array:typeLiteral96:branchFrom.
  hasAuthForProvider: hasAuthForProvider().
  TestSessionOptions.settingsOverrides: TestSessionOptions#settingsOverrides.
  ApiKeyCredential: ApiKeyCredential#
  ApiKeyCredential.typeLiteral0.key: ApiKeyCredential#typeLiteral0:key.
  TestSessionOptions: TestSessionOptions#
  TestSessionOptions.inMemory: TestSessionOptions#inMemory.
  TestSessionOptions.systemPrompt: TestSessionOptions#systemPrompt.
  TestSessionContext.tempDir: TestSessionContext#tempDir.
  CreateTestExtensionsResultInput.path: CreateTestExtensionsResultInput#path.
  CreateTestResourceLoaderOptions.skills: CreateTestResourceLoaderOptions#skills.
  buildTestTree.structure-typeLiteral95.messages: buildTestTree().(structure)typeLiteral95:messages.
  buildTestTree.structure-typeLiteral95.messages.Array.typeLiteral96.role: buildTestTree().(structure)typeLiteral95:messages.Array:typeLiteral96:role.
  PI_AGENT_DIR: PI_AGENT_DIR.
---
# Module: [`packages/coding-agent/test/utilities.ts`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts)

## Classes
### `ApiKeyCredential`
- def: [`packages/coding-agent/test/utilities.ts:35`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L35)
- signature: `type ApiKeyCredential`
- members:
  - `key` — [`L37`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L37)
  - `type` — [`L36`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L36)
- used by: (2 test-only callers)

### `AuthCredential`
- def: [`packages/coding-agent/test/utilities.ts:44`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L44)
- signature: `type AuthCredential`
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `AuthStorageData`
- def: [`packages/coding-agent/test/utilities.ts:46`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L46)
- signature: `type AuthStorageData`
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (2 test-only callers)

### `CreateTestExtensionsResultInput`
- def: [`packages/coding-agent/test/utilities.ts:180`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L180)
- signature: `interface CreateTestExtensionsResultInput`
- members:
  - `factory` — [`L181`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L181)
  - `path` — [`L182`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L182)
- uses (calls/refs, reference-scoped): [`ExtensionFactory`](../src/core/extensions/types.ts.md#ExtensionFactory)
- used by: (3 test-only callers)

### `CreateTestResourceLoaderOptions`
- def: [`packages/coding-agent/test/utilities.ts:207`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L207)
- signature: `interface CreateTestResourceLoaderOptions`
- members:
  - `extensionsResult` — [`L208`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L208)
  - `skills` — [`L209`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L209)
- uses (calls/refs, reference-scoped): [`Skill`](../src/core/skills.ts.md#Skill), [`LoadExtensionsResult`](../src/core/extensions/types.ts.md#LoadExtensionsResult)
- used by: (1 test-only callers)

### `OAuthCredentialEntry`
- def: [`packages/coding-agent/test/utilities.ts:40`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L40)
- signature: `type OAuthCredentialEntry`
- uses (calls/refs, reference-scoped): [`OAuthCredentials`](../../ai/src/utils/oauth/types.ts.md#OAuthCredentials)
- used by: (1 test-only callers)

### `TestSessionContext`
- def: [`packages/coding-agent/test/utilities.ts:173`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L173)
- doc: Resources returned by createTestSession that need cleanup.
- signature: `interface TestSessionContext`
- members:
  - `cleanup` — [`L177`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L177)
  - `session` — [`L174`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L174)
  - `sessionManager` — [`L175`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L175)
  - `tempDir` — [`L176`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L176)
- uses (calls/refs, reference-scoped): [`SessionManager`](../src/core/session-manager.ts.md#SessionManager), [`AgentSession`](../src/core/agent-session.ts.md#AgentSession)
- used by: (2 test-only callers)

### `TestSessionOptions`
- def: [`packages/coding-agent/test/utilities.ts:161`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L161)
- doc: Options for creating a test session.
- signature: `interface TestSessionOptions`
- members:
  - `inMemory` — [`L163`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L163) — Use in-memory session (no file persistence)
  - `settingsOverrides` — [`L167`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L167) — Custom settings overrides
  - `systemPrompt` — [`L165`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L165) — Custom system prompt
- used by: (1 test-only callers)

## Functions
- `assistantMsg(text: string)` — [`L138`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L138) — Create a minimal assistant message for testing.
- `buildTestTree(session: SessionManager, structure: { messages: { role: "user" | "assistant"; text: string; branchFrom?: string | undefined; }[]; })` — [`L293`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L293) — Build a session tree for testing using SessionManager.
- `createTestExtensionsResult(inputs: (ExtensionFactory | CreateTestExtensionsResultInput)[], cwd?: string)` — [`L185`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L185)
- `createTestResourceLoader(options?: CreateTestResourceLoaderOptions)` — [`L212`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L212)
- `createTestSession(options?: TestSessionOptions)` — [`L236`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L236) — Create an AgentSession for testing with proper setup and cleanup.
- `getRealAuthStorage()` — [`L124`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L124) — Get an AuthStorage instance backed by ~/.pi/agent/auth.json
- `hasAuthForProvider(provider: string)` — [`L112`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L112) — Check if a provider has credentials in ~/.pi/agent/auth.json
- `loadAuthStorage()` — [`L48`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L48)
- `resolveApiKey(provider: string)` — [`L76`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L76) — Resolve API key for a provider from ~/.pi/agent/auth.json
- `saveAuthStorage(storage: AuthStorageData)` — [`L60`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L60)
- `userMsg(text: string)` — [`L131`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L131) — Create a minimal user message for testing.

## Module values
- `API_KEY` — [`L27`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L27) — API key for authenticated tests. Tests using this should be wrapped in
- `AUTH_PATH` — [`L33`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L33)
- `PI_AGENT_DIR` — [`L118`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L118) — Path to the real pi agent config directory
- `branchFrom` — [`L296`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L296)
- `messages` — [`L296`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L296)
- `role` — [`L296`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L296)
- `text` — [`L296`](../../../../../../../raw/code/prime-agent/packages/coding-agent/test/utilities.ts#L296)

