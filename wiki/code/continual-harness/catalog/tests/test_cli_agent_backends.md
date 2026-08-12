---
title: 'Module: tests/test_cli_agent_backends.py'
type: catalog
provenance: extracted
module: tests/test_cli_agent_backends.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_cli_agent_backends`/Test
symbols:
  TestCliSessionMetrics.test_populated: CliSessionMetrics#test_populated().
  TestClaudeCodeBackendBuildLaunchCmd.test_handle_stream_event_result_updates_metrics: ClaudeCodeBackendBuildLaunchCmd#test_handle_stream_event_result_updates_metrics().
  TestHermesCliBackendStreamEvent.test_result_updates_metrics: HermesCliBackendStreamEvent#test_result_updates_metrics().
  TestClaudeCodeBackendStreamEvent.test_handle_stream_event_result_stores_model: ClaudeCodeBackendStreamEvent#test_handle_stream_event_result_stores_model().
  TestCodexCliBackendHandleStreamEvent.test_turn_completed_updates_metrics: CodexCliBackendHandleStreamEvent#test_turn_completed_updates_metrics().
  TestCodexCliBackendHandleStreamEvent.test_mcp_tool_call_formats_tool_reasoning_like_claude_gemini: CodexCliBackendHandleStreamEvent#test_mcp_tool_call_formats_tool_reasoning_like_claude_gemini().
  TestCodexCliBackendHandleStreamEvent.test_mcp_tool_call_uses_buffered_reasoning_when_args_empty: CodexCliBackendHandleStreamEvent#test_mcp_tool_call_uses_buffered_reasoning_when_args_empty().
  TestCodexCliBackendHandleStreamEvent.test_turn_failed_sets_error: CodexCliBackendHandleStreamEvent#test_turn_failed_sets_error().
  TestHermesCliBackendStreamEvent.test_system_sets_session_and_model: HermesCliBackendStreamEvent#test_system_sets_session_and_model().
  TestHermesCliBackendStreamEvent.test_tool_use_posts_short_name_without_reasoning: HermesCliBackendStreamEvent#test_tool_use_posts_short_name_without_reasoning().
  TestCliSessionMetrics.test_defaults: CliSessionMetrics#test_defaults().
  TestClaudeCodeBackendStreamEvent.test_handle_stream_event_tool_use_increments_count: ClaudeCodeBackendStreamEvent#test_handle_stream_event_tool_use_increments_count().
  TestCodexCliBackendHandleStreamEvent.test_thread_started_sets_session_id: CodexCliBackendHandleStreamEvent#test_thread_started_sets_session_id().
  TestCodexCliBackendHandleStreamEvent.test_mcp_tool_call_increments_count: CodexCliBackendHandleStreamEvent#test_mcp_tool_call_increments_count().
  TestHermesCliBackendStreamEvent.test_tool_use_increments_count: HermesCliBackendStreamEvent#test_tool_use_increments_count().
  TestGetBackend.test_claude_returns_claude_code_backend: GetBackend#test_claude_returns_claude_code_backend().
  TestGetBackend.test_gemini_returns_gemini_cli_backend: GetBackend#test_gemini_returns_gemini_cli_backend().
  TestGetBackend.test_codex_returns_codex_cli_backend: GetBackend#test_codex_returns_codex_cli_backend().
  TestGetBackend.test_hermes_returns_hermes_cli_backend: GetBackend#test_hermes_returns_hermes_cli_backend().
  TestDevcontainerBuildContext.test_devcontainer_build_context_exists: DevcontainerBuildContext#test_devcontainer_build_context_exists().
  TestClaudeCodeBackendBuildLaunchCmd.test_returns_cmd_env_bootstrap_temp_path: ClaudeCodeBackendBuildLaunchCmd#test_returns_cmd_env_bootstrap_temp_path().
  TestCodexCliBackendBuildLaunchCmd.test_returns_cmd_with_exec_json: CodexCliBackendBuildLaunchCmd#test_returns_cmd_with_exec_json().
  TestCodexCliBackendBuildLaunchCmd.test_resume_session_id_appended: CodexCliBackendBuildLaunchCmd#test_resume_session_id_appended().
  TestCodexCliBackendBuildLaunchCmd.test_resume_last_appended: CodexCliBackendBuildLaunchCmd#test_resume_last_appended().
  TestCodexCliBackendBuildLaunchCmd.test_skip_git_repo_check_included: CodexCliBackendBuildLaunchCmd#test_skip_git_repo_check_included().
  TestCodexCliBackendBuildLaunchCmd.test_thinking_effort_adds_config_override: CodexCliBackendBuildLaunchCmd#test_thinking_effort_adds_config_override().
  TestCodexCliBackendGetResumeSessionId.test_empty_dir_returns_none: CodexCliBackendGetResumeSessionId#test_empty_dir_returns_none().
  TestCodexCliBackendGetResumeSessionId.test_sessions_dir_with_file_returns_stem: CodexCliBackendGetResumeSessionId#test_sessions_dir_with_file_returns_stem().
  TestCodexCliBackendGetResumeSessionId.test_returns_most_recent_session: CodexCliBackendGetResumeSessionId#test_returns_most_recent_session().
  TestHermesCliBackendBuildLaunchCmd.test_local_cmd_structure: HermesCliBackendBuildLaunchCmd#test_local_cmd_structure().
  TestHermesCliBackendBuildLaunchCmd.test_containerized_cmd_has_docker: HermesCliBackendBuildLaunchCmd#test_containerized_cmd_has_docker().
  TestGetBackend.test_unknown_raises: GetBackend#test_unknown_raises().
  TestCodexCliBackendHandleStreamEvent.capture_post: CodexCliBackendHandleStreamEvent#capture_post().
  TestHermesCliBackendStreamEvent.capture_post: HermesCliBackendStreamEvent#capture_post().
  TestCliSessionMetrics: CliSessionMetrics#
  TestDevcontainerBuildContext: DevcontainerBuildContext#
  TestGetBackend: GetBackend#
  TestClaudeCodeBackendBuildLaunchCmd: ClaudeCodeBackendBuildLaunchCmd#
  TestClaudeCodeBackendStreamEvent: ClaudeCodeBackendStreamEvent#
  TestCodexCliBackendBuildLaunchCmd: CodexCliBackendBuildLaunchCmd#
  TestCodexCliBackendGetResumeSessionId: CodexCliBackendGetResumeSessionId#
  TestCodexCliBackendHandleStreamEvent: CodexCliBackendHandleStreamEvent#
  TestHermesCliBackendBuildLaunchCmd: HermesCliBackendBuildLaunchCmd#
  TestHermesCliBackendStreamEvent: HermesCliBackendStreamEvent#
---
# Module: [`tests/test_cli_agent_backends.py`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py)

## Classes
### `TestClaudeCodeBackendBuildLaunchCmd`
- def: [`tests/test_cli_agent_backends.py:89`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L89)
- signature: `class TestClaudeCodeBackendBuildLaunchCmd:`
- members:
  - `test_handle_stream_event_result_updates_metrics(self)` — [`L115`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L115)
  - `test_returns_cmd_env_bootstrap_temp_path(self, tmp_path)` — [`L90`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L90)
- uses (calls/refs, reference-scoped): [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`handle_stream_event`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.handle_stream_event), [`build_launch_cmd`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.build_launch_cmd), [`input_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.output_tokens), [`ClaudeCodeBackend`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend), [`num_turns`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.num_turns), [`total_cost_usd`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.total_cost_usd)

### `TestClaudeCodeBackendStreamEvent`
- def: [`tests/test_cli_agent_backends.py:132`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L132)
- doc: Verify handle_stream_event correctly updates CliSessionMetrics.
- signature: `class TestClaudeCodeBackendStreamEvent:`
- members:
  - `test_handle_stream_event_result_stores_model(self)` — [`L142`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L142)
  - `test_handle_stream_event_tool_use_increments_count(self)` — [`L135`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L135)
- uses (calls/refs, reference-scoped): [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`handle_stream_event`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.handle_stream_event), [`tool_use_count`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`ClaudeCodeBackend`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend), [`num_turns`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.num_turns), [`total_cost_usd`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.total_cost_usd)

### `TestCliSessionMetrics`
- def: [`tests/test_cli_agent_backends.py:23`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L23)
- doc: Test CliSessionMetrics dataclass.
- signature: `class TestCliSessionMetrics:`
- members:
  - `test_defaults(self)` — [`L26`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L26)
  - `test_populated(self)` — [`L32`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L32)
- uses (calls/refs, reference-scoped): [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`session_id`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`input_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.output_tokens), [`model`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.model), [`num_turns`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.num_turns), [`total_cost_usd`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.total_cost_usd)

### `TestCodexCliBackendBuildLaunchCmd`
- def: [`tests/test_cli_agent_backends.py:157`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L157)
- signature: `class TestCodexCliBackendBuildLaunchCmd:`
- members:
  - `test_resume_last_appended(self, tmp_path)` — [`L189`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L189)
  - `test_resume_session_id_appended(self, tmp_path)` — [`L174`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L174)
  - `test_returns_cmd_with_exec_json(self, tmp_path)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L158)
  - `test_skip_git_repo_check_included(self, tmp_path)` — [`L204`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L204) — Codex requires --skip-git-repo-check when workspace is not a git repo (issue #7522).
  - `test_thinking_effort_adds_config_override(self, tmp_path)` — [`L218`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L218)
- uses (calls/refs, reference-scoped): [`CodexCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend), [`build_launch_cmd`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend.build_launch_cmd)

### `TestCodexCliBackendGetResumeSessionId`
- def: [`tests/test_cli_agent_backends.py:233`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L233)
- signature: `class TestCodexCliBackendGetResumeSessionId:`
- members:
  - `test_empty_dir_returns_none(self, tmp_path)` — [`L234`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L234)
  - `test_returns_most_recent_session(self, tmp_path)` — [`L246`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L246)
  - `test_sessions_dir_with_file_returns_stem(self, tmp_path)` — [`L238`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L238)
- uses (calls/refs, reference-scoped): [`CodexCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend), [`get_resume_session_id`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend.get_resume_session_id)

### `TestCodexCliBackendHandleStreamEvent`
- def: [`tests/test_cli_agent_backends.py:256`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L256)
- signature: `class TestCodexCliBackendHandleStreamEvent:`
- members:
  - `capture_post(server_url, thinking_text, duration_sec=0, interaction_type="codex")` — [`L291`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L291)
  - `test_mcp_tool_call_formats_tool_reasoning_like_claude_gemini(self)` — [`L285`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L285) — Codex should post [tool] {reasoning} in one line, not separate reasoning + tool.
  - `test_mcp_tool_call_increments_count(self)` — [`L275`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L275)
  - `test_mcp_tool_call_uses_buffered_reasoning_when_args_empty(self)` — [`L321`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L321) — When tool args lack reasoning, use buffered reasoning from prior reasoning block.
  - `test_thread_started_sets_session_id(self)` — [`L257`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L257)
  - `test_turn_completed_updates_metrics(self)` — [`L264`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L264)
  - `test_turn_failed_sets_error(self)` — [`L353`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L353)
- uses (calls/refs, reference-scoped): [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`handle_stream_event`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend.handle_stream_event), [`CodexCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend), [`session_id`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`input_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](../utils/agent_infrastructure/cli_agent_backends.md#CliAgentBackend._post_thinking), [`error`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.error), [`is_error`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.is_error)

### `TestDevcontainerBuildContext`
- def: [`tests/test_cli_agent_backends.py:48`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L48)
- doc: Verify devcontainer_build_context points to an existing directory.
- signature: `class TestDevcontainerBuildContext:`
- members:
  - `test_devcontainer_build_context_exists(self, cli_type)` — [`L52`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L52)
- uses (calls/refs, reference-scoped): [`get_backend`](../utils/agent_infrastructure/cli_agent_backends.md#get_backend), [`devcontainer_build_context`](../utils/agent_infrastructure/cli_agent_backends.md#CliAgentBackend.devcontainer_build_context)

### `TestGetBackend`
- def: [`tests/test_cli_agent_backends.py:63`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L63)
- signature: `class TestGetBackend:`
- members:
  - `test_claude_returns_claude_code_backend(self)` — [`L64`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L64)
  - `test_codex_returns_codex_cli_backend(self)` — [`L74`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L74)
  - `test_gemini_returns_gemini_cli_backend(self)` — [`L69`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L69)
  - `test_hermes_returns_hermes_cli_backend(self)` — [`L83`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L83)
  - `test_unknown_raises(self)` — [`L79`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L79)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`get_backend`](../utils/agent_infrastructure/cli_agent_backends.md#get_backend), [`CodexCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend), [`HermesCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend), [`ClaudeCodeBackend`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend), [`name`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.name), [`name`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend.name), [`name`](../utils/agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.name), [`name`](../utils/agent_infrastructure/cli_agent_backends.md#CodexCliBackend.name)

### `TestHermesCliBackendBuildLaunchCmd`
- def: [`tests/test_cli_agent_backends.py:362`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L362)
- signature: `class TestHermesCliBackendBuildLaunchCmd:`
- members:
  - `test_containerized_cmd_has_docker(self, tmp_path)` — [`L380`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L380)
  - `test_local_cmd_structure(self, tmp_path)` — [`L363`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L363)
- uses (calls/refs, reference-scoped): [`build_launch_cmd`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend.build_launch_cmd), [`HermesCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend)

### `TestHermesCliBackendStreamEvent`
- def: [`tests/test_cli_agent_backends.py:404`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L404)
- signature: `class TestHermesCliBackendStreamEvent:`
- members:
  - `capture_post(server_url, thinking_text, duration_sec=0, interaction_type="hermes")` — [`L428`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L428)
  - `test_result_updates_metrics(self)` — [`L441`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L441)
  - `test_system_sets_session_and_model(self)` — [`L405`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L405)
  - `test_tool_use_increments_count(self)` — [`L415`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L415)
  - `test_tool_use_posts_short_name_without_reasoning(self)` — [`L424`](../../../../../raw/code/continual-harness/tests/test_cli_agent_backends.py#L424)
- uses (calls/refs, reference-scoped): [`handle_stream_event`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend.handle_stream_event), [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`session_id`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`HermesCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#HermesCliBackend), [`input_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](../utils/agent_infrastructure/cli_agent_backends.md#CliAgentBackend._post_thinking), [`model`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.model), [`num_turns`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.num_turns)

