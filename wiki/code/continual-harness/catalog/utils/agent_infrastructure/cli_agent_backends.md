---
title: 'Module: utils/agent_infrastructure/cli_agent_backends.py'
type: catalog
provenance: extracted
module: utils/agent_infrastructure/cli_agent_backends.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.agent_infrastructure.cli_agent_backends`/
symbols:
  HermesCliBackend.handle_stream_event: HermesCliBackend#handle_stream_event().
  logger: logger.
  CliSessionMetrics: CliSessionMetrics#
  ClaudeCodeBackend.handle_stream_event: ClaudeCodeBackend#handle_stream_event().
  GeminiCliBackend: GeminiCliBackend#
  GeminiCliBackend.build_launch_cmd: GeminiCliBackend#build_launch_cmd().
  ClaudeCodeBackend.build_launch_cmd: ClaudeCodeBackend#build_launch_cmd().
  CodexCliBackend.handle_stream_event: CodexCliBackend#handle_stream_event().
  get_backend: get_backend().
  GeminiCliBackend.handle_stream_event: GeminiCliBackend#handle_stream_event().
  HermesCliBackend.build_launch_cmd: HermesCliBackend#build_launch_cmd().
  CodexCliBackend: CodexCliBackend#
  ClaudeCodeBackend.log_cli_interaction: ClaudeCodeBackend#log_cli_interaction().
  CodexCliBackend.build_launch_cmd: CodexCliBackend#build_launch_cmd().
  GeminiCliBackend._handle_gemini_result: GeminiCliBackend#_handle_gemini_result().
  CodexCliBackend._handle_item_mcp_tool_call: CodexCliBackend#_handle_item_mcp_tool_call().
  CliAgentBackend: CliAgentBackend#
  HermesCliBackend.log_cli_interaction: HermesCliBackend#log_cli_interaction().
  GeminiCliBackend.log_cli_interaction: GeminiCliBackend#log_cli_interaction().
  ClaudeCodeBackend._handle_assistant_tool_use_block: ClaudeCodeBackend#_handle_assistant_tool_use_block().
  GeminiCliBackend._handle_gemini_tool_use: GeminiCliBackend#_handle_gemini_tool_use().
  CliSessionMetrics.session_id: CliSessionMetrics#session_id.
  CodexCliBackend.log_cli_interaction: CodexCliBackend#log_cli_interaction().
  CliSessionMetrics.tool_use_count: CliSessionMetrics#tool_use_count.
  CliAgentBackend.handle_stream_event: CliAgentBackend#handle_stream_event().
  ClaudeCodeBackend._handle_assistant_text_block: ClaudeCodeBackend#_handle_assistant_text_block().
  GeminiCliBackend._handle_gemini_init: GeminiCliBackend#_handle_gemini_init().
  CliAgentBackend.name: CliAgentBackend#name().
  CliAgentBackend.log_cli_interaction: CliAgentBackend#log_cli_interaction().
  HermesCliBackend._ensure_hermes_config: HermesCliBackend#_ensure_hermes_config().
  CliAgentBackend._sync_metrics_to_server: CliAgentBackend#_sync_metrics_to_server().
  HermesCliBackend: HermesCliBackend#
  CliSessionMetrics.input_tokens: CliSessionMetrics#input_tokens.
  CliSessionMetrics.output_tokens: CliSessionMetrics#output_tokens.
  CliAgentBackend.agent_memory_subdir: CliAgentBackend#agent_memory_subdir().
  CliAgentBackend.devcontainer_build_context: CliAgentBackend#devcontainer_build_context().
  CliAgentBackend.get_resume_session_id: CliAgentBackend#get_resume_session_id().
  CliAgentBackend.run_login: CliAgentBackend#run_login().
  CodexCliBackend._handle_thread_started: CodexCliBackend#_handle_thread_started().
  CodexCliBackend._handle_turn_completed: CodexCliBackend#_handle_turn_completed().
  CodexCliBackend._handle_turn_failed: CodexCliBackend#_handle_turn_failed().
  CliAgentBackend._post_thinking: CliAgentBackend#_post_thinking().
  CliAgentBackend.container_image: CliAgentBackend#container_image().
  CliAgentBackend.build_launch_cmd: CliAgentBackend#build_launch_cmd().
  CliAgentBackend.run_stream_reader: CliAgentBackend#run_stream_reader().
  ClaudeCodeBackend: ClaudeCodeBackend#
  CliSession.process: CliSession#process.
  CliAgentBackend.seed_agent_auth: CliAgentBackend#seed_agent_auth().
  CliSessionMetrics.model: CliSessionMetrics#model.
  CliSessionMetrics.total_cost_usd: CliSessionMetrics#total_cost_usd.
  CliSessionMetrics.num_turns: CliSessionMetrics#num_turns.
  CliSession: CliSession#
  ClaudeCodeBackend._last_event_time: ClaudeCodeBackend#_last_event_time.
  CliAgentBackend.is_auth_fatal_error: CliAgentBackend#is_auth_fatal_error().
  GeminiCliBackend._write_gemini_settings: GeminiCliBackend#_write_gemini_settings().
  CodexCliBackend._ensure_codex_config: CodexCliBackend#_ensure_codex_config().
  HermesCliBackend._last_event_time: HermesCliBackend#_last_event_time.
  CliSessionMetrics.is_error: CliSessionMetrics#is_error.
  CliSessionMetrics.error: CliSessionMetrics#error.
  GeminiCliBackend._last_event_time: GeminiCliBackend#_last_event_time.
  GeminiCliBackend._handle_gemini_tool_result: GeminiCliBackend#_handle_gemini_tool_result().
  GeminiCliBackend._handle_gemini_message: GeminiCliBackend#_handle_gemini_message().
  CodexCliBackend._handle_item_reasoning: CodexCliBackend#_handle_item_reasoning().
  HermesCliBackend._build_hermes_mcp_block: HermesCliBackend#_build_hermes_mcp_block().
  CodexCliBackend.get_resume_session_id: CodexCliBackend#get_resume_session_id().
  CodexCliBackend._last_event_time: CodexCliBackend#_last_event_time.
  CliAgentBackend._write_workspace_files: CliAgentBackend#_write_workspace_files().
  HermesCliBackend._build_wrapper_cmd: HermesCliBackend#_build_wrapper_cmd().
  CliSessionMetrics.duration_ms: CliSessionMetrics#duration_ms.
  CliAgentBackend._build_bootstrap_content: CliAgentBackend#_build_bootstrap_content().
  CodexCliBackend.WORKSPACE_PATH: CodexCliBackend#WORKSPACE_PATH.
  HermesCliBackend.WORKSPACE_PATH: HermesCliBackend#WORKSPACE_PATH.
  HermesCliBackend.PROJECT_ROOT_PATH: HermesCliBackend#PROJECT_ROOT_PATH.
  HermesCliBackend.CONFIG_MARKER_END: HermesCliBackend#CONFIG_MARKER_END.
  CliAgentBackend._build_mcp_config_sse: CliAgentBackend#_build_mcp_config_sse().
  CliAgentBackend._build_mcp_config_stdio: CliAgentBackend#_build_mcp_config_stdio().
  ClaudeCodeBackend._handle_user_tool_result_block: ClaudeCodeBackend#_handle_user_tool_result_block().
  GeminiCliBackend._handle_gemini_error: GeminiCliBackend#_handle_gemini_error().
  CodexCliBackend._handle_error: CodexCliBackend#_handle_error().
  CliSessionMetrics.auth_fatal_error: CliSessionMetrics#auth_fatal_error.
  CliSession.stop_event: CliSession#stop_event.
  CliSession.temp_mcp_config_path: CliSession#temp_mcp_config_path.
  ClaudeCodeBackend.WORKSPACE_PATH: ClaudeCodeBackend#WORKSPACE_PATH.
  GeminiCliBackend.name: GeminiCliBackend#name().
  GeminiCliBackend.get_resume_session_id: GeminiCliBackend#get_resume_session_id().
  CodexCliBackend._pending_reasoning: CodexCliBackend#_pending_reasoning.
  HermesCliBackend.AGENT_MEMORY_PATH: HermesCliBackend#AGENT_MEMORY_PATH.
  HermesCliBackend.CONFIG_MARKER_BEGIN: HermesCliBackend#CONFIG_MARKER_BEGIN.
  HermesCliBackend.name: HermesCliBackend#name().
  HermesCliBackend.seed_agent_auth: HermesCliBackend#seed_agent_auth().
  HermesCliBackend.get_resume_session_id: HermesCliBackend#get_resume_session_id().
  CliSessionMetrics.duration_api_ms: CliSessionMetrics#duration_api_ms.
  CliAgentBackend._is_readonly: CliAgentBackend#_is_readonly().
  ClaudeCodeBackend.AGENT_MEMORY_PATH: ClaudeCodeBackend#AGENT_MEMORY_PATH.
  ClaudeCodeBackend.name: ClaudeCodeBackend#name().
  GeminiCliBackend.WORKSPACE_PATH: GeminiCliBackend#WORKSPACE_PATH.
  GeminiCliBackend.AGENT_MEMORY_PATH: GeminiCliBackend#AGENT_MEMORY_PATH.
  GeminiCliBackend.TELEMETRY_FILENAME: GeminiCliBackend#TELEMETRY_FILENAME.
  GeminiCliBackend.container_image: GeminiCliBackend#container_image().
  CodexCliBackend.AGENT_MEMORY_PATH: CodexCliBackend#AGENT_MEMORY_PATH.
  CodexCliBackend.DIRECTIVE_FILENAME: CodexCliBackend#DIRECTIVE_FILENAME.
  CodexCliBackend.name: CodexCliBackend#name().
  HermesCliBackend.DIRECTIVE_FILENAME: HermesCliBackend#DIRECTIVE_FILENAME.
  HermesCliBackend._last_seen_session_totals: HermesCliBackend#_last_seen_session_totals.
  CliSession.stream_thread: CliSession#stream_thread.
  ClaudeCodeBackend.container_image: ClaudeCodeBackend#container_image().
  ClaudeCodeBackend.DIRECTIVE_FILENAME: ClaudeCodeBackend#DIRECTIVE_FILENAME.
  ClaudeCodeBackend.MCP_CONFIG_FILENAME: ClaudeCodeBackend#MCP_CONFIG_FILENAME.
  ClaudeCodeBackend.is_auth_fatal_error: ClaudeCodeBackend#is_auth_fatal_error().
  ClaudeCodeBackend._build_cli_base_args: ClaudeCodeBackend#_build_cli_base_args().
  ClaudeCodeBackend.normalize_model_name: ClaudeCodeBackend#normalize_model_name().
  GeminiCliBackend.agent_memory_subdir: GeminiCliBackend#agent_memory_subdir().
  GeminiCliBackend.devcontainer_build_context: GeminiCliBackend#devcontainer_build_context().
  GeminiCliBackend._build_mcp_config_sse: GeminiCliBackend#_build_mcp_config_sse().
  GeminiCliBackend._build_mcp_config_stdio: GeminiCliBackend#_build_mcp_config_stdio().
  GeminiCliBackend._build_settings: GeminiCliBackend#_build_settings().
  GeminiCliBackend.run_login: GeminiCliBackend#run_login().
  CodexCliBackend.CONFIG_FILENAME: CodexCliBackend#CONFIG_FILENAME.
  CodexCliBackend.SESSIONS_SUBDIR: CodexCliBackend#SESSIONS_SUBDIR.
  CodexCliBackend.container_image: CodexCliBackend#container_image().
  HermesCliBackend.CONFIG_FILENAME: HermesCliBackend#CONFIG_FILENAME.
  HermesCliBackend.container_image: HermesCliBackend#container_image().
  HermesCliBackend.is_auth_fatal_error: HermesCliBackend#is_auth_fatal_error().
  HermesCliBackend._normalize_tool_name: HermesCliBackend#_normalize_tool_name().
  ClaudeCodeBackend.agent_memory_subdir: ClaudeCodeBackend#agent_memory_subdir().
  ClaudeCodeBackend.devcontainer_build_context: ClaudeCodeBackend#devcontainer_build_context().
  ClaudeCodeBackend.__init__: ClaudeCodeBackend#__init__().
  ClaudeCodeBackend.seed_agent_auth: ClaudeCodeBackend#seed_agent_auth().
  ClaudeCodeBackend.get_resume_session_id: ClaudeCodeBackend#get_resume_session_id().
  ClaudeCodeBackend.run_login: ClaudeCodeBackend#run_login().
  GeminiCliBackend.__init__: GeminiCliBackend#__init__().
  CodexCliBackend.agent_memory_subdir: CodexCliBackend#agent_memory_subdir().
  CodexCliBackend.devcontainer_build_context: CodexCliBackend#devcontainer_build_context().
  CodexCliBackend.__init__: CodexCliBackend#__init__().
  CodexCliBackend.is_auth_fatal_error: CodexCliBackend#is_auth_fatal_error().
  CodexCliBackend.seed_agent_auth: CodexCliBackend#seed_agent_auth().
  CodexCliBackend.run_login: CodexCliBackend#run_login().
  HermesCliBackend.agent_memory_subdir: HermesCliBackend#agent_memory_subdir().
  HermesCliBackend.devcontainer_build_context: HermesCliBackend#devcontainer_build_context().
  HermesCliBackend.__init__: HermesCliBackend#__init__().
  HermesCliBackend.run_login: HermesCliBackend#run_login().
---
# Module: [`utils/agent_infrastructure/cli_agent_backends.py`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py)

## Classes
### `ClaudeCodeBackend`  ·  implements/extends CliAgentBackend
- def: [`utils/agent_infrastructure/cli_agent_backends.py:309`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L309)
- doc: Backend for Anthropic Claude Code CLI (--print --output-format stream-json).
- signature: `class ClaudeCodeBackend(CliAgentBackend):`
- members:
  - `_build_cli_base_args(self, *, dangerously_skip_permissions: bool = True, resume_session_id: str | None = None, thinking_effort: str | None = None)` — [`L381`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L381) — Build base CLI args (output format, verbose, disallowed tools, permissions, resume, thinking).
  - `_handle_assistant_text_block(self, block: dict, now: float, metrics: CliSessionMetrics | None = None)` — [`L502`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L502) — Handle assistant text block: OAuth check + logging. Raises SystemExit(1) on auth error.
  - `_handle_assistant_tool_use_block(self, block: dict, now: float, metrics: CliSessionMetrics | None, server_url: str | None)` — [`L520`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L520) — Handle assistant tool_use block: metrics, _post_thinking, logging.
  - `_handle_user_tool_result_block(self, block: dict)` — [`L549`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L549) — Handle user tool_result block: logging.
  - `agent_memory_subdir(self)` — [`L317`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L317)
  - `build_launch_cmd(self, directive_path: str, server_url: str, working_dir: str, *, dangerously_skip_permissions: bool = True, project_root: str | None = None, containerized: bool = False, session_number: int = 1, resume_session_id: str | None = None, thinking_effort: str | None = None, mcp_sse_port: int | None = None, run_id: str | None = None, agent_memory_dir: str | None = None)` — [`L402`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L402)
  - `container_image(self)` — [`L321`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L321)
  - `devcontainer_build_context(self)` — [`L325`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L325)
  - `get_resume_session_id(self, agent_memory_dir: Path)` — [`L733`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L733) — Find the most recent session ID from Claude memory.
  - `handle_stream_event(self, event: dict, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L564`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L564) — documented in [utils-agent_infrastructure-cli_agent_backends](../../../concepts/utils-agent_infrastructure-cli_agent_backends.md)
  - `is_auth_fatal_error(self, text: str)` — [`L339`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L339) — Detect Claude Code OAuth token expiration or not logged in. See anthropics/claude-code#18225.
  - `log_cli_interaction(self, agent_memory_dir: Path, processed_hashes: set, last_cli_step: int, server_url: str | None = None)` — [`L643`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L643) — Poll Claude Code JSONL files and append new entries as steps to cumulative_metrics.
  - `name(self)` — [`L336`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L336)
  - `normalize_model_name(raw: str)` — [`L624`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L624) — Normalize provider-prefixed model names to canonical pricing-table form.
  - `run_login(self)` — [`L745`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L745) — Run 'claude auth login' interactively. Returns True on success.
  - `seed_agent_auth(self, agent_memory_dir: Path)` — [`L349`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L349) — Seed container agent memory with host Claude auth files.
  - `AGENT_MEMORY_PATH` — [`L314`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L314)
  - `DIRECTIVE_FILENAME` — [`L328`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L328)
  - `MCP_CONFIG_FILENAME` — [`L329`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L329)
  - `WORKSPACE_PATH` — [`L313`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L313)
- protocol/private: `__init__`[`L331`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L331), `_last_event_time`[`L333`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L333)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`get_llm_logger`](../data_persistence/llm_logger.md#get_llm_logger), [`logger`](cli_agent_backends.md#logger), [`CliSessionMetrics`](cli_agent_backends.md#CliSessionMetrics), [`load_new_usage_entries`](../metric_tracking/claude_session_reader.md#load_new_usage_entries), [`append_cli_step`](../data_persistence/llm_logger.md#LLMLogger.append_cli_step), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`session_id`](cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`_sync_metrics_to_server`](cli_agent_backends.md#CliAgentBackend._sync_metrics_to_server), [`input_tokens`](cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](cli_agent_backends.md#CliAgentBackend._post_thinking), [`model`](cli_agent_backends.md#CliSessionMetrics.model), [`num_turns`](cli_agent_backends.md#CliSessionMetrics.num_turns), [`total_cost_usd`](cli_agent_backends.md#CliSessionMetrics.total_cost_usd), [`error`](cli_agent_backends.md#CliSessionMetrics.error), [`is_error`](cli_agent_backends.md#CliSessionMetrics.is_error), [`_write_workspace_files`](cli_agent_backends.md#CliAgentBackend._write_workspace_files), [`_build_bootstrap_content`](cli_agent_backends.md#CliAgentBackend._build_bootstrap_content), [`duration_ms`](cli_agent_backends.md#CliSessionMetrics.duration_ms), [`find_jsonl_files`](../metric_tracking/claude_session_reader.md#find_jsonl_files), [`_build_mcp_config_sse`](cli_agent_backends.md#CliAgentBackend._build_mcp_config_sse), [`_build_mcp_config_stdio`](cli_agent_backends.md#CliAgentBackend._build_mcp_config_stdio), [`auth_fatal_error`](cli_agent_backends.md#CliSessionMetrics.auth_fatal_error), [`duration_api_ms`](cli_agent_backends.md#CliSessionMetrics.duration_api_ms)
- used by: [`get_backend`](cli_agent_backends.md#get_backend), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`handle_stream_event`](cli_agent_backends.md#CliAgentBackend.handle_stream_event), [`log_cli_interaction`](cli_agent_backends.md#CliAgentBackend.log_cli_interaction), [`name`](cli_agent_backends.md#CliAgentBackend.name), [`agent_memory_subdir`](cli_agent_backends.md#CliAgentBackend.agent_memory_subdir), [`devcontainer_build_context`](cli_agent_backends.md#CliAgentBackend.devcontainer_build_context), [`get_resume_session_id`](cli_agent_backends.md#CliAgentBackend.get_resume_session_id), [`run_login`](cli_agent_backends.md#CliAgentBackend.run_login), [`build_launch_cmd`](cli_agent_backends.md#CliAgentBackend.build_launch_cmd), [`container_image`](cli_agent_backends.md#CliAgentBackend.container_image), [`seed_agent_auth`](cli_agent_backends.md#CliAgentBackend.seed_agent_auth), [`is_auth_fatal_error`](cli_agent_backends.md#CliAgentBackend.is_auth_fatal_error)  (5 test-only)

### `CliAgentBackend`  ·  implements/extends ABC
- def: [`utils/agent_infrastructure/cli_agent_backends.py:55`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L55)
- doc: Abstract base for CLI agent backends (Claude Code, Codex, etc.).
- signature: `class CliAgentBackend(ABC):`
- members:
  - `_build_bootstrap_content(self, directive_path: str, server_url: str)` — [`L211`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L211) — Build bootstrap prompt string from directive file and server URL.
  - `_build_mcp_config_sse(self, mcp_sse_port: int)` — [`L181`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L181) — Build MCP config dict for SSE (containerized) mode. type=sse is REQUIRED.
  - `_build_mcp_config_stdio(self, server_url: str, pythonpath: str)` — [`L194`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L194) — Build MCP config dict for stdio (local) mode.
  - `_post_thinking(self, server_url: str, thinking_text: str, duration_sec: float = 0, interaction_type: str = "cli")` — [`L229`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L229) — POST agent thinking to game server for UI streaming (same as VLM agents).
  - `_sync_metrics_to_server(server_url: str)` — [`L285`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L285) — Push run_cli's in-memory cumulative metrics to the server (single-writer pattern).
  - `_write_workspace_files(self, working_dir: Path, bootstrap: str, mcp_config: dict, directive_filename: str = ".agent_directive.txt", mcp_config_filename: str = ".mcp_config.json")` — [`L251`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L251) — Write directive and MCP config to workspace, set both read-only.
  - `agent_memory_subdir(self)` — [`L65`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L65) — Cache subdir for agent memory (e.g. 'claude_memory'). Override for other backends.
  - `build_launch_cmd(self, directive_path: str, server_url: str, working_dir: str, *, dangerously_skip_permissions: bool = True, project_root: str | None = None, **kwargs)` — [`L81`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L81) — Build command, env, bootstrap prompt, and optional temp MCP config path.
  - `container_image(self)` — [`L70`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L70) — Docker image name for containerized runs. Override for other backends.
  - `devcontainer_build_context(self)` — [`L75`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L75) — Path to devcontainer build context (Dockerfile dir), relative to project root.
  - `get_resume_session_id(self, agent_memory_dir: Path)` — [`L128`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L128) — Return the session ID to resume from, or None if not found/supported.
  - `handle_stream_event(self, event: dict, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L104`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L104) — Process one stream event (e.g. system, assistant, user, result). Update metrics and optionally POST thinking to server.
  - `is_auth_fatal_error(self, text: str)` — [`L137`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L137) — Return True if text indicates a fatal auth error (e.g. expired OAuth token).
  - `log_cli_interaction(self, agent_memory_dir: Path, processed_hashes: set, last_cli_step: int, server_url: str | None = None)` — [`L114`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L114) — Log CLI interaction (steps/metrics) from backend-specific source (file, stream, etc.).
  - `name(self)` — [`L60`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L60) — Backend identifier (e.g. 'claude', 'codex').
  - `run_login(self)` — [`L133`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L133) — Run interactive login flow. Returns True on success.
  - `run_stream_reader(self, stdout_pipe, stop_event: threading.Event, log_file: io.TextIOWrapper | None, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L147`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L147) — Read stdout line-by-line (JSONL), tee to log_file, parse and handle events.
  - `seed_agent_auth(self, agent_memory_dir: Path)` — [`L142`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L142) — Seed container agent memory with host auth files. Override in subclasses.
- protocol/private: `_is_readonly`[`L268`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L268)
- uses (calls/refs, reference-scoped): [`get_llm_logger`](../data_persistence/llm_logger.md#get_llm_logger), [`handle_stream_event`](cli_agent_backends.md#HermesCliBackend.handle_stream_event), [`logger`](cli_agent_backends.md#logger), [`CliSessionMetrics`](cli_agent_backends.md#CliSessionMetrics), [`handle_stream_event`](cli_agent_backends.md#ClaudeCodeBackend.handle_stream_event), [`GeminiCliBackend`](cli_agent_backends.md#GeminiCliBackend), [`build_launch_cmd`](cli_agent_backends.md#GeminiCliBackend.build_launch_cmd), [`build_launch_cmd`](cli_agent_backends.md#ClaudeCodeBackend.build_launch_cmd), [`handle_stream_event`](cli_agent_backends.md#CodexCliBackend.handle_stream_event), [`handle_stream_event`](cli_agent_backends.md#GeminiCliBackend.handle_stream_event), [`build_launch_cmd`](cli_agent_backends.md#HermesCliBackend.build_launch_cmd), [`CodexCliBackend`](cli_agent_backends.md#CodexCliBackend), [`build_launch_cmd`](cli_agent_backends.md#CodexCliBackend.build_launch_cmd), [`log_cli_interaction`](cli_agent_backends.md#ClaudeCodeBackend.log_cli_interaction), [`log_cli_interaction`](cli_agent_backends.md#HermesCliBackend.log_cli_interaction), [`log_cli_interaction`](cli_agent_backends.md#GeminiCliBackend.log_cli_interaction), [`log_cli_interaction`](cli_agent_backends.md#CodexCliBackend.log_cli_interaction), [`HermesCliBackend`](cli_agent_backends.md#HermesCliBackend), [`ClaudeCodeBackend`](cli_agent_backends.md#ClaudeCodeBackend), [`get_cumulative_metrics`](../data_persistence/llm_logger.md#LLMLogger.get_cumulative_metrics), [`get_resume_session_id`](cli_agent_backends.md#CodexCliBackend.get_resume_session_id), [`get_resume_session_id`](cli_agent_backends.md#GeminiCliBackend.get_resume_session_id), [`name`](cli_agent_backends.md#GeminiCliBackend.name), [`name`](cli_agent_backends.md#HermesCliBackend.name), [`get_resume_session_id`](cli_agent_backends.md#HermesCliBackend.get_resume_session_id), [`seed_agent_auth`](cli_agent_backends.md#HermesCliBackend.seed_agent_auth), [`container_image`](cli_agent_backends.md#GeminiCliBackend.container_image), [`name`](cli_agent_backends.md#ClaudeCodeBackend.name), [`name`](cli_agent_backends.md#CodexCliBackend.name), [`_build_mcp_config_sse`](cli_agent_backends.md#GeminiCliBackend._build_mcp_config_sse), [`_build_mcp_config_stdio`](cli_agent_backends.md#GeminiCliBackend._build_mcp_config_stdio), [`agent_memory_subdir`](cli_agent_backends.md#GeminiCliBackend.agent_memory_subdir), [`container_image`](cli_agent_backends.md#ClaudeCodeBackend.container_image), [`container_image`](cli_agent_backends.md#CodexCliBackend.container_image), [`container_image`](cli_agent_backends.md#HermesCliBackend.container_image), [`devcontainer_build_context`](cli_agent_backends.md#GeminiCliBackend.devcontainer_build_context), [`is_auth_fatal_error`](cli_agent_backends.md#ClaudeCodeBackend.is_auth_fatal_error), [`is_auth_fatal_error`](cli_agent_backends.md#HermesCliBackend.is_auth_fatal_error), [`run_login`](cli_agent_backends.md#GeminiCliBackend.run_login), [`agent_memory_subdir`](cli_agent_backends.md#ClaudeCodeBackend.agent_memory_subdir)  (+12 more)
- used by: [`_run_agent_loop`](../../run_cli.md#_run_agent_loop), [`main`](../../run_cli.md#main), [`handle_stream_event`](cli_agent_backends.md#HermesCliBackend.handle_stream_event), [`GeminiCliBackend`](cli_agent_backends.md#GeminiCliBackend), [`build_launch_cmd`](cli_agent_backends.md#GeminiCliBackend.build_launch_cmd), [`build_launch_cmd`](cli_agent_backends.md#ClaudeCodeBackend.build_launch_cmd), [`get_backend`](cli_agent_backends.md#get_backend), [`build_launch_cmd`](cli_agent_backends.md#HermesCliBackend.build_launch_cmd), [`CodexCliBackend`](cli_agent_backends.md#CodexCliBackend), [`build_launch_cmd`](cli_agent_backends.md#CodexCliBackend.build_launch_cmd), [`log_cli_interaction`](cli_agent_backends.md#ClaudeCodeBackend.log_cli_interaction), [`_handle_item_mcp_tool_call`](cli_agent_backends.md#CodexCliBackend._handle_item_mcp_tool_call), [`log_cli_interaction`](cli_agent_backends.md#HermesCliBackend.log_cli_interaction), [`log_cli_interaction`](cli_agent_backends.md#GeminiCliBackend.log_cli_interaction), [`_handle_assistant_tool_use_block`](cli_agent_backends.md#ClaudeCodeBackend._handle_assistant_tool_use_block), [`_handle_gemini_tool_use`](cli_agent_backends.md#GeminiCliBackend._handle_gemini_tool_use), [`log_cli_interaction`](cli_agent_backends.md#CodexCliBackend.log_cli_interaction), [`_load_last_session_id`](../../run_cli.md#_load_last_session_id), [`HermesCliBackend`](cli_agent_backends.md#HermesCliBackend), [`ClaudeCodeBackend`](cli_agent_backends.md#ClaudeCodeBackend)  (4 test-only)

### `CliSession`
- def: [`utils/agent_infrastructure/cli_agent_backends.py:47`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L47)
- doc: Resources for a single CLI agent subprocess session.
- signature: `class CliSession:`
- members:
  - `process` — [`L49`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L49)
  - `stop_event` — [`L50`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L50)
  - `stream_thread` — [`L51`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L51)
  - `temp_mcp_config_path` — [`L52`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L52)
- used by: [`_run_agent_loop`](../../run_cli.md#_run_agent_loop), [`main`](../../run_cli.md#main), [`_cleanup_services`](../../run_cli.md#_cleanup_services), [`launch_cli_agent`](../../run_cli.md#launch_cli_agent), [`_cleanup_cli_session`](../../run_cli.md#_cleanup_cli_session)

### `CliSessionMetrics`
- def: [`utils/agent_infrastructure/cli_agent_backends.py:30`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L30) — documented in [utils-agent_infrastructure-cli_agent_backends](../../../concepts/utils-agent_infrastructure-cli_agent_backends.md)
- doc: Metrics collected from a single CLI agent session (e.g. stream-json result event).
- signature: `class CliSessionMetrics:`
- members:
  - `auth_fatal_error` — [`L43`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L43)
  - `duration_api_ms` — [`L39`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L39)
  - `duration_ms` — [`L38`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L38)
  - `error` — [`L41`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L41)
  - `input_tokens` — [`L35`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L35)
  - `is_error` — [`L40`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L40)
  - `model` — [`L33`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L33)
  - `num_turns` — [`L37`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L37)
  - `output_tokens` — [`L36`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L36)
  - `session_id` — [`L32`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L32)
  - `tool_use_count` — [`L42`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L42)
  - `total_cost_usd` — [`L34`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L34)
- used by: [`_run_agent_loop`](../../run_cli.md#_run_agent_loop), [`handle_stream_event`](cli_agent_backends.md#HermesCliBackend.handle_stream_event), [`handle_stream_event`](cli_agent_backends.md#ClaudeCodeBackend.handle_stream_event), [`handle_stream_event`](cli_agent_backends.md#CodexCliBackend.handle_stream_event), [`handle_stream_event`](cli_agent_backends.md#GeminiCliBackend.handle_stream_event), [`_handle_gemini_result`](cli_agent_backends.md#GeminiCliBackend._handle_gemini_result), [`_handle_item_mcp_tool_call`](cli_agent_backends.md#CodexCliBackend._handle_item_mcp_tool_call), [`_handle_assistant_tool_use_block`](cli_agent_backends.md#ClaudeCodeBackend._handle_assistant_tool_use_block), [`_handle_gemini_tool_use`](cli_agent_backends.md#GeminiCliBackend._handle_gemini_tool_use), [`launch_cli_agent`](../../run_cli.md#launch_cli_agent), [`_handle_assistant_text_block`](cli_agent_backends.md#ClaudeCodeBackend._handle_assistant_text_block), [`_handle_gemini_init`](cli_agent_backends.md#GeminiCliBackend._handle_gemini_init), [`handle_stream_event`](cli_agent_backends.md#CliAgentBackend.handle_stream_event), [`_handle_thread_started`](cli_agent_backends.md#CodexCliBackend._handle_thread_started), [`_handle_turn_completed`](cli_agent_backends.md#CodexCliBackend._handle_turn_completed), [`_handle_turn_failed`](cli_agent_backends.md#CodexCliBackend._handle_turn_failed), [`run_stream_reader`](cli_agent_backends.md#CliAgentBackend.run_stream_reader)  (22 test-only)

### `CodexCliBackend`  ·  implements/extends CliAgentBackend
- def: [`utils/agent_infrastructure/cli_agent_backends.py:1193`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1193)
- doc: Backend for OpenAI Codex CLI (codex exec --json, non-interactive only).
- signature: `class CodexCliBackend(CliAgentBackend):`
- members:
  - `_ensure_codex_config(self, agent_memory_dir: Path, mcp_sse_url: str | None = None, mcp_sse_port: int = 8002, *, server_url: str | None = None, project_root: str | None = None)` — [`L1260`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1260) — Ensure config.toml exists with MCP config. Use SSE url when containerized, stdio when local.
  - `_handle_error(self, event: dict)` — [`L1534`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1534) — Handle error event (may be transient reconnect notice).
  - `_handle_item_mcp_tool_call(self, event: dict, now: float, metrics: CliSessionMetrics | None, server_url: str | None)` — [`L1483`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1483) — Handle item.completed with item.type mcp_tool_call: tool_use count and _post_thinking.
  - `_handle_item_reasoning(self, event: dict, now: float, server_url: str | None)` — [`L1518`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1518) — Handle item.completed with item.type reasoning: buffer for next tool call.
  - `_handle_thread_started(self, event: dict, now: float, metrics: CliSessionMetrics | None)` — [`L1447`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1447) — Handle thread.started: set session_id from thread_id.
  - `_handle_turn_completed(self, event: dict, metrics: CliSessionMetrics | None)` — [`L1460`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1460) — Handle turn.completed: update metrics from usage.
  - `_handle_turn_failed(self, event: dict, metrics: CliSessionMetrics | None)` — [`L1476`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1476) — Handle turn.failed: set error state.
  - `agent_memory_subdir(self)` — [`L1211`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1211)
  - `build_launch_cmd(self, directive_path: str, server_url: str, working_dir: str, *, dangerously_skip_permissions: bool = True, project_root: str | None = None, containerized: bool = False, session_number: int = 1, resume_session_id: str | None = None, thinking_effort: str | None = None, mcp_sse_port: int | None = None, run_id: str | None = None, agent_memory_dir: str | None = None)` — [`L1337`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1337)
  - `container_image(self)` — [`L1215`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1215)
  - `devcontainer_build_context(self)` — [`L1219`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1219)
  - `get_resume_session_id(self, agent_memory_dir: Path)` — [`L1629`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1629) — Find the most recent Codex session ID from sessions dir.
  - `handle_stream_event(self, event: dict, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L1542`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1542) — Dispatch Codex exec --json events to typed handlers.
  - `is_auth_fatal_error(self, text: str)` — [`L1227`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1227) — Detect Codex auth failures (OpenRouter/API key or ChatGPT login).
  - `log_cli_interaction(self, agent_memory_dir: Path, processed_hashes: set, last_cli_step: int, server_url: str | None = None)` — [`L1568`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1568) — Poll Codex session JSONL files and append new entries as steps.
  - `name(self)` — [`L1207`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1207)
  - `run_login(self)` — [`L1641`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1641) — Run codex login if needed; no-op when using OpenRouter API key.
  - `seed_agent_auth(self, agent_memory_dir: Path)` — [`L1237`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1237) — Seed container with host Codex auth (credentials, config) if present.
  - `AGENT_MEMORY_PATH` — [`L1201`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1201)
  - `CONFIG_FILENAME` — [`L1203`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1203)
  - `DIRECTIVE_FILENAME` — [`L1202`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1202)
  - `SESSIONS_SUBDIR` — [`L1204`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1204)
  - `WORKSPACE_PATH` — [`L1200`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1200)
- protocol/private: `__init__`[`L1222`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1222), `_last_event_time`[`L1224`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1224), `_pending_reasoning`[`L1225`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1225)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`get_llm_logger`](../data_persistence/llm_logger.md#get_llm_logger), [`logger`](cli_agent_backends.md#logger), [`CliSessionMetrics`](cli_agent_backends.md#CliSessionMetrics), [`load_new_usage_entries`](../metric_tracking/codex_session_reader.md#load_new_usage_entries), [`append_cli_step`](../data_persistence/llm_logger.md#LLMLogger.append_cli_step), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`session_id`](cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`_sync_metrics_to_server`](cli_agent_backends.md#CliAgentBackend._sync_metrics_to_server), [`input_tokens`](cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](cli_agent_backends.md#CliAgentBackend._post_thinking), [`error`](cli_agent_backends.md#CliSessionMetrics.error), [`is_error`](cli_agent_backends.md#CliSessionMetrics.is_error), [`_build_bootstrap_content`](cli_agent_backends.md#CliAgentBackend._build_bootstrap_content)
- used by: [`get_backend`](cli_agent_backends.md#get_backend), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`handle_stream_event`](cli_agent_backends.md#CliAgentBackend.handle_stream_event), [`log_cli_interaction`](cli_agent_backends.md#CliAgentBackend.log_cli_interaction), [`name`](cli_agent_backends.md#CliAgentBackend.name), [`agent_memory_subdir`](cli_agent_backends.md#CliAgentBackend.agent_memory_subdir), [`devcontainer_build_context`](cli_agent_backends.md#CliAgentBackend.devcontainer_build_context), [`get_resume_session_id`](cli_agent_backends.md#CliAgentBackend.get_resume_session_id), [`run_login`](cli_agent_backends.md#CliAgentBackend.run_login), [`build_launch_cmd`](cli_agent_backends.md#CliAgentBackend.build_launch_cmd), [`container_image`](cli_agent_backends.md#CliAgentBackend.container_image), [`seed_agent_auth`](cli_agent_backends.md#CliAgentBackend.seed_agent_auth), [`is_auth_fatal_error`](cli_agent_backends.md#CliAgentBackend.is_auth_fatal_error)  (16 test-only)

### `GeminiCliBackend`  ·  implements/extends CliAgentBackend
- def: [`utils/agent_infrastructure/cli_agent_backends.py:763`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L763)
- doc: Backend for Google Gemini CLI (headless --output-format stream-json).
- signature: `class GeminiCliBackend(CliAgentBackend):`
- members:
  - `_build_settings(self, mcp_config: dict, telemetry_outfile: str, thinking_effort: str | None = None)` — [`L831`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L831) — Build a complete Gemini CLI settings.json.
  - `_handle_gemini_error(self, event: dict)` — [`L1049`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1049) — Handle error event: logging.
  - `_handle_gemini_init(self, event: dict, now: float, metrics: CliSessionMetrics | None)` — [`L990`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L990) — Handle init event: session metadata.
  - `_handle_gemini_message(self, event: dict, now: float)` — [`L1037`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1037) — Handle message event: logging (delta chunks at DEBUG).
  - `_handle_gemini_result(self, event: dict, metrics: CliSessionMetrics | None)` — [`L1054`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1054) — Handle result event: final metrics.
  - `_handle_gemini_tool_result(self, event: dict, now: float)` — [`L1030`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1030) — Handle tool_result event: logging.
  - `_handle_gemini_tool_use(self, event: dict, now: float, metrics: CliSessionMetrics | None, server_url: str | None)` — [`L1007`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1007) — Handle tool_use event: metrics, _post_thinking, logging.
  - `_write_gemini_settings(self, settings_dir: Path, mcp_config: dict, telemetry_outfile: str, thinking_effort: str | None = None)` — [`L867`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L867) — Write settings.json into the given directory. Returns the path.
  - `agent_memory_subdir(self)` — [`L782`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L782)
  - `build_launch_cmd(self, directive_path: str, server_url: str, working_dir: str, *, dangerously_skip_permissions: bool = True, project_root: str | None = None, containerized: bool = False, session_number: int = 1, resume_session_id: str | None = None, thinking_effort: str | None = None, mcp_sse_port: int | None = None, run_id: str | None = None, agent_memory_dir: str | None = None)` — [`L895`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L895)
  - `container_image(self)` — [`L786`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L786)
  - `devcontainer_build_context(self)` — [`L790`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L790)
  - `get_resume_session_id(self, agent_memory_dir: Path)` — [`L1166`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1166) — Find the most recent Gemini session ID from chat history.
  - `handle_stream_event(self, event: dict, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L1074`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1074) — Dispatch stream events to typed handlers (consistent with Claude backend).
  - `log_cli_interaction(self, agent_memory_dir: Path, processed_hashes: set, last_cli_step: int, server_url: str | None = None)` — [`L1101`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1101) — Poll Gemini session JSON files for new gemini messages and append steps.
  - `name(self)` — [`L778`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L778)
  - `run_login(self)` — [`L1188`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1188)
  - `AGENT_MEMORY_PATH` — [`L774`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L774)
  - `TELEMETRY_FILENAME` — [`L775`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L775)
  - `WORKSPACE_PATH` — [`L773`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L773)
- protocol/private: `__init__`[`L793`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L793), `_build_mcp_config_sse`[`L801`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L801), `_build_mcp_config_stdio`[`L812`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L812), `_last_event_time`[`L795`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L795)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`get_llm_logger`](../data_persistence/llm_logger.md#get_llm_logger), [`logger`](cli_agent_backends.md#logger), [`CliSessionMetrics`](cli_agent_backends.md#CliSessionMetrics), [`load_new_usage_entries`](../metric_tracking/gemini_session_reader.md#load_new_usage_entries), [`append_cli_step`](../data_persistence/llm_logger.md#LLMLogger.append_cli_step), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`session_id`](cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`_sync_metrics_to_server`](cli_agent_backends.md#CliAgentBackend._sync_metrics_to_server), [`input_tokens`](cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](cli_agent_backends.md#CliAgentBackend._post_thinking), [`model`](cli_agent_backends.md#CliSessionMetrics.model), [`error`](cli_agent_backends.md#CliSessionMetrics.error), [`is_error`](cli_agent_backends.md#CliSessionMetrics.is_error), [`_write_workspace_files`](cli_agent_backends.md#CliAgentBackend._write_workspace_files), [`_build_bootstrap_content`](cli_agent_backends.md#CliAgentBackend._build_bootstrap_content), [`duration_ms`](cli_agent_backends.md#CliSessionMetrics.duration_ms)
- used by: [`get_backend`](cli_agent_backends.md#get_backend), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`handle_stream_event`](cli_agent_backends.md#CliAgentBackend.handle_stream_event), [`log_cli_interaction`](cli_agent_backends.md#CliAgentBackend.log_cli_interaction), [`name`](cli_agent_backends.md#CliAgentBackend.name), [`agent_memory_subdir`](cli_agent_backends.md#CliAgentBackend.agent_memory_subdir), [`devcontainer_build_context`](cli_agent_backends.md#CliAgentBackend.devcontainer_build_context), [`get_resume_session_id`](cli_agent_backends.md#CliAgentBackend.get_resume_session_id), [`run_login`](cli_agent_backends.md#CliAgentBackend.run_login), [`build_launch_cmd`](cli_agent_backends.md#CliAgentBackend.build_launch_cmd), [`container_image`](cli_agent_backends.md#CliAgentBackend.container_image), [`_build_mcp_config_sse`](cli_agent_backends.md#CliAgentBackend._build_mcp_config_sse), [`_build_mcp_config_stdio`](cli_agent_backends.md#CliAgentBackend._build_mcp_config_stdio)  (25 test-only)

### `HermesCliBackend`  ·  implements/extends CliAgentBackend
- def: [`utils/agent_infrastructure/cli_agent_backends.py:1655`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1655)
- doc: Backend for the Nous Hermes agent, bridged through a local JSONL wrapper.
- signature: `class HermesCliBackend(CliAgentBackend):`
- members:
  - `agent_memory_subdir(self)` — [`L1671`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1671)
  - `build_launch_cmd(self, directive_path: str, server_url: str, working_dir: str, *, dangerously_skip_permissions: bool = True, project_root: str | None = None, containerized: bool = False, session_number: int = 1, resume_session_id: str | None = None, thinking_effort: str | None = None, mcp_sse_port: int | None = None, run_id: str | None = None, agent_memory_dir: str | None = None)` — [`L1846`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1846)
  - `container_image(self)` — [`L1675`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1675)
  - `devcontainer_build_context(self)` — [`L1679`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1679)
  - `get_resume_session_id(self, agent_memory_dir: Path)` — [`L2105`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L2105)
  - `handle_stream_event(self, event: dict, metrics: CliSessionMetrics | None, server_url: str | None = None)` — [`L1978`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1978)
  - `is_auth_fatal_error(self, text: str)` — [`L1687`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1687)
  - `log_cli_interaction(self, agent_memory_dir: Path, processed_hashes: set, last_cli_step: int, server_url: str | None = None)` — [`L2047`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L2047)
  - `name(self)` — [`L1667`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1667)
  - `run_login(self)` — [`L2110`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L2110)
  - `seed_agent_auth(self, agent_memory_dir: Path)` — [`L1703`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1703) — Seed run-local Hermes home from the user's ~/.hermes directory when present.
  - `AGENT_MEMORY_PATH` — [`L1660`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1660)
  - `CONFIG_FILENAME` — [`L1662`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1662)
  - `CONFIG_MARKER_BEGIN` — [`L1663`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1663)
  - `CONFIG_MARKER_END` — [`L1664`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1664)
  - `DIRECTIVE_FILENAME` — [`L1661`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1661)
  - `PROJECT_ROOT_PATH` — [`L1659`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1659)
  - `WORKSPACE_PATH` — [`L1658`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1658)
- protocol/private: `__init__`[`L1682`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1682), `_build_hermes_mcp_block`[`L1726`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1726), `_build_wrapper_cmd`[`L1789`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1789), `_ensure_hermes_config`[`L1758`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1758), `_last_event_time`[`L1684`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1684), `_last_seen_session_totals`[`L1685`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1685), `_normalize_tool_name`[`L1697`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L1697)
- uses (calls/refs, reference-scoped): [`cumulative_metrics`](../data_persistence/llm_logger.md#LLMLogger.cumulative_metrics), [`get_llm_logger`](../data_persistence/llm_logger.md#get_llm_logger), [`logger`](cli_agent_backends.md#logger), [`CliSessionMetrics`](cli_agent_backends.md#CliSessionMetrics), [`append_cli_step`](../data_persistence/llm_logger.md#LLMLogger.append_cli_step), [`load_new_usage_entries`](../metric_tracking/hermes_session_reader.md#load_new_usage_entries), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`session_id`](cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`_sync_metrics_to_server`](cli_agent_backends.md#CliAgentBackend._sync_metrics_to_server), [`input_tokens`](cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](cli_agent_backends.md#CliSessionMetrics.output_tokens), [`_post_thinking`](cli_agent_backends.md#CliAgentBackend._post_thinking), [`model`](cli_agent_backends.md#CliSessionMetrics.model), [`num_turns`](cli_agent_backends.md#CliSessionMetrics.num_turns), [`total_cost_usd`](cli_agent_backends.md#CliSessionMetrics.total_cost_usd), [`get_latest_session_id`](../metric_tracking/hermes_session_reader.md#get_latest_session_id), [`error`](cli_agent_backends.md#CliSessionMetrics.error), [`is_error`](cli_agent_backends.md#CliSessionMetrics.is_error), [`_build_bootstrap_content`](cli_agent_backends.md#CliAgentBackend._build_bootstrap_content), [`duration_ms`](cli_agent_backends.md#CliSessionMetrics.duration_ms), [`auth_fatal_error`](cli_agent_backends.md#CliSessionMetrics.auth_fatal_error), [`duration_api_ms`](cli_agent_backends.md#CliSessionMetrics.duration_api_ms)
- used by: [`get_backend`](cli_agent_backends.md#get_backend), [`CliAgentBackend`](cli_agent_backends.md#CliAgentBackend), [`handle_stream_event`](cli_agent_backends.md#CliAgentBackend.handle_stream_event), [`log_cli_interaction`](cli_agent_backends.md#CliAgentBackend.log_cli_interaction), [`name`](cli_agent_backends.md#CliAgentBackend.name), [`agent_memory_subdir`](cli_agent_backends.md#CliAgentBackend.agent_memory_subdir), [`devcontainer_build_context`](cli_agent_backends.md#CliAgentBackend.devcontainer_build_context), [`get_resume_session_id`](cli_agent_backends.md#CliAgentBackend.get_resume_session_id), [`run_login`](cli_agent_backends.md#CliAgentBackend.run_login), [`build_launch_cmd`](cli_agent_backends.md#CliAgentBackend.build_launch_cmd), [`container_image`](cli_agent_backends.md#CliAgentBackend.container_image), [`seed_agent_auth`](cli_agent_backends.md#CliAgentBackend.seed_agent_auth), [`is_auth_fatal_error`](cli_agent_backends.md#CliAgentBackend.is_auth_fatal_error)  (7 test-only)

## Functions
- `get_backend(cli_type: str)` — [`L2123`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L2123) — Return the backend for the given CLI type.

## Module values
- `logger` — [`L26`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/cli_agent_backends.py#L26)

