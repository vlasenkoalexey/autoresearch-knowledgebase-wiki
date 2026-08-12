---
title: 'Module: agents/subagents/utils/runtime.py'
type: catalog
provenance: extracted
module: agents/subagents/utils/runtime.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.utils.runtime`/
symbols:
  PokeAgentRuntime.claim_step: PokeAgentRuntime#claim_step().
  PokeAgentRuntime.current_step: PokeAgentRuntime#current_step.
  PokeAgentRuntime.get_step_record: PokeAgentRuntime#get_step_record().
  PokeAgentRuntime._mark_record: PokeAgentRuntime#_mark_record().
  PokeAgentRuntime: PokeAgentRuntime#
  PokeAgentRuntime.publish_history: PokeAgentRuntime#publish_history().
  PokeAgentRuntime.__init__: PokeAgentRuntime#__init__().
  PokeAgentRuntime.publish_function_result: PokeAgentRuntime#publish_function_result().
  PokeAgentRuntime.sync_step: PokeAgentRuntime#sync_step().
  PokeAgentRuntime._records: PokeAgentRuntime#_records.
  PokeAgentRuntime.peek_next_step: PokeAgentRuntime#peek_next_step().
  PokeAgentRuntime._on_step_change: PokeAgentRuntime#_on_step_change.
  StepRecord: StepRecord#
  StepRecord.step_number: StepRecord#step_number.
  StepRecord.published_to_history: StepRecord#published_to_history.
  StepRecord.published_function_results: StepRecord#published_function_results.
  HistoryPublisher: HistoryPublisher.
  FunctionResultPublisher: FunctionResultPublisher.
  StepChangePublisher: StepChangePublisher.
  StepRecord.owner: StepRecord#owner.
  StepRecord.interaction_name: StepRecord#interaction_name.
  PokeAgentRuntime._publish_history: PokeAgentRuntime#_publish_history.
  PokeAgentRuntime._publish_function_result: PokeAgentRuntime#_publish_function_result.
---
# Module: [`agents/subagents/utils/runtime.py`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py)

## Classes
### `PokeAgentRuntime`
- def: [`agents/subagents/utils/runtime.py:24`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L24)
- doc: Owns global-step allocation and orchestrator publication boundaries.
- signature: `class PokeAgentRuntime:`
- members:
  - `claim_step(self, *, owner: str, interaction_name: str)` — [`L44`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L44)
  - `get_step_record(self, step_number: int)` — [`L92`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L92)
  - `peek_next_step(self)` — [`L41`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L41)
  - `publish_function_result(self, *, step_number: int, function_name: str, result_json: str)` — [`L88`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L88)
  - `publish_history(self, *, step_number: int, prompt: str, response: str, tool_calls: Optional[List[Dict[str, Any]]] = None, action_details: Optional[str] = None, player_coords: Optional[tuple[int, int]] = None, start_coords: Optional[tuple[int, int]] = None, end_coords: Optional[tuple[int, int]] = None)` — [`L64`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L64)
  - `sync_step(self, step_number: int)` — [`L58`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L58)
  - `current_step` — [`L35`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L35)
- protocol/private: `__init__`[`L27`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L27), `_mark_record`[`L98`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L98), `_on_step_change`[`L38`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L38), `_publish_function_result`[`L37`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L37), `_publish_history`[`L36`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L36), `_records`[`L39`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L39)
- uses (calls/refs, reference-scoped): [`StepRecord`](runtime.md#StepRecord), [`step_number`](runtime.md#StepRecord.step_number), [`published_function_results`](runtime.md#StepRecord.published_function_results), [`published_to_history`](runtime.md#StepRecord.published_to_history), [`FunctionResultPublisher`](runtime.md#FunctionResultPublisher), [`HistoryPublisher`](runtime.md#HistoryPublisher), [`StepChangePublisher`](runtime.md#StepChangePublisher), [`interaction_name`](runtime.md#StepRecord.interaction_name), [`owner`](runtime.md#StepRecord.owner)
- used by: [`run_step`](../../PokeAgent.md#PokeAgent.run_step), [`_run_planner_loop`](../../PokeAgent.md#PokeAgent._run_planner_loop), [`_run_battler_loop`](../../PokeAgent.md#PokeAgent._run_battler_loop), [`run`](../../PokeAgent.md#PokeAgent.run), [`runtime`](../../PokeAgent.md#PokeAgent.runtime), [`_run_one_step_subagent`](../../PokeAgent.md#PokeAgent._run_one_step_subagent)  (4 test-only)

### `StepRecord`
- def: [`agents/subagents/utils/runtime.py:16`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L16)
- signature: `class StepRecord:`
- members:
  - `interaction_name` — [`L19`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L19)
  - `owner` — [`L18`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L18)
  - `published_function_results` — [`L21`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L21)
  - `published_to_history` — [`L20`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L20)
  - `step_number` — [`L17`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L17)
- used by: [`claim_step`](runtime.md#PokeAgentRuntime.claim_step), [`_mark_record`](runtime.md#PokeAgentRuntime._mark_record), [`get_step_record`](runtime.md#PokeAgentRuntime.get_step_record), [`_records`](runtime.md#PokeAgentRuntime._records)  (1 test-only)

## Module values
- `FunctionResultPublisher` — [`L11`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L11)
- `HistoryPublisher` — [`L10`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L10)
- `StepChangePublisher` — [`L12`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/runtime.py#L12)

