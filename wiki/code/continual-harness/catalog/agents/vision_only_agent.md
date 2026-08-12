---
title: 'Module: agents/vision_only_agent.py'
type: catalog
provenance: extracted
module: agents/vision_only_agent.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.vision_only_agent`/
symbols:
  logger: logger.
  VisionOnlyAgent.run_step: VisionOnlyAgent#run_step().
  VisionOnlyAgent.run: VisionOnlyAgent#run().
  VisionOnlyAgent._execute_reflect: VisionOnlyAgent#_execute_reflect().
  VisionOnlyAgent.step_count: VisionOnlyAgent#step_count.
  VisionOnlyAgent.vlm: VisionOnlyAgent#vlm.
  VisionOnlyAgent._run_local_subagent: VisionOnlyAgent#_run_local_subagent().
  VisionOnlyAgent._add_to_history: VisionOnlyAgent#_add_to_history().
  MCPToolAdapter.call_tool: MCPToolAdapter#call_tool().
  VisionOnlyAgent._local_subagent_vlm: VisionOnlyAgent#_local_subagent_vlm.
  VisionOnlyAgent.model: VisionOnlyAgent#model.
  VisionOnlyAgent.conversation_history: VisionOnlyAgent#conversation_history.
  VisionOnlyAgent._build_structured_prompt: VisionOnlyAgent#_build_structured_prompt().
  VisionOnlyAgent._handle_vertex_function_calls: VisionOnlyAgent#_handle_vertex_function_calls().
  VisionOnlyAgent.allow_slam: VisionOnlyAgent#allow_slam.
  VisionOnlyAgent._execute_function_call_by_name: VisionOnlyAgent#_execute_function_call_by_name().
  VisionOnlyAgent._execute_function_call: VisionOnlyAgent#_execute_function_call().
  VisionOnlyAgent.server_url: VisionOnlyAgent#server_url.
  VisionOnlyAgent._create_tool_declarations: VisionOnlyAgent#_create_tool_declarations().
  VisionOnlyAgent.check_prerequisites: VisionOnlyAgent#check_prerequisites().
  main: main().
  VisionOnlyAgent._load_system_instructions: VisionOnlyAgent#_load_system_instructions().
  VisionOnlyAgent.backend: VisionOnlyAgent#backend.
  VisionOnlyAgent._send_thinking_to_server: VisionOnlyAgent#_send_thinking_to_server().
  VisionOnlyAgent._wait_for_actions_complete: VisionOnlyAgent#_wait_for_actions_complete().
  VisionOnlyAgent.call_vlm_with_image: VisionOnlyAgent#call_vlm_with_image().
  VisionOnlyAgent.call_vlm_with_text: VisionOnlyAgent#call_vlm_with_text().
  VisionOnlyAgent.tools: VisionOnlyAgent#tools.
  VisionOnlyAgent._convert_protobuf_args: VisionOnlyAgent#_convert_protobuf_args().
  VisionOnlyAgent.max_steps: VisionOnlyAgent#max_steps.
  VisionOnlyAgent.mcp_adapter: VisionOnlyAgent#mcp_adapter.
  VisionOnlyAgent: VisionOnlyAgent#
  VisionOnlyAgent._extract_text_from_response: VisionOnlyAgent#_extract_text_from_response().
  MCPToolAdapter._convert_protobuf_to_native: MCPToolAdapter#_convert_protobuf_to_native().
  VisionOnlyAgent._get_local_subagent_vlm: VisionOnlyAgent#_get_local_subagent_vlm().
  VisionOnlyAgent._is_black_frame: VisionOnlyAgent#_is_black_frame().
  VisionOnlyAgent._format_action_history: VisionOnlyAgent#_format_action_history().
  MCPToolAdapter: MCPToolAdapter#
  VisionOnlyAgent.__init__: VisionOnlyAgent#__init__().
  VisionOnlyAgent.llm_logger: VisionOnlyAgent#llm_logger.
  VisionOnlyAgent._calculate_context_size: VisionOnlyAgent#_calculate_context_size().
  VisionOnlyAgent._format_history_for_display: VisionOnlyAgent#_format_history_for_display().
  VisionOnlyAgent.allow_walkthrough: VisionOnlyAgent#allow_walkthrough.
  VisionOnlyAgent.system_instructions: VisionOnlyAgent#system_instructions.
  MCPToolAdapter.server_url: MCPToolAdapter#server_url.
  MCPToolAdapter.print_game_state: MCPToolAdapter#print_game_state.
  MCPToolAdapter.__init__: MCPToolAdapter#__init__().
  VisionOnlyAgent.max_context_chars: VisionOnlyAgent#max_context_chars.
  VisionOnlyAgent.target_context_chars: VisionOnlyAgent#target_context_chars.
---
# Module: [`agents/vision_only_agent.py`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py)

## Classes
### `MCPToolAdapter`
- def: [`agents/vision_only_agent.py:53`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L53)
- doc: Adapter to call MCP server tools via HTTP.
- signature: `class MCPToolAdapter:`
- members:
  - `_convert_protobuf_to_native(self, value)` — [`L60`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L60) — Recursively convert protobuf objects to native Python types.
  - `call_tool(self, tool_name: str, arguments: Dict[str, Any])` — [`L64`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L64) — Call an MCP tool via HTTP request to the game server.
  - `print_game_state` — [`L58`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L58)
  - `server_url` — [`L57`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L57)
- protocol/private: `__init__`[`L56`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L56)
- uses (calls/refs, reference-scoped): [`logger`](vision_only_agent.md#logger), [`convert_protobuf_value`](../utils/json_utils.md#convert_protobuf_value)
- used by: [`_execute_function_call_by_name`](vision_only_agent.md#VisionOnlyAgent._execute_function_call_by_name), [`mcp_adapter`](vision_only_agent.md#VisionOnlyAgent.mcp_adapter)  (1 test-only)

### `VisionOnlyAgent`
- def: [`agents/vision_only_agent.py:143`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L143)
- doc: Vision-Only CLI Agent - uses only visual input without map data or pathfinding.
- signature: `class VisionOnlyAgent:`
- members:
  - `_add_to_history(self, prompt: str, response: str, tool_calls: List[Dict] = None, action_details: str = None, player_coords: tuple = None)` — [`L574`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L574) — Add interaction to conversation history - ONLY stores LLM responses and actions.
  - `_build_structured_prompt(self, game_state_result: str, step_count: int)` — [`L1125`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1125) — Build a prompt WITHOUT map information.
  - `_calculate_context_size(self)` — [`L615`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L615) — Calculate total character count of conversation history.
  - `_convert_protobuf_args(self, proto_args)` — [`L556`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L556) — Convert protobuf arguments to JSON-serializable Python types.
  - `_create_tool_declarations(self)` — [`L211`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L211) — Create Gemini function declarations for MCP tools (NO NAVIGATE_TO).
  - `_execute_function_call(self, function_call)` — [`L560`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L560) — Execute a function call and return the result as JSON string.
  - `_execute_function_call_by_name(self, function_name: str, arguments: dict)` — [`L460`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L460) — Execute a function by name with given arguments and return result as JSON string.
  - `_execute_reflect(self, arguments: dict)` — [`L472`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L472) — Execute reflection using agent's own VLM to analyze situation.
  - `_extract_text_from_response(self, response)` — [`L1708`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1708) — Extract text content from response
  - `_format_action_history(self)` — [`L1539`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1539) — Format action history - shows only LLM thinking and actions taken.
  - `_format_history_for_display(self)` — [`L626`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L626) — Format conversation history for display.
  - `_get_local_subagent_vlm(self)` — [`L533`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L533) — Lazily create a tool-less VLM for one-step subagents.
  - `_handle_vertex_function_calls(self, response, tool_calls_made, tool_call_count, max_tool_calls)` — [`L1669`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1669) — Handle function calls from VertexAI backend
  - `_is_black_frame(self, image)` — [`L1515`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1515) — Check if frame is a black screen (transition)
  - `_load_system_instructions(self, filename: str)` — [`L198`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L198) — Load system instructions from file.
  - `_run_local_subagent(self, *, prompt: str, interaction_name: str, current_image=None)` — [`L543`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L543) — Run a one-step subagent with tools disabled.
  - `_send_thinking_to_server(self, thinking_text: str, step_num: int)` — [`L676`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L676) — Send agent thinking to server for display in stream.
  - `_wait_for_actions_complete(self, timeout: int = 30)` — [`L1097`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1097) — Wait for all queued actions to complete before proceeding.
  - `call_vlm_with_image()` — [`L755`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L755)
  - `call_vlm_with_text()` — [`L796`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L796)
  - `check_prerequisites(self)` — [`L647`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L647) — Check if prerequisites are met.
  - `run(self)` — [`L1562`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1562) — Run the agent loop.
  - `run_step(self, prompt: str, max_tool_calls: int = 5, screenshot_b64: str = None)` — [`L694`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L694) — Run a single agent step.
  - `allow_slam` — [`L167`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L167)
  - `allow_walkthrough` — [`L166`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L166)
  - `backend` — [`L161`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L161)
  - `conversation_history` — [`L174`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L174)
  - `llm_logger` — [`L196`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L196)
  - `max_context_chars` — [`L164`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L164)
  - `max_steps` — [`L162`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L162)
  - `mcp_adapter` — [`L180`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L180)
  - `model` — [`L160`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L160)
  - `server_url` — [`L159`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L159)
  - `step_count` — [`L163`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L163)
  - `system_instructions` — [`L177`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L177)
  - `target_context_chars` — [`L165`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L165)
  - `tools` — [`L184`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L184)
  - `vlm` — [`L185`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L185)
- protocol/private: `__init__`[`L146`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L146), `_local_subagent_vlm`[`L536`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L536)
- uses (calls/refs, reference-scoped): [`logger`](vision_only_agent.md#logger), [`get_llm_logger`](../utils/data_persistence/llm_logger.md#get_llm_logger), [`get_run_data_manager`](../utils/data_persistence/run_data_manager.md#get_run_data_manager), [`load_subagent_context`](subagents/utils/context.md#load_subagent_context), [`GAME_NAME`](prompts/paths.md#GAME_NAME), [`get_text_query`](../utils/agent_infrastructure/vlm_backends.md#VLM.get_text_query), [`update_server_metrics`](../utils/metric_tracking/server_metrics.md#update_server_metrics), [`clamp_trajectory_window`](subagents/utils/trajectory_window.md#clamp_trajectory_window), [`POKEAGENT_PROMPT_PATH`](prompts/paths.md#POKEAGENT_PROMPT_PATH), [`get_query`](../utils/agent_infrastructure/vlm_backends.md#VLM.get_query), [`VLM`](../utils/agent_infrastructure/vlm_backends.md#VLM), [`build_reflect_prompt`](subagents/reflect.md#build_reflect_prompt), [`call_tool`](vision_only_agent.md#MCPToolAdapter.call_tool), [`resolve_repo_path`](prompts/paths.md#resolve_repo_path), [`convert_protobuf_args`](../utils/json_utils.md#convert_protobuf_args), [`MCPToolAdapter`](vision_only_agent.md#MCPToolAdapter)
- used by: [`main`](vision_only_agent.md#main)  (1 test-only)

## Functions
- `main()` — [`L1731`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L1731) — Main entry point.

## Module values
- `logger` — [`L50`](../../../../../raw/code/continual-harness/agents/vision_only_agent.py#L50)

