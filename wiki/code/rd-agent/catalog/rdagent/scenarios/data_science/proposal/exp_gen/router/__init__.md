---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.router`/ParallelMultiTraceExpGen#
symbols:
  ParallelMultiTraceExpGen.async_gen: async_gen().
  ParallelMultiTraceExpGen.trace_scheduler: trace_scheduler.
  ParallelMultiTraceExpGen.planner: planner.
  ParallelMultiTraceExpGen.exp_gen: exp_gen.
  ParallelMultiTraceExpGen.gen: gen().
  ParallelMultiTraceExpGen.draft_exp_gen: draft_exp_gen.
  ParallelMultiTraceExpGen.merge_exp_gen: merge_exp_gen.
  ParallelMultiTraceExpGen.reset: reset().
  ParallelMultiTraceExpGen: ''
  ParallelMultiTraceExpGen.__init__: __init__().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py)

## Classes
### `ParallelMultiTraceExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py:36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L36)
- doc: An experiment generation strategy that enables parallel multi-trace exploration.
- signature: `class ParallelMultiTraceExpGen(ExpGen):`
- members:
  - `async_gen(self, trace: DSTrace, loop: LoopBase)` — [`L70`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L70) — Waits for a free execution slot, selects a parent trace using the — documented in [rdagent-app-data_science-conf](../../../../../../../concepts/rdagent-app-data_science-conf.md)
  - `gen(self, trace: DSTrace, plan: ExperimentPlan | None = None)` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L58)
  - `reset(self)` — [`L67`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L67)
  - `draft_exp_gen` — [`L49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L49)
  - `exp_gen` — [`L48`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L48)
  - `merge_exp_gen` — [`L50`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L50)
  - `planner` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L56)
  - `trace_scheduler` — [`L52`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L52)
- protocol/private: `__init__`[`L45`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/router/__init__.py#L45)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`Experiment`](../../../../../core/experiment.md#Experiment), [`DSExperiment`](../../../experiment/experiment.md#DSExperiment), [`log_object`](../../../../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../../../../core/conf.md#RD_AGENT_SETTINGS), [`gen`](../merge.md#ExpGen2Hypothesis.gen), [`DSTrace`](../base.md#DSTrace), [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`import_class`](../../../../../core/utils.md#import_class), [`gen`](../../../../../core/proposal.md#ExpGen.gen), [`gen`](../draft/draft.md#DSDraftV2ExpGen.gen), [`RD_Agent_TIMER_wrapper`](../../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`remain_time`](../../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../../log/timer.md#RDAgentTimerWrapper.timer), [`DSExperimentPlan`](../planner/__init__.md#DSExperimentPlan), [`scen`](../../../../../core/proposal.md#ExpGen.scen), [`DataScienceRDLoop`](../../../loop.md#DataScienceRDLoop), [`LoopBase`](../../../../../utils/workflow/loop.md#LoopBase), [`started`](../../../../../log/timer.md#RDAgentTimer.started), [`ExperimentPlan`](../../../../../core/experiment.md#ExperimentPlan), [`set_current_selection`](../../../../../core/proposal.md#Trace.set_current_selection), [`get_leaves`](../base.md#DSTrace.get_leaves), [`loop_idx`](../../../../../utils/workflow/loop.md#LoopBase.loop_idx), [`sota_experiment`](../base.md#DSTrace.sota_experiment), [`RDAgentTimer`](../../../../../log/timer.md#RDAgentTimer), [`sota_exp_to_submit`](../base.md#DSTrace.sota_exp_to_submit), [`exp2idx`](../../../../../core/proposal.md#Trace.exp2idx), [`__init__`](../../../../../core/proposal.md#ExpGen.__init__), [`get_max_parallel`](../../../../../core/conf.md#RDAgentSettings.get_max_parallel), [`get_unfinished_loop_cnt`](../../../../../utils/workflow/loop.md#LoopBase.get_unfinished_loop_cnt), [`default_exp_gen`](../../../loop.md#DataScienceRDLoop.default_exp_gen), [`merge_hours`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`coding_fail_reanalyze_threshold`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.coding_fail_reanalyze_threshold), [`consecutive_errors`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.consecutive_errors), [`next`](../trace_scheduler.md#TraceScheduler.next), [`register_uncommitted_exp`](../base.md#DSTrace.register_uncommitted_exp), [`ExpGen2Hypothesis`](../merge.md#ExpGen2Hypothesis), [`TraceScheduler`](../trace_scheduler.md#TraceScheduler)  (+11 more)
- used by: [`ExpGen`](../../../../../core/proposal.md#ExpGen), [`gen`](../../../../../core/proposal.md#ExpGen.gen), [`async_gen`](../../../../../core/proposal.md#ExpGen.async_gen), [`reset`](../../../../../core/proposal.md#ExpGen.reset)

