---
title: 'Module: tests/test_pokeagent_subagents.py'
type: catalog
provenance: extracted
module: tests/test_pokeagent_subagents.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_pokeagent_subagents`/
symbols:
  _make_agent: _make_agent().
  test_battler_consumes_global_steps_and_publishes_only_final_summary: test_battler_consumes_global_steps_and_publishes_only_final_summary().
  test_battler_accumulates_inner_turn_history: test_battler_accumulates_inner_turn_history().
  test_planner_consumes_global_steps: test_planner_consumes_global_steps().
  test_planner_initial_summarization: test_planner_initial_summarization().
  test_planner_accumulates_history_across_turns: test_planner_accumulates_history_across_turns().
  test_planner_failed_replan_continues_loop: test_planner_failed_replan_continues_loop().
  test_planner_safety_cap_at_25: test_planner_safety_cap_at_25().
  _state_payload: _state_payload().
  test_local_subagent_runner_can_log_metrics_with_stable_interaction_name: test_local_subagent_runner_can_log_metrics_with_stable_interaction_name().
  test_runtime_tracks_claims_and_publication: test_runtime_tracks_claims_and_publication().
  test_planner_calls_replan_and_exits: test_planner_calls_replan_and_exits().
  _POKE_MODULE: _POKE_MODULE.
  _build_adapter: _build_adapter().
  test_reflect_uses_toolless_local_subagent_and_trajectory_window: test_reflect_uses_toolless_local_subagent_and_trajectory_window().
  test_battler_vlm_inherits_system_instructions: test_battler_vlm_inherits_system_instructions().
  PlannerVLM.get_text_query: PlannerVLM#get_text_query().
  _planner_cache_key: _planner_cache_key().
  test_registry_exposes_renamed_subagent_tools_and_battler_surface: test_registry_exposes_renamed_subagent_tools_and_battler_surface().
  LoggingVLM.get_text_query: LoggingVLM#get_text_query().
  RecordingVLM: RecordingVLM#
  test_verify_returns_structured_verdict_for_categorized_objective: test_verify_returns_structured_verdict_for_categorized_objective().
  test_summarize_returns_summary_and_claims_step: test_summarize_returns_summary_and_claims_step().
  RecordingVLM.get_text_query: RecordingVLM#get_text_query().
  RecordingVLM.calls: RecordingVLM#calls.
  _write_trajectory_window: _write_trajectory_window().
  RecordingVLM.get_query: RecordingVLM#get_query().
  PlannerVLM: PlannerVLM#
  TestBuiltinToggle.test_include_builtins_true_has_all: TestBuiltinToggle#test_include_builtins_true_has_all().
  TestBuiltinToggle.test_include_builtins_false_excludes_builtins: TestBuiltinToggle#test_include_builtins_false_excludes_builtins().
  sys_path: sys_path.
  BattlerVLM.get_query: BattlerVLM#get_query().
  PlannerVLM.get_query: PlannerVLM#get_query().
  LoggingVLM: LoggingVLM#
  PlannerNoToolVLM.get_query: PlannerNoToolVLM#get_query().
  test_planner_safety_cap_at_25.AlwaysResearchVLM.get_query: test_planner_safety_cap_at_25().AlwaysResearchVLM#get_query().
  RecordingVLM.instances: RecordingVLM#instances.
  LoggingVLM.get_query: LoggingVLM#get_query().
  test_parse_verify_response_strips_markdown_json_fence: test_parse_verify_response_strips_markdown_json_fence().
  PlannerNoToolVLM.get_text_query: PlannerNoToolVLM#get_text_query().
  test_planner_safety_cap_at_25.AlwaysResearchVLM.get_text_query: test_planner_safety_cap_at_25().AlwaysResearchVLM#get_text_query().
  TestBuiltinToggle.test_include_builtins_false_keeps_generic_tools: TestBuiltinToggle#test_include_builtins_false_keeps_generic_tools().
  TestBuiltinToggle.test_default_includes_builtins: TestBuiltinToggle#test_default_includes_builtins().
  BattlerVLM: BattlerVLM#
  _make_agent._test_cache_path: _make_agent()._test_cache_path().
  PlannerVLM.calls: PlannerVLM#calls.
  PNG_BASE64: PNG_BASE64.
  BattlerVLM.calls: BattlerVLM#calls.
  _build_adapter.call_tool: _build_adapter().call_tool().
  test_local_subagent_runner_can_log_metrics_with_stable_interaction_name._get_cache_path: test_local_subagent_runner_can_log_metrics_with_stable_interaction_name()._get_cache_path().
  test_battler_consumes_global_steps_and_publishes_only_final_summary._get_cache_path: test_battler_consumes_global_steps_and_publishes_only_final_summary()._get_cache_path().
  test_battler_vlm_inherits_system_instructions.SpyVLM: test_battler_vlm_inherits_system_instructions().SpyVLM#
  test_battler_accumulates_inner_turn_history._get_cache_path: test_battler_accumulates_inner_turn_history()._get_cache_path().
  test_battler_accumulates_inner_turn_history.capturing_get_query: test_battler_accumulates_inner_turn_history().capturing_get_query().
  PlannerVLM.return_on_turn: PlannerVLM#return_on_turn.
  PlannerVLM._make_replan_response: PlannerVLM#_make_replan_response().
  PlannerVLM._make_research_response: PlannerVLM#_make_research_response().
  PlannerNoToolVLM.calls: PlannerNoToolVLM#calls.
  test_planner_consumes_global_steps._get_cache_path: test_planner_consumes_global_steps()._get_cache_path().
  test_planner_failed_replan_continues_loop.failing_then_succeeding_call_tool: test_planner_failed_replan_continues_loop().failing_then_succeeding_call_tool().
  test_planner_safety_cap_at_25.AlwaysResearchVLM: test_planner_safety_cap_at_25().AlwaysResearchVLM#
  AlwaysResearchVLM.calls: AlwaysResearchVLM#calls.
  test_planner_initial_summarization.spy_summarize: test_planner_initial_summarization().spy_summarize().
  test_planner_accumulates_history_across_turns.capturing_get_query: test_planner_accumulates_history_across_turns().capturing_get_query().
  RecordingVLM.__init__: RecordingVLM#__init__().
  RecordingVLM.args: RecordingVLM#args.
  RecordingVLM.kwargs: RecordingVLM#kwargs.
  BattlerVLM.__init__: BattlerVLM#__init__().
  test_battler_vlm_inherits_system_instructions.SpyVLM.__init__: test_battler_vlm_inherits_system_instructions().SpyVLM#__init__().
  SpyVLM.init_kwargs: SpyVLM#init_kwargs.
  test_battler_vlm_inherits_system_instructions.SpyVLM.get_query: test_battler_vlm_inherits_system_instructions().SpyVLM#get_query().
  test_battler_vlm_inherits_system_instructions.SpyVLM.get_text_query: test_battler_vlm_inherits_system_instructions().SpyVLM#get_text_query().
  PlannerVLM.__init__: PlannerVLM#__init__().
  PlannerVLM.replan_succeeds: PlannerVLM#replan_succeeds.
  PlannerNoToolVLM: PlannerNoToolVLM#
  PlannerNoToolVLM.__init__: PlannerNoToolVLM#__init__().
  test_planner_safety_cap_at_25.AlwaysResearchVLM.__init__: test_planner_safety_cap_at_25().AlwaysResearchVLM#__init__().
  TestBuiltinToggle: TestBuiltinToggle#
---
# Module: [`tests/test_pokeagent_subagents.py`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py)

## Classes
### `AlwaysResearchVLM`
- def: [`tests/test_pokeagent_subagents.py:672`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L672)
- signature: `class AlwaysResearchVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L676`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L676)
  - `get_text_query(self, prompt, interaction_name)` — [`L683`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L683)
  - `calls` — [`L674`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L674)
- protocol/private: `__init__`[`L673`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L673)
- used by: (1 test-only callers)

### `BattlerVLM`
- def: [`tests/test_pokeagent_subagents.py:92`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L92)
- signature: `class BattlerVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L96`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L96)
  - `calls` — [`L94`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L94)
- protocol/private: `__init__`[`L93`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L93)
- used by: (2 test-only callers)

### `LoggingVLM`  ·  implements/extends RecordingVLM
- def: [`tests/test_pokeagent_subagents.py:74`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L74)
- signature: `class LoggingVLM(RecordingVLM):`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L88`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L88)
  - `get_text_query(self, prompt, interaction_name)` — [`L75`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L75)
- uses (calls/refs, reference-scoped): [`get_llm_logger`](../utils/data_persistence/llm_logger.md#get_llm_logger), [`log_interaction`](../utils/data_persistence/llm_logger.md#LLMLogger.log_interaction)  (2 test-only)
- used by: (4 test-only callers)

### `PlannerNoToolVLM`
- def: [`tests/test_pokeagent_subagents.py:563`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L563)
- doc: VLM mock that returns no tool calls (tests safety break).
- signature: `class PlannerNoToolVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L569`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L569)
  - `get_text_query(self, prompt, interaction_name)` — [`L573`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L573)
  - `calls` — [`L567`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L567)
- protocol/private: `__init__`[`L566`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L566)

### `PlannerVLM`
- def: [`tests/test_pokeagent_subagents.py:521`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L521)
- doc: VLM mock that calls replan_objectives with return_to_orchestrator=true on its first turn.
- signature: `class PlannerVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L552`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L552)
  - `get_text_query(self, prompt, interaction_name)` — [`L556`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L556)
  - `calls` — [`L525`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L525)
  - `replan_succeeds` — [`L526`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L526)
  - `return_on_turn` — [`L527`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L527)
- protocol/private: `__init__`[`L524`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L524), `_make_replan_response`[`L529`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L529), `_make_research_response`[`L543`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L543)
- used by: (5 test-only callers)

### `RecordingVLM`
- def: [`tests/test_pokeagent_subagents.py:36`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L36)
- signature: `class RecordingVLM:`
- members:
  - `get_query(self, image, prompt, interaction_name)` — [`L69`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L69)
  - `get_text_query(self, prompt, interaction_name)` — [`L45`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L45)
  - `args` — [`L40`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L40)
  - `calls` — [`L42`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L42)
  - `instances` — [`L37`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L37)
  - `kwargs` — [`L41`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L41)
- protocol/private: `__init__`[`L39`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L39)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (4 test-only callers)

### `SpyVLM`
- def: [`tests/test_pokeagent_subagents.py:439`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L439)
- signature: `class SpyVLM:`
- members:
  - `get_query(self, img, prompt, name)` — [`L444`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L444)
  - `get_text_query(self, prompt, name)` — [`L447`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L447)
  - `init_kwargs` — [`L441`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L441)
- protocol/private: `__init__`[`L440`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L440)
- used by: (1 test-only callers)

### `TestBuiltinToggle`
- def: [`tests/test_pokeagent_subagents.py:751`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L751)
- doc: Tests for the include_builtins flag on build_local_subagent_tool_declarations.
- signature: `class TestBuiltinToggle:`
- members:
  - `test_default_includes_builtins(self)` — [`L772`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L772)
  - `test_include_builtins_false_excludes_builtins(self)` — [`L760`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L760)
  - `test_include_builtins_false_keeps_generic_tools(self)` — [`L766`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L766)
  - `test_include_builtins_true_has_all(self)` — [`L754`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L754)
- uses (calls/refs, reference-scoped): [`build_local_subagent_tool_declarations`](../agents/subagents/utils/registry.md#build_local_subagent_tool_declarations), [`BUILTIN_SUBAGENT_TOOL_NAMES`](../agents/subagents/utils/registry.md#BUILTIN_SUBAGENT_TOOL_NAMES.BUILTIN_SUBAGENT_TOOL_NAMES)

## Functions
- `_build_adapter(states=None)` — [`L145`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L145)
- `_get_cache_path(relative_path)` — [`L330`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L330)
- `_get_cache_path(relative_path)` — [`L393`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L393)
- `_get_cache_path(relative_path)` — [`L470`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L470)
- `_get_cache_path(relative_path)` — [`L589`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L589)
- `_make_agent(tmp_path, vlm_cls=RecordingVLM, adapter=None)` — [`L240`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L240)
- `_planner_cache_key()` — [`L577`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L577) — Build the cache key that _get_subagent_vlm uses for the planner VLM.
- `_state_payload(*, location: str, in_battle: bool, state_text: str)` — [`L105`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L105)
- `_test_cache_path(relative_path)` — [`L248`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L248)
- `_write_trajectory_window(run_manager: RunDataManager, steps: int = 4)` — [`L217`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L217)
- `call_tool(name, arguments)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L158)
- `capturing_get_query(image, prompt, interaction_name)` — [`L497`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L497)
- `capturing_get_query(image, prompt, interaction_name)` — [`L732`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L732)
- `failing_then_succeeding_call_tool(name, arguments)` — [`L641`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L641)
- `spy_summarize(args)` — [`L707`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L707)
- `test_battler_accumulates_inner_turn_history(tmp_path)` — [`L460`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L460) — Each battler turn should see the history of prior turns in its prompt.
- `test_battler_consumes_global_steps_and_publishes_only_final_summary(tmp_path)` — [`L389`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L389)
- `test_battler_vlm_inherits_system_instructions(tmp_path)` — [`L432`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L432) — The battler VLM must receive the orchestrator's system_instruction and only allowed tools.
- `test_local_subagent_runner_can_log_metrics_with_stable_interaction_name(tmp_path)` — [`L325`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L325)
- `test_parse_verify_response_strips_markdown_json_fence()` — [`L281`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L281)
- `test_planner_accumulates_history_across_turns(tmp_path)` — [`L720`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L720) — Subsequent planner turns should see prior tool call history in the prompt.
- `test_planner_calls_replan_and_exits(tmp_path)` — [`L617`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L617) — Planner exits when replan_objectives returns success with return_to_orchestrator=true.
- `test_planner_consumes_global_steps(tmp_path)` — [`L584`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L584) — Each planner turn claims a global step; nested summarize claims one too.
- `test_planner_failed_replan_continues_loop(tmp_path)` — [`L634`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L634) — When replan_objectives fails, the planner should keep looping (not exit).
- `test_planner_initial_summarization(tmp_path)` — [`L697`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L697) — The planner must call subagent_summarize before entering its main loop.
- `test_planner_safety_cap_at_25(tmp_path)` — [`L668`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L668) — If the planner never calls replan_objectives with return_to_orchestrator, it stops at the safety cap.
- `test_reflect_uses_toolless_local_subagent_and_trajectory_window(tmp_path)` — [`L265`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L265)
- `test_registry_exposes_renamed_subagent_tools_and_battler_surface()` — [`L373`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L373)
- `test_runtime_tracks_claims_and_publication()` — [`L351`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L351)
- `test_summarize_returns_summary_and_claims_step(tmp_path)` — [`L312`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L312)
- `test_verify_returns_structured_verdict_for_categorized_objective(tmp_path)` — [`L297`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L297)

## Module values
- `PNG_BASE64` — [`L32`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L32)
- `_POKE_MODULE` — [`L33`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L33)
- `sys_path` — [`L27`](../../../../../raw/code/continual-harness/tests/test_pokeagent_subagents.py#L27)

