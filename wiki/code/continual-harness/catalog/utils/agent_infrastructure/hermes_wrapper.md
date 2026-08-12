---
title: 'Module: utils/agent_infrastructure/hermes_wrapper.py'
type: catalog
provenance: extracted
module: utils/agent_infrastructure/hermes_wrapper.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.agent_infrastructure.hermes_wrapper`/
symbols:
  main: main().
  main._patch_agent_runtime._wrap_openai_client._wrap_create._wrapped: main()._patch_agent_runtime()._wrap_openai_client()._wrap_create()._wrapped().
  _debug_log: _debug_log().
  main._patch_agent_runtime: main()._patch_agent_runtime().
  _emit: _emit().
  main._build_multimodal_registry_handler._handler: main()._build_multimodal_registry_handler()._handler().
  main._patch_registered_mcp_handlers: main()._patch_registered_mcp_handlers().
  main._patch_agent_runtime._patched_build_api_kwargs: main()._patch_agent_runtime()._patched_build_api_kwargs().
  main.tool_progress_callback: main().tool_progress_callback().
  _to_namespace: _to_namespace().
  main._handle_signal: main()._handle_signal().
  main._patch_agent_runtime._wrap_openai_client._wrap_create: main()._patch_agent_runtime()._wrap_openai_client()._wrap_create().
  _extract_usage_snapshot: _extract_usage_snapshot().
  main._capture_usage_snapshot: main()._capture_usage_snapshot().
  main._patch_mcp_image_bridge: main()._patch_mcp_image_bridge().
  main._build_multimodal_registry_handler: main()._build_multimodal_registry_handler().
  main._build_multimodal_registry_handler._handler._call: main()._build_multimodal_registry_handler()._handler()._call().
  main._patch_agent_runtime._wrap_openai_client: main()._patch_agent_runtime()._wrap_openai_client().
  main._patch_agent_runtime._patched_create_openai_client: main()._patch_agent_runtime()._patched_create_openai_client().
  main._patch_agent_runtime._patched_build_assistant_message: main()._patch_agent_runtime()._patched_build_assistant_message().
  main.reasoning_callback: main().reasoning_callback().
  _coerce_mapping: _coerce_mapping().
  _normalize_tool_name: _normalize_tool_name().
  _read_text: _read_text().
  _build_initial_prompt: _build_initial_prompt().
  _append_jsonl: _append_jsonl().
  main._patch_agent_runtime._wrap_openai_client._wrap_create._count_images: main()._patch_agent_runtime()._wrap_openai_client()._wrap_create()._count_images().
  main._patch_agent_runtime._wrap_openai_client._wrap_create._strip_vision_messages: main()._patch_agent_runtime()._wrap_openai_client()._wrap_create()._strip_vision_messages().
  _extract_tool_reasoning: _extract_tool_reasoning().
---
# Module: [`utils/agent_infrastructure/hermes_wrapper.py`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py)

## Functions
- `_append_jsonl(path: Path, payload: dict[str, Any])` — [`L87`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L87)
- `_build_initial_prompt(directive_text: str, server_url: str, is_resume: bool)` — [`L44`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L44) — Build initial user message. Matches base _build_bootstrap_content runtime context.
- `_build_multimodal_registry_handler(server_name: str, tool_name: str, tool_timeout: float)` — [`L303`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L303)
- `_call()` — [`L325`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L325)
- `_capture_usage_snapshot(snapshot: dict[str, Any], session_id: str, model_name: str)` — [`L265`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L265)
- `_coerce_mapping(value: Any)` — [`L121`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L121)
- `_count_images(msgs)` — [`L487`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L487)
- `_debug_log(log_path: Path, hypothesis_id: str, location: str, message: str, data: dict[str, Any] | None = None, run_id: str = "")` — [`L94`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L94)
- `_emit(event: dict[str, Any])` — [`L31`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L31)
- `_extract_tool_reasoning(arguments: dict[str, Any])` — [`L72`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L72)
- `_extract_usage_snapshot(response: Any)` — [`L146`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L146)
- `_handle_signal(signum, _frame)` — [`L213`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L213)
- `_handler(args: dict, **kwargs)` — [`L306`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L306)
- `_normalize_tool_name(name: str)` — [`L80`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L80)
- `_patch_agent_runtime()` — [`L475`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L475)
- `_patch_mcp_image_bridge()` — [`L290`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L290)
- `_patch_registered_mcp_handlers(agent: Any)` — [`L440`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L440)
- `_patched_build_api_kwargs(self, api_messages: list[dict[str, Any]])` — [`L616`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L616)
- `_patched_build_assistant_message(self, assistant_message, finish_reason: str)` — [`L609`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L609)
- `_patched_create_openai_client(self, *client_args, **client_kwargs)` — [`L605`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L605)
- `_read_text(path: str | None)` — [`L35`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L35)
- `_strip_vision_messages(msgs)` — [`L507`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L507) — Remove synthetic user messages that carry image_url parts.
- `_to_namespace(value: Any)` — [`L138`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L138)
- `_wrap_create(call)` — [`L486`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L486)
- `_wrap_openai_client(client: Any)` — [`L480`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L480)
- `_wrapped(*call_args, **call_kwargs)` — [`L526`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L526)
- `main()` — [`L176`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L176)
- `reasoning_callback(reasoning_text: str)` — [`L713`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L713)
- `tool_progress_callback(tool_name: str, _preview: str, arguments: dict[str, Any])` — [`L695`](../../../../../../raw/code/continual-harness/utils/agent_infrastructure/hermes_wrapper.py#L695)

