---
title: 'Module: tests/test_gemini_backend.py'
type: catalog
provenance: extracted
module: tests/test_gemini_backend.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_gemini_backend`/TestGemini
symbols:
  TestGeminiStreamEvents.test_result_event_updates_metrics: StreamEvents#test_result_event_updates_metrics().
  TestGeminiStreamEvents.test_init_event_sets_session_and_model: StreamEvents#test_init_event_sets_session_and_model().
  TestGeminiStreamEvents.test_tool_use_increments_count: StreamEvents#test_tool_use_increments_count().
  TestGeminiStreamEvents.test_tool_use_gemini_format_tool_name_parameters: StreamEvents#test_tool_use_gemini_format_tool_name_parameters().
  TestGeminiLogCliInteraction.test_appends_steps_to_llm_logger: LogCliInteraction#test_appends_steps_to_llm_logger().
  TestGeminiBackendProperties.test_get_backend_returns_gemini: BackendProperties#test_get_backend_returns_gemini().
  TestGeminiStreamEvents.test_tool_use_posts_reasoning_to_server: StreamEvents#test_tool_use_posts_reasoning_to_server().
  TestGeminiStreamEvents.test_error_event_does_not_crash: StreamEvents#test_error_event_does_not_crash().
  TestGeminiStreamEvents.test_message_event_does_not_crash: StreamEvents#test_message_event_does_not_crash().
  TestGeminiBackendProperties.test_agent_memory_subdir: BackendProperties#test_agent_memory_subdir().
  TestGeminiBackendProperties.test_container_image: BackendProperties#test_container_image().
  TestGeminiBackendProperties.test_devcontainer_build_context_exists: BackendProperties#test_devcontainer_build_context_exists().
  TestGeminiBuildLaunchCmd.test_local_cmd_structure: BuildLaunchCmd#test_local_cmd_structure().
  TestGeminiBuildLaunchCmd.test_local_writes_gemini_settings: BuildLaunchCmd#test_local_writes_gemini_settings().
  TestGeminiBuildLaunchCmd.test_thinking_effort_adds_model_config_overrides: BuildLaunchCmd#test_thinking_effort_adds_model_config_overrides().
  TestGeminiBuildLaunchCmd.test_resume_session_id_appended: BuildLaunchCmd#test_resume_session_id_appended().
  TestGeminiBuildLaunchCmd.test_containerized_requires_run_id: BuildLaunchCmd#test_containerized_requires_run_id().
  TestGeminiBuildLaunchCmd.test_containerized_cmd_has_docker: BuildLaunchCmd#test_containerized_cmd_has_docker().
  TestGeminiBuildLaunchCmd.test_containerized_writes_settings_to_agent_memory: BuildLaunchCmd#test_containerized_writes_settings_to_agent_memory().
  TestGeminiResumeSession.test_returns_none_for_empty_dir: ResumeSession#test_returns_none_for_empty_dir().
  TestGeminiResumeSession.test_finds_most_recent_session: ResumeSession#test_finds_most_recent_session().
  TestGeminiResumeSession.test_ignores_non_json_files: ResumeSession#test_ignores_non_json_files().
  TestGeminiRunLogin.test_always_returns_true: RunLogin#test_always_returns_true().
  TestGeminiLogCliInteraction.test_no_entries_returns_unchanged: LogCliInteraction#test_no_entries_returns_unchanged().
  TestGeminiLogCliInteraction._make_gemini_message: LogCliInteraction#_make_gemini_message().
  TestGeminiLogCliInteraction._make_session_with_messages: LogCliInteraction#_make_session_with_messages().
  TestGeminiBackendProperties: BackendProperties#
  TestGeminiBuildLaunchCmd: BuildLaunchCmd#
  TestGeminiStreamEvents: StreamEvents#
  TestGeminiResumeSession: ResumeSession#
  TestGeminiRunLogin: RunLogin#
  TestGeminiLogCliInteraction: LogCliInteraction#
---
# Module: [`tests/test_gemini_backend.py`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py)

## Classes
### `TestGeminiBackendProperties`
- def: [`tests/test_gemini_backend.py:22`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L22)
- signature: `class TestGeminiBackendProperties:`
- members:
  - `test_agent_memory_subdir(self)` — [`L28`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L28)
  - `test_container_image(self)` — [`L32`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L32)
  - `test_devcontainer_build_context_exists(self)` — [`L36`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L36)
  - `test_get_backend_returns_gemini(self)` — [`L23`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L23)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`get_backend`](../utils/agent_infrastructure/cli_agent_backends.md#get_backend), [`name`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.name), [`container_image`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.container_image), [`agent_memory_subdir`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.agent_memory_subdir), [`devcontainer_build_context`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.devcontainer_build_context)

### `TestGeminiBuildLaunchCmd`
- def: [`tests/test_gemini_backend.py:48`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L48)
- signature: `class TestGeminiBuildLaunchCmd:`
- members:
  - `test_containerized_cmd_has_docker(self, tmp_path)` — [`L126`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L126)
  - `test_containerized_requires_run_id(self, tmp_path)` — [`L118`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L118)
  - `test_containerized_writes_settings_to_agent_memory(self, tmp_path)` — [`L148`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L148)
  - `test_local_cmd_structure(self, tmp_path)` — [`L49`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L49)
  - `test_local_writes_gemini_settings(self, tmp_path)` — [`L67`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L67)
  - `test_resume_session_id_appended(self, tmp_path)` — [`L103`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L103)
  - `test_thinking_effort_adds_model_config_overrides(self, tmp_path)` — [`L82`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L82)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`build_launch_cmd`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.build_launch_cmd)

### `TestGeminiLogCliInteraction`
- def: [`tests/test_gemini_backend.py:295`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L295)
- signature: `class TestGeminiLogCliInteraction:`
- members:
  - `test_appends_steps_to_llm_logger(self, tmp_path, monkeypatch)` — [`L316`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L316)
  - `test_no_entries_returns_unchanged(self, tmp_path)` — [`L342`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L342)
- protocol/private: `_make_gemini_message`[`L299`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L299), `_make_session_with_messages`[`L296`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L296)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`log_cli_interaction`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.log_cli_interaction)

### `TestGeminiResumeSession`
- def: [`tests/test_gemini_backend.py:259`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L259)
- signature: `class TestGeminiResumeSession:`
- members:
  - `test_finds_most_recent_session(self, tmp_path)` — [`L264`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L264)
  - `test_ignores_non_json_files(self, tmp_path)` — [`L275`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L275)
  - `test_returns_none_for_empty_dir(self, tmp_path)` — [`L260`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L260)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`get_resume_session_id`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.get_resume_session_id)

### `TestGeminiRunLogin`
- def: [`tests/test_gemini_backend.py:286`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L286)
- signature: `class TestGeminiRunLogin:`
- members:
  - `test_always_returns_true(self)` — [`L287`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L287)
- uses (calls/refs, reference-scoped): [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`run_login`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.run_login)

### `TestGeminiStreamEvents`
- def: [`tests/test_gemini_backend.py:173`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L173)
- signature: `class TestGeminiStreamEvents:`
- members:
  - `test_error_event_does_not_crash(self)` — [`L239`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L239)
  - `test_init_event_sets_session_and_model(self)` — [`L174`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L174)
  - `test_message_event_does_not_crash(self)` — [`L247`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L247)
  - `test_result_event_updates_metrics(self)` — [`L225`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L225)
  - `test_tool_use_gemini_format_tool_name_parameters(self)` — [`L193`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L193) — Gemini stream-json uses tool_name and parameters.
  - `test_tool_use_increments_count(self)` — [`L184`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L184)
  - `test_tool_use_posts_reasoning_to_server(self)` — [`L203`](../../../../../raw/code/continual-harness/tests/test_gemini_backend.py#L203) — Tool use with reasoning in parameters is posted for UI streaming (like Claude).
- uses (calls/refs, reference-scoped): [`CliSessionMetrics`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics), [`GeminiCliBackend`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend), [`handle_stream_event`](../utils/agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.handle_stream_event), [`session_id`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.session_id), [`tool_use_count`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.tool_use_count), [`input_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.input_tokens), [`output_tokens`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.output_tokens), [`model`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.model), [`duration_ms`](../utils/agent_infrastructure/cli_agent_backends.md#CliSessionMetrics.duration_ms)

