---
title: 'Module: rdagent/log/timer.py'
type: catalog
provenance: extracted
module: rdagent/log/timer.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.timer`/RD
symbols:
  RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper: _Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper.
  RDAgentTimerWrapper.timer: AgentTimerWrapper#timer.
  RDAgentTimer.remain_time: AgentTimer#remain_time().
  RDAgentTimer.started: AgentTimer#started.
  RDAgentTimer.all_duration: AgentTimer#all_duration.
  RDAgentTimer.add_duration: AgentTimer#add_duration().
  RDAgentTimer.restart_by_remain_time: AgentTimer#restart_by_remain_time().
  RDAgentTimer.reset: AgentTimer#reset().
  RDAgentTimer: AgentTimer#
  RDAgentTimer.update_remain_time: AgentTimer#update_remain_time().
  RDAgentTimerWrapper.replace_timer: AgentTimerWrapper#replace_timer().
  RDAgentTimer.is_timeout: AgentTimer#is_timeout().
  RDAgentTimer.target_time: AgentTimer#target_time.
  RDAgentTimer._remain_time_duration: AgentTimer#_remain_time_duration.
  RDAgentTimerWrapper: AgentTimerWrapper#
  RDAgentTimerWrapper.api_fail_count: AgentTimerWrapper#api_fail_count.
  RDAgentTimerWrapper.latest_api_fail_time: AgentTimerWrapper#latest_api_fail_time.
  RDAgentTimer.__init__: AgentTimer#__init__().
  RDAgentTimerWrapper.__init__: AgentTimerWrapper#__init__().
---
# Module: [`rdagent/log/timer.py`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py)

## Classes
### `RDAgentTimer`
- def: [`rdagent/log/timer.py:8`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L8) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
- signature: `class RDAgentTimer:`
- members:
  - `add_duration(self, duration: timedelta)` — [`L50`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L50) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `is_timeout(self)` — [`L56`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L56) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `remain_time(self)` — [`L68`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L68) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `reset(self, all_duration: str | timedelta)` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L15) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `restart_by_remain_time(self)` — [`L41`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L41) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `update_remain_time(self)` — [`L63`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L63) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `all_duration` — [`L12`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L12)
  - `started` — [`L10`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L10) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `target_time` — [`L11`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L11) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
- protocol/private: `__init__`[`L9`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L9), `_remain_time_duration`[`L13`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L13)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](__init__.md#rdagent_logger.rdagent_logger), [`info`](logger.md#RDAgentLog.info), [`warning`](logger.md#RDAgentLog.warning)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`run`](../utils/workflow/loop.md#LoopBase.run), [`_try_create_chat_completion_or_embedding`](../oai/backend/base.md#APIBackend._try_create_chat_completion_or_embedding), [`load`](../utils/workflow/loop.md#LoopBase.load), [`hypothesis_rewrite`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`log_workflow_state`](../utils/workflow/tracking.md#WorkflowTracker.log_workflow_state), [`real_full_timeout`](../scenarios/data_science/scen/__init__.md#DataScienceScen.real_full_timeout), [`_check_exit_conditions_on_step`](../utils/workflow/loop.md#LoopBase._check_exit_conditions_on_step), [`timer`](timer.md#RDAgentTimerWrapper.timer), [`plan`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExpPlannerHandCraft.plan), [`set_time_limit`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector.set_time_limit), [`timer`](../utils/workflow/loop.md#LoopBase.timer), [`dump`](../utils/workflow/loop.md#LoopBase.dump), [`get_first_session_file_after_duration`](utils/folder.md#get_first_session_file_after_duration), [`replace_timer`](timer.md#RDAgentTimerWrapper.replace_timer), [`global_timer`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector.global_timer)

### `RDAgentTimerWrapper`  ·  implements/extends SingletonBaseClass
- def: [`rdagent/log/timer.py:75`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L75) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
- signature: `class RDAgentTimerWrapper(SingletonBaseClass):`
- members:
  - `replace_timer(self, timer: RDAgentTimer)` — [`L81`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L81) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
  - `api_fail_count` — [`L78`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L78)
  - `latest_api_fail_time` — [`L79`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L79)
  - `timer` — [`L77`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L77) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
- protocol/private: `__init__`[`L76`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L76)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](__init__.md#rdagent_logger.rdagent_logger), [`info`](logger.md#RDAgentLog.info), [`SingletonBaseClass`](../core/utils.md#SingletonBaseClass), [`RDAgentTimer`](timer.md#RDAgentTimer)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`async_gen`](../scenarios/data_science/proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`hypothesis_select_with_llm`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_select_with_llm), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../scenarios/data_science/proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.gen), [`_try_create_chat_completion_or_embedding`](../oai/backend/base.md#APIBackend._try_create_chat_completion_or_embedding), [`load`](../utils/workflow/loop.md#LoopBase.load), [`hypothesis_rewrite`](../scenarios/data_science/proposal/exp_gen/proposal.md#DSProposalV2ExpGen.hypothesis_rewrite), [`RD_Agent_TIMER_wrapper`](timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`log_workflow_state`](../utils/workflow/tracking.md#WorkflowTracker.log_workflow_state), [`real_full_timeout`](../scenarios/data_science/scen/__init__.md#DataScienceScen.real_full_timeout), [`SingletonBaseClass`](../core/utils.md#SingletonBaseClass), [`plan`](../scenarios/data_science/proposal/exp_gen/planner/__init__.md#DSExpPlannerHandCraft.plan), [`timer`](../utils/workflow/loop.md#LoopBase.timer), [`dump`](../utils/workflow/loop.md#LoopBase.dump), [`global_timer`](../scenarios/data_science/proposal/exp_gen/select/expand.md#LimitTimeCKPSelector.global_timer)

## Module values
- `RD_Agent_TIMER_wrapper` — [`L86`](../../../../../../raw/code/rd-agent/rdagent/log/timer.py#L86) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)

