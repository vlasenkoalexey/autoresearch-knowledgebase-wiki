---
title: 'Module: packages/ai/src/mcp/oauth.ts'
type: catalog
provenance: extracted
module: packages/ai/src/mcp/oauth.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/mcp/`oauth.ts`/
symbols:
  createMcpOAuthProvider: createMcpOAuthProvider().
  toCredentials: toCredentials().
  startCallbackServer.Promise.typeLiteral43.waitForCode: startCallbackServer().Promise:typeLiteral43:waitForCode.
  discover: discover().
  McpOAuthConfig.server: McpOAuthConfig#server.
  McpOAuthConfig.url: McpOAuthConfig#url.
  CALLBACK_PORTS: CALLBACK_PORTS.
  parseRedirectInput: parseRedirectInput().
  ALL_REDIRECT_URIS: ALL_REDIRECT_URIS.
  registerClient: registerClient().
  redirectUriFor: redirectUriFor.
  McpCredentials: McpCredentials#
  AuthServerMetadata.token_endpoint: AuthServerMetadata#token_endpoint.
  McpOAuthConfig: McpOAuthConfig#
  McpOAuthConfig.label: McpOAuthConfig#label.
  McpOAuthConfig.clientId: McpOAuthConfig#clientId.
  CALLBACK_PORT_BASE: CALLBACK_PORT_BASE.
  McpOAuthConfig.scopes: McpOAuthConfig#scopes.
  CallbackResult: CallbackResult#
  startCallbackServer.Promise.typeLiteral43.redirectUri: startCallbackServer().Promise:typeLiteral43:redirectUri.
  CALLBACK_PORT_COUNT: CALLBACK_PORT_COUNT.
  CALLBACK_PATH: CALLBACK_PATH.
  TOKEN_EXPIRY_BUFFER_MS: TOKEN_EXPIRY_BUFFER_MS.
  AuthServerMetadata: AuthServerMetadata#
  AuthServerMetadata.authorization_endpoint: AuthServerMetadata#authorization_endpoint.
  AuthServerMetadata.registration_endpoint: AuthServerMetadata#registration_endpoint.
  McpCredentials.tokenEndpoint: McpCredentials#tokenEndpoint.
  McpCredentials.clientId: McpCredentials#clientId.
  fetchJson: fetchJson().
  startCallbackServer.Promise.typeLiteral43.cancel: startCallbackServer().Promise:typeLiteral43:cancel.
  exchangeToken: exchangeToken().
  toCredentials.token-typeLiteral140.expires_in: toCredentials().(token)typeLiteral140:expires_in.
  CALLBACK_HOST: CALLBACK_HOST.
  AuthServerMetadata.issuer: AuthServerMetadata#issuer.
  AuthServerMetadata.scopes_supported: AuthServerMetadata#scopes_supported.
  randomState: randomState().
  startCallbackServer: startCallbackServer().
  startCallbackServer.Promise.typeLiteral43.server: startCallbackServer().Promise:typeLiteral43:server.
  parseRedirectInput.typeLiteral117.code: parseRedirectInput().typeLiteral117:code.
  parseRedirectInput.typeLiteral117.state: parseRedirectInput().typeLiteral117:state.
  toCredentials.token-typeLiteral140.access_token: toCredentials().(token)typeLiteral140:access_token.
  toCredentials.token-typeLiteral140.refresh_token: toCredentials().(token)typeLiteral140:refresh_token.
  exchangeToken.Promise.typeLiteral133.access_token: exchangeToken().Promise:typeLiteral133:access_token.
  exchangeToken.Promise.typeLiteral133.refresh_token: exchangeToken().Promise:typeLiteral133:refresh_token.
  exchangeToken.Promise.typeLiteral133.expires_in: exchangeToken().Promise:typeLiteral133:expires_in.
---
# Module: [`packages/ai/src/mcp/oauth.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts)

## Classes
### `AuthServerMetadata`
- def: [`packages/ai/src/mcp/oauth.ts:21`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L21)
- doc: Authorization-server metadata we rely on (RFC 8414 / OAuth 2.1 + DCR).
- signature: `interface AuthServerMetadata`
- members:
  - `authorization_endpoint` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L23)
  - `issuer` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L22)
  - `registration_endpoint` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L25)
  - `scopes_supported` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L26)
  - `token_endpoint` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L24)
- used by: [`createMcpOAuthProvider`](oauth.ts.md#createMcpOAuthProvider), [`discover`](oauth.ts.md#discover)

### `CallbackResult`
- def: [`packages/ai/src/mcp/oauth.ts:110`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L110)
- signature: `type CallbackResult`
- used by: [`waitForCode`](oauth.ts.md#startCallbackServer.Promise.typeLiteral43.waitForCode)

### `McpCredentials`
- def: [`packages/ai/src/mcp/oauth.ts:43`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L43)
- doc: Extra fields we persist alongside the standard credential triple.
- signature: `interface McpCredentials`
- members:
  - `clientId` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L45)
  - `tokenEndpoint` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L44)
- uses (calls/refs, reference-scoped): [`OAuthCredentials`](../utils/oauth/types.ts.md#OAuthCredentials)
- used by: [`createMcpOAuthProvider`](oauth.ts.md#createMcpOAuthProvider), [`toCredentials`](oauth.ts.md#toCredentials)

### `McpOAuthConfig`
- def: [`packages/ai/src/mcp/oauth.ts:29`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L29)
- signature: `interface McpOAuthConfig`
- members:
  - `clientId` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L37) — Pre-registered client id (servers without DCR, e.g. Slack).
  - `label` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L33) — Human label for UI.
  - `scopes` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L39) — Explicit scopes; falls back to the server's advertised scopes.
  - `server` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L31) — MCP server name; provider id becomes `mcp:<server>`.
  - `url` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L35) — The MCP endpoint URL — discovery is rooted at its origin.
- used by: [`createMcpOAuthProvider`](oauth.ts.md#createMcpOAuthProvider), [`registerUserProviders`](../../../coding-agent/src/core/mcp/mcp-manager.ts.md#McpManager.registerUserProviders), [`registerBuiltinMcpOAuthProviders`](catalog.ts.md#registerBuiltinMcpOAuthProviders), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-index.ts), [`catalog.ts`](catalog.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-mcp-catalog.ts), [`oauth`](catalog.ts.md#McpCatalogEntry.oauth)  (1 test-only)

## Functions
- `createMcpOAuthProvider(config: McpOAuthConfig)` — [`L250`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L250) — Build a provider for one MCP server. Register it with registerOAuthProvider().
- `discover(url: string)` — [`L67`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L67) — Try the protected-resource and auth-server well-known docs at the URL's origin.
- `exchangeToken(tokenEndpoint: string, params: Record<string, string>)` — [`L215`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L215)
- `fetchJson(url: string, init?: RequestInit | undefined)` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L48)
- `parseRedirectInput(input: string, expectedState: string)` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L193)
- `randomState()` — [`L57`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L57) — Random, URL-safe CSRF `state` value, independent of the PKCE verifier.
- `registerClient(registrationEndpoint: string, label: string)` — [`L91`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L91) — Dynamic client registration (RFC 7591). Returns the issued client_id.
- `startCallbackServer(label: string)` — [`L112`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L112)
- `toCredentials(token: { access_token: string; refresh_token?: string | undefined; expires_in?: number | undefined; }, tokenEndpoint: string, clientId: string, previousRefresh?: string | undefined)` — [`L231`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L231)

## Module values
- `ALL_REDIRECT_URIS` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L17)
- `CALLBACK_HOST` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L9)
- `CALLBACK_PATH` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L14)
- `CALLBACK_PORTS` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L15)
- `CALLBACK_PORT_BASE` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L12)
- `CALLBACK_PORT_COUNT` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L13)
- `TOKEN_EXPIRY_BUFFER_MS` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L18)
- `access_token` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L218)
- `access_token` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L232)
- `cancel` — [`L115`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L115)
- `code` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L193)
- `expires_in` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L218)
- `expires_in` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L232)
- `redirectUri` — [`L114`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L114)
- `redirectUriFor` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L16)
- `refresh_token` — [`L218`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L218)
- `refresh_token` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L232)
- `server` — [`L113`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L113)
- `state` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L193)
- `waitForCode` — [`L116`](../../../../../../../../raw/code/prime-agent/packages/ai/src/mcp/oauth.ts#L116)

