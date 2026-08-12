---
title: 'Module: prime-agent-runtime/src/rlm/mcp_base.py'
type: catalog
provenance: extracted
module: prime-agent-runtime/src/rlm/mcp_base.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `prime-agent-runtime.src.rlm.mcp_base`/
symbols:
  McpIntegration._resolve_token: McpIntegration#_resolve_token().
  McpIntegration._token: McpIntegration#_token().
  McpIntegration._call: McpIntegration#_call().
  McpIntegration._tools: McpIntegration#_tools.
  McpIntegration._open_session: McpIntegration#_open_session().
  McpIntegration._ensure_tools: McpIntegration#_ensure_tools().
  McpIntegration._resolve_config: McpIntegration#_resolve_config().
  McpIntegration.server: McpIntegration#server.
  McpIntegration.call_tool: McpIntegration#call_tool().
  McpIntegration.list_tools: McpIntegration#list_tools().
  McpIntegration.__getattr__: McpIntegration#__getattr__().
  _read_auth: _read_auth().
  McpIntegration._provider_id: McpIntegration#_provider_id().
  _parse_result: _parse_result().
  McpIntegration.__init__: McpIntegration#__init__().
  McpIntegration.bearer_token_env: McpIntegration#bearer_token_env.
  _EXPIRY_SKEW_SECONDS: _EXPIRY_SKEW_SECONDS.
  NotEnabled: NotEnabled#
  McpToolError: McpToolError#
  _agent_dir: _agent_dir().
  _resolve_config_value: _resolve_config_value().
  _resolve_streamable_http: _resolve_streamable_http().
  McpIntegration.url: McpIntegration#url.
  McpIntegration._lock: McpIntegration#_lock.
  __all__: __all__.
  NotEnabled.__init__: NotEnabled#__init__().
  NotEnabled.server: NotEnabled#server.
  McpIntegration: McpIntegration#
---
# Module: [`prime-agent-runtime/src/rlm/mcp_base.py`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py)

## Classes
### `McpIntegration`
- def: [`prime-agent-runtime/src/rlm/mcp_base.py:112`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L112)
- doc: Subclass and set `server` (and `url` for remote servers).
- signature: `class McpIntegration:`
- members:
  - `_open_session(self, stack: AsyncExitStack)` — [`L206`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L206) — Open an initialized MCP ClientSession bound to ``stack``.
  - `_resolve_config(self)` — [`L192`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L192) — Host-resolved (url, extra_headers), honoring a user's mcpServers override.
  - `_token(self)` — [`L142`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L142) — Current usable bearer token, or None if missing/expired (needs refresh).
  - `call_tool(self, tool: str, arguments: dict[str, Any] | None = None)` — [`L271`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L271) — Call ``tool`` on the server and return its parsed result.
  - `list_tools(self)` — [`L248`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L248) — Return the server's tools as ``[{name, description, inputSchema}]``.
  - `bearer_token_env` — [`L128`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L128)
  - `server` — [`L122`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L122)
  - `url` — [`L125`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L125)
- protocol/private: `__getattr__`[`L283`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L283), `__init__`[`L130`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L130), `_call`[`L288`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L288), `_ensure_tools`[`L253`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L253), `_lock`[`L134`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L134), `_provider_id`[`L139`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L139), `_resolve_token`[`L167`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L167), `_tools`[`L133`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L133)
- uses (calls/refs, reference-scoped): [`host_request`](__init__.md#host_request), [`_read_auth`](mcp_base.md#_read_auth), [`_parse_result`](mcp_base.md#_parse_result), [`NotEnabled`](mcp_base.md#NotEnabled), [`_EXPIRY_SKEW_SECONDS`](mcp_base.md#_EXPIRY_SKEW_SECONDS), [`_resolve_config_value`](mcp_base.md#_resolve_config_value), [`_resolve_streamable_http`](mcp_base.md#_resolve_streamable_http)

### `McpToolError`  ·  implements/extends RuntimeError
- def: [`prime-agent-runtime/src/rlm/mcp_base.py:52`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L52)
- doc: Raised when an MCP tool call returns a result flagged as an error.
- signature: `class McpToolError(RuntimeError):`
- used by: [`_parse_result`](mcp_base.md#_parse_result)

### `NotEnabled`  ·  implements/extends RuntimeError
- def: [`prime-agent-runtime/src/rlm/mcp_base.py:36`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L36)
- doc: Raised when an integration has no usable credentials.
- signature: `class NotEnabled(RuntimeError):`
- members:
  - `server` — [`L44`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L44)
- protocol/private: `__init__`[`L43`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L43)
- used by: [`_resolve_token`](mcp_base.md#McpIntegration._resolve_token)

## Functions
- `_agent_dir()` — [`L56`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L56) — Resolve the Prime Agent config dir the same way the rest of the runtime does.
- `_parse_result(result: Any)` — [`L306`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L306) — Normalize a CallToolResult into plain Python (structured output preferred).
- `_read_auth(provider: str)` — [`L68`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L68) — Read one credential entry from auth.json. Returns None if absent/unreadable.
- `_resolve_config_value(value: str)` — [`L80`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L80) — Resolve a stored api_key value the way the host does.
- `_resolve_streamable_http()` — [`L93`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L93) — Return an SDK streamable-HTTP transport callable.

## Module values
- `_EXPIRY_SKEW_SECONDS` — [`L33`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L33)
- `__all__` — [`L29`](../../../../../../../raw/code/prime-agent/prime-agent-runtime/src/rlm/mcp_base.py#L29)

