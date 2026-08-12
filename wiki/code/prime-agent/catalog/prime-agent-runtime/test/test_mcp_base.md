---
title: 'Module: prime-agent-runtime/test/test_mcp_base.py'
type: catalog
provenance: extracted
module: prime-agent-runtime/test/test_mcp_base.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `prime-agent-runtime.test.test_mcp_base`/
symbols:
  _Integration: _Integration#
  McpIntegrationTest.test_auto_bound_tool_calls_session: McpIntegrationTest#test_auto_bound_tool_calls_session().
  _run: _run().
  McpIntegrationTest._write_auth: McpIntegrationTest#_write_auth().
  McpIntegrationTest.test_unknown_tool_raises_with_available_list: McpIntegrationTest#test_unknown_tool_raises_with_available_list().
  McpIntegrationTest.test_resolve_config_prefers_host_override_and_headers: McpIntegrationTest#test_resolve_config_prefers_host_override_and_headers().
  McpIntegrationTest._run_open_session_with_transport: McpIntegrationTest#_run_open_session_with_transport().
  McpIntegrationTest.test_refreshes_via_host_when_expired: McpIntegrationTest#test_refreshes_via_host_when_expired().
  McpIntegrationTest.test_not_enabled_when_refresh_leaves_token_expired: McpIntegrationTest#test_not_enabled_when_refresh_leaves_token_expired().
  McpIntegrationTest.test_refresh_failure_surfaces_as_error_not_not_enabled: McpIntegrationTest#test_refresh_failure_surfaces_as_error_not_not_enabled().
  McpIntegrationTest.test_reads_oauth_access_token: McpIntegrationTest#test_reads_oauth_access_token().
  McpIntegrationTest.test_reads_api_key: McpIntegrationTest#test_reads_api_key().
  McpIntegrationTest.test_api_key_env_indirection_resolved: McpIntegrationTest#test_api_key_env_indirection_resolved().
  McpIntegrationTest._patch_session: McpIntegrationTest#_patch_session().
  McpIntegrationTest.transport: McpIntegrationTest#transport().
  McpIntegrationTest.auth_path: McpIntegrationTest#auth_path.
  McpIntegrationTest.fake_host_request: McpIntegrationTest#fake_host_request().
  _FakeSession.list_tools: _FakeSession#list_tools().
  _FakeSession.call_tool: _FakeSession#call_tool().
  McpIntegrationTest.test_not_enabled_without_credentials: McpIntegrationTest#test_not_enabled_without_credentials().
  McpIntegrationTest.test_bearer_token_env_wins.EnvIntegration.bearer_token_env: McpIntegrationTest#test_bearer_token_env_wins().EnvIntegration#bearer_token_env.
  McpIntegrationTest.test_open_session_uses_headers_signature: McpIntegrationTest#test_open_session_uses_headers_signature().
  McpIntegrationTest.test_open_session_uses_http_client_signature: McpIntegrationTest#test_open_session_uses_http_client_signature().
  McpIntegrationTest.agent_dir: McpIntegrationTest#agent_dir.
  McpIntegrationTest.test_bearer_token_env_wins.EnvIntegration: McpIntegrationTest#test_bearer_token_env_wins().EnvIntegration#
  McpIntegrationTest.test_requires_server_attribute.Bad.server: McpIntegrationTest#test_requires_server_attribute().Bad#server.
  _FakeSession: _FakeSession#
  _FakeSession.calls: _FakeSession#calls.
  McpIntegrationTest._tmp: McpIntegrationTest#_tmp.
  _FakeSession._tools: _FakeSession#_tools.
  _FakeSession._result: _FakeSession#_result.
  _FakeSession.make: _FakeSession#make().
  _Integration.url: _Integration#url.
  McpIntegrationTest.fake_open: McpIntegrationTest#fake_open().
  McpIntegrationTest.failing_host_request: McpIntegrationTest#failing_host_request().
  McpIntegrationTest.test_requires_server_attribute.Bad: McpIntegrationTest#test_requires_server_attribute().Bad#
  McpIntegrationTest.test_open_session_uses_headers_signature._CM: McpIntegrationTest#test_open_session_uses_headers_signature()._CM#
  McpIntegrationTest.test_open_session_uses_http_client_signature._CM: McpIntegrationTest#test_open_session_uses_http_client_signature()._CM#
  McpIntegrationTest.host_with_override: McpIntegrationTest#host_with_override().
  McpIntegrationTest.host_empty: McpIntegrationTest#host_empty().
  _FakeSession.__init__: _FakeSession#__init__().
  _Integration.server: _Integration#server.
  McpIntegrationTest: McpIntegrationTest#
  McpIntegrationTest.setUp: McpIntegrationTest#setUp().
  McpIntegrationTest.test_bearer_token_env_wins: McpIntegrationTest#test_bearer_token_env_wins().
  McpIntegrationTest.test_empty_structured_result_preserved: McpIntegrationTest#test_empty_structured_result_preserved().
  McpIntegrationTest.test_error_result_raises: McpIntegrationTest#test_error_result_raises().
  McpIntegrationTest.test_text_result_parsing: McpIntegrationTest#test_text_result_parsing().
  McpIntegrationTest.test_requires_server_attribute: McpIntegrationTest#test_requires_server_attribute().
  McpIntegrationTest.test_open_session_uses_headers_signature._CM.__aenter__: McpIntegrationTest#test_open_session_uses_headers_signature()._CM#__aenter__().
  McpIntegrationTest.test_open_session_uses_headers_signature._CM.__aexit__: McpIntegrationTest#test_open_session_uses_headers_signature()._CM#__aexit__().
  McpIntegrationTest.test_open_session_uses_http_client_signature._CM.__aenter__: McpIntegrationTest#test_open_session_uses_http_client_signature()._CM#__aenter__().
  McpIntegrationTest.test_open_session_uses_http_client_signature._CM.__aexit__: McpIntegrationTest#test_open_session_uses_http_client_signature()._CM#__aexit__().
---
# Module: [`prime-agent-runtime/test/test_mcp_base.py`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py)

## Classes
### `Bad`
- def: [`prime-agent-runtime/test/test_mcp_base.py:189`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L189)
- signature: `class Bad(McpIntegration):`
- members:
  - `server` — [`L190`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L190)

### `EnvIntegration`  ·  implements/extends _Integration
- def: [`prime-agent-runtime/test/test_mcp_base.py:140`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L140)
- signature: `class EnvIntegration(_Integration):`
- members:
  - `bearer_token_env` — [`L141`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L141)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `McpIntegrationTest`  ·  implements/extends TestCase
- def: [`prime-agent-runtime/test/test_mcp_base.py:52`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L52)
- signature: `class McpIntegrationTest(unittest.TestCase):`
- members:
  - `_run_open_session_with_transport(self, transport)` — [`L195`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L195) — Drive the real _open_session against a fake transport callable.
  - `failing_host_request(req_type, payload)` — [`L130`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L130)
  - `fake_host_request(req_type, payload)` — [`L97`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L97)
  - `fake_open(self_, stack: AsyncExitStack)` — [`L67`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L67)
  - `host_empty(req_type, payload)` — [`L260`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L260)
  - `host_with_override(req_type, payload)` — [`L257`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L257)
  - `setUp(self)` — [`L53`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L53)
  - `test_api_key_env_indirection_resolved(self)` — [`L87`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L87)
  - `test_auto_bound_tool_calls_session(self)` — [`L158`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L158)
  - `test_bearer_token_env_wins(self)` — [`L139`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L139)
  - `test_empty_structured_result_preserved(self)` — [`L146`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L146)
  - `test_error_result_raises(self)` — [`L151`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L151)
  - `test_not_enabled_when_refresh_leaves_token_expired(self)` — [`L109`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L109)
  - `test_not_enabled_without_credentials(self)` — [`L72`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L72)
  - `test_open_session_uses_headers_signature(self)` — [`L220`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L220)
  - `test_open_session_uses_http_client_signature(self)` — [`L238`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L238)
  - `test_reads_api_key(self)` — [`L83`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L83)
  - `test_reads_oauth_access_token(self)` — [`L77`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L77)
  - `test_refresh_failure_surfaces_as_error_not_not_enabled(self)` — [`L123`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L123)
  - `test_refreshes_via_host_when_expired(self)` — [`L92`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L92)
  - `test_requires_server_attribute(self)` — [`L188`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L188)
  - `test_resolve_config_prefers_host_override_and_headers(self)` — [`L256`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L256)
  - `test_text_result_parsing(self)` — [`L183`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L183)
  - `test_unknown_tool_raises_with_available_list(self)` — [`L172`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L172)
  - `transport(url, headers=None)` — [`L231`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L231)
  - `agent_dir` — [`L55`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L55)
  - `auth_path` — [`L56`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L56)
- protocol/private: `_patch_session`[`L65`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L65), `_tmp`[`L54`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L54), `_write_auth`[`L62`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L62)
- uses (calls/refs, reference-scoped): (7 test-only callers)

### `_CM`
- def: [`prime-agent-runtime/test/test_mcp_base.py:242`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L242)
- signature: `class _CM:`
- protocol/private: `__aenter__`[`L225`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L225), `__aenter__`[`L243`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L243), `__aexit__`[`L228`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L228), `__aexit__`[`L246`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L246)
- used by: (1 test-only callers)

### `_FakeSession`
- def: [`prime-agent-runtime/test/test_mcp_base.py:20`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L20)
- doc: Stand-in for an mcp ClientSession with canned tools/results.
- signature: `class _FakeSession:`
- members:
  - `call_tool(self, name, arguments)` — [`L42`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L42)
  - `list_tools(self)` — [`L28`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L28)
  - `make(name, desc, schema)` — [`L31`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L31)
  - `calls` — [`L26`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L26)
- protocol/private: `__init__`[`L23`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L23), `_result`[`L25`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L25), `_tools`[`L24`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L24)
- used by: (2 test-only callers)

### `_Integration`
- def: [`prime-agent-runtime/test/test_mcp_base.py:47`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L47)
- signature: `class _Integration(McpIntegration):`
- members:
  - `server` — [`L48`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L48)
  - `url` — [`L49`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L49)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (13 test-only callers)

## Functions
- `_run(coro)` — [`L16`](../../../../../../raw/code/prime-agent/prime-agent-runtime/test/test_mcp_base.py#L16)

