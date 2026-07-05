---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.planner`/DSExp
symbols:
  DSExpPlannerHandCraft.plan: PlannerHandCraft#plan().
  DSExperimentPlan: erimentPlan#
  DSExpPlannerHandCraft: PlannerHandCraft#
  DSExperimentPlan.__init__: erimentPlan#__init__().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py)

## Classes
### `DSExpPlannerHandCraft`  ·  implements/extends ExpPlanner
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py:22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py#L22)
- doc: A specific planner for data science experiments.
- signature: `class DSExpPlannerHandCraft(ExpPlanner[DSExperimentPlan]):`
- members:
  - `plan(self, trace: DSTrace)` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py#L27) — Generate a plan for the experiment based on the trace. — documented in [rdagent-log-timer](../../../../../../../concepts/rdagent-log-timer.md)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../../../../app/data_science/conf.md#DS_RD_SETTING), [`DSTrace`](../base.md#DSTrace), [`RD_Agent_TIMER_wrapper`](../../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`remain_time`](../../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../../log/timer.md#RDAgentTimerWrapper.timer), [`DSExperimentPlan`](__init__.md#DSExperimentPlan), [`started`](../../../../../log/timer.md#RDAgentTimer.started), [`all_duration`](../../../../../log/timer.md#RDAgentTimer.all_duration), [`sota_experiment`](../base.md#DSTrace.sota_experiment), [`ExpPlanner`](../../../../../core/proposal.md#ExpPlanner), [`model_architecture_suggestion_time_percent`](../../../../../app/data_science/conf.md#DataScienceBasePropSetting.model_architecture_suggestion_time_percent)
- used by: [`ExpPlanner`](../../../../../core/proposal.md#ExpPlanner), [`plan`](../../../../../core/proposal.md#ExpPlanner.plan)

### `DSExperimentPlan`  ·  implements/extends ExperimentPlan
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py:9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py#L9)
- doc: A specific plan for data science experiments.
- signature: `class DSExperimentPlan(ExperimentPlan):`
- protocol/private: `__init__`[`L15`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/planner/__init__.py#L15)
- uses (calls/refs, reference-scoped): [`ExperimentPlan`](../../../../../core/experiment.md#ExperimentPlan)
- used by: [`async_gen`](../router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](../proposal.md#DSProposalV2ExpGen.gen), [`gen`](../merge.md#ExpGen2TraceAndMergeV2.gen), [`gen`](../merge.md#ExpGen2Hypothesis.gen), [`gen`](../proposal.md#DSProposalV1ExpGen.gen), [`gen`](../draft/draft.md#DSDraftExpGen.gen), [`gen`](../merge.md#ExpGen2TraceAndMergeV3.gen), [`gen`](../merge.md#ExpGen2TraceAndMerge.gen), [`gen`](../draft/draft.md#DSDraftV2ExpGen.gen), [`gen`](../merge.md#MergeExpGen.gen), [`gen`](../merge.md#MergeExpGen_MultiTrace.gen), [`gen`](../naive.md#NaiveExpGen.gen), [`plan`](__init__.md#DSExpPlannerHandCraft.plan), [`ExperimentPlan`](../../../../../core/experiment.md#ExperimentPlan), [`DSExpPlannerHandCraft`](__init__.md#DSExpPlannerHandCraft)

