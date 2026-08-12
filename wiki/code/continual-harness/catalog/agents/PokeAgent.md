---
title: 'Module: agents/PokeAgent.py'
type: catalog
provenance: extracted
module: agents/PokeAgent.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.PokeAgent`/
symbols:
  logger: logger.
  PokeAgent.run_step: PokeAgent#run_step().
  PokeAgent._run_planner_loop: PokeAgent#_run_planner_loop().
  PokeAgent._run_battler_loop: PokeAgent#_run_battler_loop().
  PokeAgent.run: PokeAgent#run().
  PokeAgent.harness_evolver: PokeAgent#harness_evolver.
  PokeAgent.runtime: PokeAgent#runtime.
  PokeAgent._build_structured_prompt: PokeAgent#_build_structured_prompt().
  PokeAgent._execute_function_call: PokeAgent#_execute_function_call().
  PokeAgent._build_optimized_prompt: PokeAgent#_build_optimized_prompt().
  PokeAgent._get_subagent_vlm: PokeAgent#_get_subagent_vlm().
  PokeAgent.executor: PokeAgent#executor.
  PokeAgent._execute_builtin_subagent_by_registry_id: PokeAgent#_execute_builtin_subagent_by_registry_id().
  PokeAgent._execute_subagent_summarize: PokeAgent#_execute_subagent_summarize().
  PokeAgent._run_one_step_subagent: PokeAgent#_run_one_step_subagent().
  PokeAgent: PokeAgent#
  PokeAgent._execute_subagent_gym_puzzle: PokeAgent#_execute_subagent_gym_puzzle().
  PokeAgent._execute_subagent_red_puzzle: PokeAgent#_execute_subagent_red_puzzle().
  PokeAgent._execute_function_call_by_name: PokeAgent#_execute_function_call_by_name().
  PokeAgent._execute_subagent_cleanup_run_artifacts: PokeAgent#_execute_subagent_cleanup_run_artifacts().
  PokeAgent._execute_subagent_verify: PokeAgent#_execute_subagent_verify().
  PokeAgent._execute_subagent_plan_objectives: PokeAgent#_execute_subagent_plan_objectives().
  PokeAgent.mcp_adapter: PokeAgent#mcp_adapter.
  PokeAgent._execute_subagent_reflect: PokeAgent#_execute_subagent_reflect().
  PokeAgent._execute_subagent_battler: PokeAgent#_execute_subagent_battler().
  MCPToolAdapter.call_tool: MCPToolAdapter#call_tool().
  PokeAgent.vlm: PokeAgent#vlm.
  PokeAgent._subagent_vlm_cache: PokeAgent#_subagent_vlm_cache.
  PokeAgent._load_base_prompt: PokeAgent#_load_base_prompt().
  PokeAgent.step_count: PokeAgent#step_count.
  PokeAgent._execute_run_skill: PokeAgent#_execute_run_skill().
  PokeAgent._execute_evolve_harness: PokeAgent#_execute_evolve_harness().
  PokeAgent._gather_store_context: PokeAgent#_gather_store_context().
  _SIMPLEST_SCAFFOLD: _SIMPLEST_SCAFFOLD.
  PokeAgent._handle_vlm_function_calls: PokeAgent#_handle_vlm_function_calls().
  PokeAgent.server_url: PokeAgent#server_url.
  PokeAgent.conversation_history: PokeAgent#conversation_history.
  PokeAgent._store_function_result_for_context: PokeAgent#_store_function_result_for_context().
  PokeAgent._log_thinking: PokeAgent#_log_thinking().
  PokeAgent.prompt_optimizer: PokeAgent#prompt_optimizer.
  PokeAgent._wait_for_actions_complete: PokeAgent#_wait_for_actions_complete().
  PokeAgent.backend: PokeAgent#backend.
  PokeAgent.scaffold: PokeAgent#scaffold.
  PokeAgent._execute_custom_subagent: PokeAgent#_execute_custom_subagent().
  PokeAgent.call: PokeAgent#call().
  PokeAgent._format_action_history: PokeAgent#_format_action_history().
  PokeAgent.tools: PokeAgent#tools.
  PokeAgent.llm_logger: PokeAgent#llm_logger.
  PokeAgent._load_system_instructions: PokeAgent#_load_system_instructions().
  PokeAgent._load_bootstrap_prompt: PokeAgent#_load_bootstrap_prompt().
  PokeAgent._create_tool_declarations: PokeAgent#_create_tool_declarations().
  PokeAgent._add_to_history: PokeAgent#_add_to_history().
  PokeAgent.check_prerequisites: PokeAgent#check_prerequisites().
  PokeAgent._get_memory_context: PokeAgent#_get_memory_context().
  PokeAgent._get_skill_context: PokeAgent#_get_skill_context().
  PokeAgent._get_subagent_context: PokeAgent#_get_subagent_context().
  PokeAgent.model: PokeAgent#model.
  PokeAgent.optimization_window_length: PokeAgent#optimization_window_length.
  PokeAgent.recent_function_results: PokeAgent#recent_function_results.
  PokeAgent._log_trajectory_for_step: PokeAgent#_log_trajectory_for_step().
  PokeAgent._execute_run_code: PokeAgent#_execute_run_code().
  PokeAgent._extract_text_from_response: PokeAgent#_extract_text_from_response().
  PokeAgent._bootstrap_prompt_content: PokeAgent#_bootstrap_prompt_content.
  PokeAgent._convert_protobuf_args: PokeAgent#_convert_protobuf_args().
  PokeAgent._get_function_results_context: PokeAgent#_get_function_results_context().
  PokeAgent.include_builtins: PokeAgent#include_builtins.
  PokeAgent._normalize_replan_objectives_arguments: PokeAgent#_normalize_replan_objectives_arguments().
  PokeAgent.call_vlm_with_image: PokeAgent#call_vlm_with_image().
  PokeAgent.call_vlm_with_text: PokeAgent#call_vlm_with_text().
  main: main().
  PokeAgent.system_instructions: PokeAgent#system_instructions.
  PokeAgent._inject_evolution_summary: PokeAgent#_inject_evolution_summary().
  PokeAgent.max_steps: PokeAgent#max_steps.
  PokeAgent._execute_process_trajectory_history: PokeAgent#_execute_process_trajectory_history().
  PokeAgent._send_thinking_to_server: PokeAgent#_send_thinking_to_server().
  PokeAgent._load_bootstrap_addendum: PokeAgent#_load_bootstrap_addendum().
  PokeAgent._tool_caller: PokeAgent#_tool_caller().
  PokeAgent._format_history_for_display: PokeAgent#_format_history_for_display().
  ACTION_HISTORY_WINDOW: ACTION_HISTORY_WINDOW.
  PokeAgent.optimization_enabled: PokeAgent#optimization_enabled.
  PokeAgent.bootstrap_prompt_path: PokeAgent#bootstrap_prompt_path.
  PokeAgent._local_subagent_vlm: PokeAgent#_local_subagent_vlm.
  PokeAgent.format_objective: PokeAgent#format_objective().
  PokeAgent._calculate_context_size: PokeAgent#_calculate_context_size().
  PokeAgent._is_black_frame: PokeAgent#_is_black_frame().
  MCPToolAdapter: MCPToolAdapter#
  PokeAgent._BUILTIN_VLM_KEYS: PokeAgent#_BUILTIN_VLM_KEYS.
  PokeAgent.__init__: PokeAgent#__init__().
  PokeAgent._convert_protobuf_value: PokeAgent#_convert_protobuf_value().
  _NO_BUILTINS_SCAFFOLDS: _NO_BUILTINS_SCAFFOLDS.
  PokeAgent.bootstrap_active: PokeAgent#bootstrap_active.
  PokeAgent.format_battling_group: PokeAgent#format_battling_group().
  PokeAgent._is_title_sequence: PokeAgent#_is_title_sequence().
  PokeAgent._strip_map_info: PokeAgent#_strip_map_info().
  MCPToolAdapter.server_url: MCPToolAdapter#server_url.
  PokeAgent.max_context_chars: PokeAgent#max_context_chars.
  PokeAgent.target_context_chars: PokeAgent#target_context_chars.
  PokeAgent._VLM_CACHE_CAP: PokeAgent#_VLM_CACHE_CAP.
  PokeAgent._metrics_safe_subagent_args: PokeAgent#_metrics_safe_subagent_args().
  PokeAgent._extract_recommended_next_action: PokeAgent#_extract_recommended_next_action().
  MCPToolAdapter.__init__: MCPToolAdapter#__init__().
  PokeAgent.bootstrap_from: PokeAgent#bootstrap_from.
---
# Module: [`agents/PokeAgent.py`](../../../../../raw/code/continual-harness/agents/PokeAgent.py)

## Classes
### `MCPToolAdapter`
- def: [`agents/PokeAgent.py:99`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L99)
- doc: Adapter to call MCP server tools via HTTP.
- signature: `class MCPToolAdapter:`
- members:
  - `call_tool(self, tool_name: str, arguments: Dict[str, Any])` — [`L105`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L105) — Call an MCP tool via HTTP request to the game server.
  - `server_url` — [`L103`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L103)
- protocol/private: `__init__`[`L102`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L102)
- uses (calls/refs, reference-scoped): [`logger`](PokeAgent.md#logger)
- used by: [`run_step`](PokeAgent.md#PokeAgent.run_step), [`_run_planner_loop`](PokeAgent.md#PokeAgent._run_planner_loop), [`_execute_function_call`](PokeAgent.md#PokeAgent._execute_function_call), [`_execute_subagent_gym_puzzle`](PokeAgent.md#PokeAgent._execute_subagent_gym_puzzle), [`_execute_subagent_red_puzzle`](PokeAgent.md#PokeAgent._execute_subagent_red_puzzle), [`_execute_function_call_by_name`](PokeAgent.md#PokeAgent._execute_function_call_by_name), [`_execute_subagent_plan_objectives`](PokeAgent.md#PokeAgent._execute_subagent_plan_objectives), [`mcp_adapter`](PokeAgent.md#PokeAgent.mcp_adapter), [`_execute_subagent_battler`](PokeAgent.md#PokeAgent._execute_subagent_battler), [`call`](PokeAgent.md#PokeAgent.call), [`_get_memory_context`](PokeAgent.md#PokeAgent._get_memory_context), [`_get_skill_context`](PokeAgent.md#PokeAgent._get_skill_context), [`_get_subagent_context`](PokeAgent.md#PokeAgent._get_subagent_context)  (1 test-only)

### `PokeAgent`
- def: [`agents/PokeAgent.py:177`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L177)
- doc: Custom benchmark agent using Gemini API directly with all MCP tools available.
- signature: `class PokeAgent:`
- members:
  - `_add_to_history(self, prompt: str, response: str, tool_calls: List[Dict] = None, action_details: str = None, player_coords: tuple = None, start_coords: tuple = None, end_coords: tuple = None, step_number: Optional[int] = None)` — [`L1498`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1498) — Add interaction to conversation history - ONLY stores LLM responses and actions.
  - `_build_optimized_prompt(self, game_state_result: str, step_count: int)` — [`L2380`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2380) — Build optimized prompt by combining base_prompt.md with current game context.
  - `_build_structured_prompt(self, game_state_result: str, step_count: int)` — [`L2638`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2638) — Build an autonomous prompt that emphasizes creating your own objectives.
  - `_calculate_context_size(self)` — [`L1563`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1563) — Calculate total character count of conversation history.
  - `_convert_protobuf_args(self, proto_args)` — [`L1427`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1427) — Convert protobuf arguments to JSON-serializable Python types.
  - `_convert_protobuf_value(self, value)` — [`L1423`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1423) — Recursively convert a protobuf value to JSON-serializable Python types.
  - `_create_tool_declarations(self)` — [`L390`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L390) — Build Gemini-compatible tool declarations from the centralized registry.
  - `_execute_builtin_subagent_by_registry_id(self, subagent_id: str, arguments: dict)` — [`L772`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L772) — If *subagent_id* is a built-in registry entry, run native handler; else None.
  - `_execute_custom_subagent(self, arguments: dict)` — [`L755`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L755) — Launch a custom subagent (from registry or inline config).
  - `_execute_evolve_harness(self, arguments: dict)` — [`L521`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L521) — Trigger an on-demand evolution pass.
  - `_execute_function_call(self, function_call, allowed_tool_names: Optional[set[str]] = None)` — [`L1444`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1444) — Execute a function call and return the result as JSON string.
  - `_execute_function_call_by_name(self, function_name: str, arguments: dict)` — [`L396`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L396) — Execute a function by name with given arguments and return result as JSON string.
  - `_execute_process_trajectory_history(self, arguments: dict)` — [`L817`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L817) — One-step VLM analysis on a trajectory window with a directive.
  - `_execute_run_code(self, arguments: dict)` — [`L542`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L542) — Execute arbitrary Python code in the game sandbox for prototyping/debugging.
  - `_execute_run_skill(self, arguments: dict)` — [`L421`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L421) — Execute a skill's code in a sandbox with access to game tools.
  - `_execute_subagent_battler(self, arguments: dict)` — [`L1079`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1079) — Delegate the active battle to a local looping battler.
  - `_execute_subagent_cleanup_run_artifacts(self, arguments: dict)` — [`L1034`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1034) — Remove cache/run files and/or dated top-level dirs (deterministic; optional dry_run).
  - `_execute_subagent_gym_puzzle(self, arguments: dict)` — [`L910`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L910) — Execute gym puzzle solving using a lightweight local subagent.
  - `_execute_subagent_plan_objectives(self, arguments: dict)` — [`L1242`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1242) — Delegate objective planning/replanning to the local planner loop.
  - `_execute_subagent_red_puzzle(self, arguments: dict)` — [`L953`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L953) — Execute Red puzzle solving using a lightweight local subagent.
  - `_execute_subagent_reflect(self, arguments: dict)` — [`L831`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L831) — Execute reflection using a local, tool-less subagent.
  - `_execute_subagent_summarize(self, arguments: dict)` — [`L996`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L996) — Summarize the latest trajectory window without an extra compaction layer.
  - `_execute_subagent_verify(self, arguments: dict)` — [`L872`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L872) — Execute objective verification using a local, tool-less subagent.
  - `_extract_text_from_response(self, response)` — [`L3240`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L3240) — Extract text content from response
  - `_format_action_history(self)` — [`L2952`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2952) — Format short-term memory (last ACTION_HISTORY_WINDOW steps) with full tool details.
  - `_format_history_for_display(self)` — [`L1574`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1574) — Format conversation history for display.
  - `_gather_store_context(self)` — [`L2364`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2364) — Fetch memory, skill, and subagent overviews, gated by scaffold.
  - `_get_function_results_context(self)` — [`L2272`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2272) — Format recent function results for inclusion in prompt.
  - `_get_memory_context(self, **_kwargs)` — [`L2300`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2300) — Fetch the memory tree overview for inclusion in the prompt.
  - `_get_skill_context(self)` — [`L2328`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2328) — Fetch the skill library tree overview for inclusion in the prompt.
  - `_get_subagent_context(self)` — [`L2346`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2346) — Fetch the subagent registry tree overview for inclusion in the prompt.
  - `_get_subagent_vlm(self, tool_names: Optional[set[str]] = None, supplemental_tools: Optional[list[dict]] = None, *, pinned: bool = False)` — [`L633`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L633) — Lazily create cached VLMs for local subagents with LRU eviction.
  - `_handle_vlm_function_calls(self, response, tool_calls_made, tool_call_count, max_tool_calls, allowed_tool_names: Optional[set[str]] = None)` — [`L3117`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L3117) — Handle function calls from VLM backend
  - `_inject_evolution_summary(self, results: dict)` — [`L2229`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2229) — Inject a human-readable evolution summary so the orchestrator sees what changed.
  - `_is_black_frame(self, image)` — [`L2881`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2881) — Check if frame is a black screen (transition)
  - `_is_title_sequence(self, game_state_data: Dict[str, Any])` — [`L2828`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2828) — Detect if in title sequence
  - `_load_base_prompt(self)` — [`L327`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L327) — Load base prompt (strategic guidance) from file.
  - `_load_bootstrap_addendum(self)` — [`L378`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L378) — Load the bootstrap addendum prompt that tells the agent about bootstrapped content.
  - `_load_bootstrap_prompt(self)` — [`L364`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L364) — Read the bootstrapped evolved prompt file, if one was provided.
  - `_load_system_instructions(self, filename: str)` — [`L311`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L311) — Load system instructions from file.
  - `_log_thinking(self, prompt: str, response: str, duration: float = None, tool_calls: list = None, step_number: Optional[int] = None)` — [`L2206`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2206) — Log interaction to LLM logger with full tool call history.
  - `_log_trajectory_for_step(self, run_manager, step_num: int, pre_state: dict, prompt: str, reasoning: str, tool_calls: list, response: str)` — [`L2914`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2914) — Log trajectory for a CLI agent step.
  - `_metrics_safe_subagent_args(arguments: Optional[Dict[str, Any]], *, keys: tuple[str, ...])` — [`L703`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L703) — Copy selected orchestrator tool args for cumulative_metrics (truncate long strings).
  - `_normalize_replan_objectives_arguments(self, arguments: Dict[str, Any])` — [`L1431`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1431) — Coerce replan_objectives ``edits`` to ``list[dict]`` for JSON/MCP and DOM validation.
  - `_run_one_step_subagent(self, *, prompt: str, interaction_name: str, current_image=None, orchestrator_args: Optional[Dict[str, Any]] = None, metrics_arg_keys: Optional[tuple[str, ...]] = None)` — [`L720`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L720) — Run a one-step local subagent with its own claimed global step.
  - `_send_thinking_to_server(self, thinking_text: str, step_num: int)` — [`L1625`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1625) — Send agent thinking to server for display in stream.
  - `_store_function_result_for_context(self, function_name: str, result_json: str)` — [`L2258`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2258) — Store function result to include in next step's context.
  - `_strip_map_info(self, state_text: str)` — [`L2851`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2851) — Strip map/navigation information from state text during title sequence
  - `_wait_for_actions_complete(self, timeout: int = 30)` — [`L2140`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2140) — Wait for all queued actions to complete before proceeding.
  - `call(**kwargs)` — [`L466`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L466)
  - `call_vlm_with_image()` — [`L1751`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1751)
  - `call_vlm_with_text()` — [`L1791`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1791)
  - `check_prerequisites(self)` — [`L1594`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1594) — Check if prerequisites are met.
  - `format_battling_group(group_list)` — [`L2456`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2456)
  - `format_objective(obj_dict, category_emoji, category_name)` — [`L2430`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2430)
  - `run(self)` — [`L2997`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L2997) — Run the autonomous agent loop. — documented in [agents-PokeAgent](../../concepts/agents-PokeAgent.md)
  - `run_step(self, prompt: str, max_tool_calls: int = 5, screenshot_b64: str = None, step_number: Optional[int] = None)` — [`L1643`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1643) — Run a single agent step. — documented in [agents-PokeAgent](../../concepts/agents-PokeAgent.md)
  - `backend` — [`L198`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L198)
  - `bootstrap_active` — [`L209`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L209)
  - `bootstrap_from` — [`L210`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L210)
  - `bootstrap_prompt_path` — [`L211`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L211)
  - `conversation_history` — [`L214`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L214)
  - `executor` — [`L263`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L263)
  - `harness_evolver` — [`L282`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L282)
  - `include_builtins` — [`L206`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L206)
  - `llm_logger` — [`L260`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L260)
  - `max_context_chars` — [`L201`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L201)
  - `max_steps` — [`L199`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L199)
  - `mcp_adapter` — [`L244`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L244)
  - `model` — [`L197`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L197)
  - `optimization_enabled` — [`L203`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L203)
  - `optimization_window_length` — [`L204`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L204)
  - `prompt_optimizer` — [`L281`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L281)
  - `recent_function_results` — [`L218`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L218)
  - `runtime` — [`L222`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L222)
  - `scaffold` — [`L205`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L205)
  - `server_url` — [`L196`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L196)
  - `step_count` — [`L200`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L200)
  - `system_instructions` — [`L241`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L241)
  - `target_context_chars` — [`L202`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L202)
  - `tools` — [`L248`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L248)
  - `vlm` — [`L249`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L249)
- protocol/private: `_BUILTIN_VLM_KEYS`[`L631`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L631), `_VLM_CACHE_CAP`[`L220`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L220), `__init__`[`L180`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L180), `_bootstrap_prompt_content`[`L278`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L278), `_extract_recommended_next_action`[`L821`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L821), `_local_subagent_vlm`[`L221`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L221), `_run_battler_loop`[`L1122`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1122), `_run_planner_loop`[`L1289`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L1289), `_subagent_vlm_cache`[`L219`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L219), `_tool_caller`[`L465`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L465)
- uses (calls/refs, reference-scoped): [`logger`](PokeAgent.md#logger), [`get_llm_logger`](../utils/data_persistence/llm_logger.md#get_llm_logger), [`run_run_artifact_cleanup`](../utils/run_artifact_cleanup.md#run_run_artifact_cleanup), [`get_run_data_manager`](../utils/data_persistence/run_data_manager.md#get_run_data_manager), [`as_dict`](../utils/run_artifact_cleanup.md#CleanupResult.as_dict), [`optimize_prompt`](utils/prompt_optimizer.md#PromptOptimizer.optimize_prompt), [`get`](../utils/stores/base_store.md#BaseStore.get), [`evolve`](utils/harness_evolver.md#HarnessEvolver.evolve), [`build_tools_for_scaffold`](tools/registry.md#build_tools_for_scaffold), [`load_subagent_context`](subagents/utils/context.md#load_subagent_context), [`claim_step`](subagents/utils/runtime.md#PokeAgentRuntime.claim_step), [`convert_protobuf_value`](../utils/json_utils.md#convert_protobuf_value), [`call_tool`](PokeAgent.md#MCPToolAdapter.call_tool), [`run_id`](../utils/data_persistence/run_data_manager.md#RunDataManager.run_id), [`get_text_query`](../utils/agent_infrastructure/vlm_backends.md#VLM.get_text_query), [`log_interaction`](../utils/data_persistence/llm_logger.md#LLMLogger.log_interaction), [`update_server_metrics`](../utils/metric_tracking/server_metrics.md#update_server_metrics), [`clamp_trajectory_window`](subagents/utils/trajectory_window.md#clamp_trajectory_window), [`POKEAGENT_PROMPT_PATH`](prompts/paths.md#POKEAGENT_PROMPT_PATH), [`normalize_replan_edits`](../utils/json_utils.md#normalize_replan_edits), [`CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH`](prompts/paths.md#CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH), [`get_skill_store`](../utils/stores/skills.md#get_skill_store), [`initialize_run_data_manager`](../utils/data_persistence/run_data_manager.md#initialize_run_data_manager), [`_SIMPLEST_SCAFFOLD`](PokeAgent.md#_SIMPLEST_SCAFFOLD), [`get_subagent_store`](../utils/stores/subagents.md#get_subagent_store), [`get_query`](../utils/agent_infrastructure/vlm_backends.md#VLM.get_query), [`VLM`](../utils/agent_infrastructure/vlm_backends.md#VLM), [`CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH`](prompts/paths.md#CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH), [`build_reflect_prompt`](subagents/reflect.md#build_reflect_prompt), [`execute_custom_subagent`](subagents/utils/executor.md#SubagentExecutor.execute_custom_subagent), [`get_local_subagent_spec`](subagents/utils/registry.md#get_local_subagent_spec), [`handler_method`](subagents/utils/registry.md#LocalSubagentSpec.handler_method), [`name`](../utils/stores/skills.md#SkillEntry.name), [`render_prompt`](prompts/paths.md#render_prompt), [`should_evolve`](utils/harness_evolver.md#HarnessEvolver.should_evolve), [`add_step_tool_calls`](../utils/data_persistence/llm_logger.md#LLMLogger.add_step_tool_calls), [`prompt_optimizer`](utils/harness_evolver.md#HarnessEvolver.prompt_optimizer), [`name`](../utils/stores/subagents.md#SubagentEntry.name), [`parse_verify_response`](subagents/verify.md#parse_verify_response), [`process_trajectory_history`](subagents/utils/executor.md#SubagentExecutor.process_trajectory_history)  (+47 more)
- used by: [`main`](PokeAgent.md#main)  (25 test-only)

## Functions
- `main()` — [`L3263`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L3263) — Main entry point.

## Module values
- `ACTION_HISTORY_WINDOW` — [`L96`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L96)
- `_NO_BUILTINS_SCAFFOLDS` — [`L86`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L86)
- `_SIMPLEST_SCAFFOLD` — [`L87`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L87)
- `logger` — [`L93`](../../../../../raw/code/continual-harness/agents/PokeAgent.py#L93)

