---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/merge.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/merge.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.merge`/
symbols:
  ExpGen2TraceAndMergeV2.gen: ExpGen2TraceAndMergeV2#gen().
  ExpGen2Hypothesis.gen: ExpGen2Hypothesis#gen().
  ExpGen2TraceAndMergeV3.gen: ExpGen2TraceAndMergeV3#gen().
  ExpGen2TraceAndMerge.gen: ExpGen2TraceAndMerge#gen().
  MergeExpGen.gen: MergeExpGen#gen().
  MergeExpGen_MultiTrace.gen: MergeExpGen_MultiTrace#gen().
  ExpGen2Hypothesis.get_exp_index: ExpGen2Hypothesis#get_exp_index().
  ExpGen2Hypothesis.hypothesis_gen: ExpGen2Hypothesis#hypothesis_gen().
  ExpGen2TraceAndMergeV2.exp_gen: ExpGen2TraceAndMergeV2#exp_gen.
  ExpGen2TraceAndMerge.exp_gen: ExpGen2TraceAndMerge#exp_gen.
  ExpGen2TraceAndMergeV3.exp_gen: ExpGen2TraceAndMergeV3#exp_gen.
  ExpGen2TraceAndMerge.merge_exp_gen: ExpGen2TraceAndMerge#merge_exp_gen.
  ExpGen2TraceAndMergeV2.merge_exp_gen: ExpGen2TraceAndMergeV2#merge_exp_gen.
  ExpGen2TraceAndMergeV3.merge_exp_gen: ExpGen2TraceAndMergeV3#merge_exp_gen.
  ExpGen2Hypothesis: ExpGen2Hypothesis#
  MergeExpGen: MergeExpGen#
  MergeExpGen_MultiTrace: MergeExpGen_MultiTrace#
  ExpGen2TraceAndMergeV2.reset_exp_gen_version: ExpGen2TraceAndMergeV2#reset_exp_gen_version().
  ExpGen2TraceAndMerge: ExpGen2TraceAndMerge#
  ExpGen2TraceAndMerge.__init__: ExpGen2TraceAndMerge#__init__().
  ExpGen2TraceAndMergeV2: ExpGen2TraceAndMergeV2#
  ExpGen2TraceAndMergeV2.__init__: ExpGen2TraceAndMergeV2#__init__().
  ExpGen2TraceAndMergeV3: ExpGen2TraceAndMergeV3#
  ExpGen2TraceAndMergeV3.__init__: ExpGen2TraceAndMergeV3#__init__().
  ExpGen2TraceAndMergeV2.flag_start_merge: ExpGen2TraceAndMergeV2#flag_start_merge.
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py)

## Classes
### `ExpGen2Hypothesis`  ·  implements/extends DSProposalV2ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:99`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L99)
- signature: `class ExpGen2Hypothesis(DSProposalV2ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L148`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L148) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
  - `get_exp_index(self, trace: DSTrace)` — [`L131`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L131)
  - `hypothesis_gen(self, component_desc: str, sota_exp_desc: str, enable_idea_pool: bool, pipeline: bool = True, exp_feedback_list_desc: str = "", scenario_desc: str = "", problems: dict = {})` — [`L101`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L101)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`task_gen`](proposal.md#DSProposalV2ExpGen.task_gen), [`DSTrace`](base.md#DSTrace), [`get_scenario_all_desc`](../../scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`result`](../../../../core/experiment.md#Experiment.result), [`ExperimentFeedback`](../../../../core/proposal.md#ExperimentFeedback), [`scen`](../../../../core/proposal.md#Trace.scen), [`hist`](base.md#DSTrace.hist), [`knowledge_base`](../../../../core/proposal.md#Trace.knowledge_base), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`sota_experiment_fb`](base.md#DSTrace.sota_experiment_fb), [`wait_retry`](../../../../utils/workflow/misc.md#wait_retry), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`get_leaves`](base.md#DSTrace.get_leaves), [`coder_on_whole_pipeline`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`sota_exp_to_submit`](base.md#DSTrace.sota_exp_to_submit), [`current_selection`](../../../../core/proposal.md#Trace.current_selection), [`DSProposalV2ExpGen`](proposal.md#DSProposalV2ExpGen), [`hypothesis_rank`](proposal.md#DSProposalV2ExpGen.hypothesis_rank), [`enable_knowledge_base`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_knowledge_base), [`max_sota_retrieved_num`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.max_sota_retrieved_num)
- used by: [`async_gen`](router/__init__.md#ParallelMultiTraceExpGen.async_gen), [`gen`](proposal.md#DSProposalV2ExpGen.gen), [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`gen`](merge.md#ExpGen2TraceAndMergeV3.gen), [`DSProposalV2ExpGen`](proposal.md#DSProposalV2ExpGen), [`merge_exp_gen`](router/__init__.md#ParallelMultiTraceExpGen.merge_exp_gen), [`merge_exp_gen`](merge.md#ExpGen2TraceAndMergeV3.merge_exp_gen)

### `ExpGen2TraceAndMerge`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:239`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L239)
- signature: `class ExpGen2TraceAndMerge(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L246`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L246) — documented in [rdagent-log-timer](../../../../../../concepts/rdagent-log-timer.md)
  - `exp_gen` — [`L244`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L244)
  - `merge_exp_gen` — [`L243`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L243)
- protocol/private: `__init__`[`L241`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L241)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`RD_Agent_TIMER_wrapper`](../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`gen`](merge.md#MergeExpGen.gen), [`remain_time`](../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../log/timer.md#RDAgentTimerWrapper.timer), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`scen`](../../../../core/proposal.md#ExpGen.scen), [`DataScienceRDLoop`](../../loop.md#DataScienceRDLoop), [`set_current_selection`](../../../../core/proposal.md#Trace.set_current_selection), [`get_leaves`](base.md#DSTrace.get_leaves), [`RDAgentTimer`](../../../../log/timer.md#RDAgentTimer), [`__init__`](../../../../core/proposal.md#ExpGen.__init__), [`sub_trace_count`](base.md#DSTrace.sub_trace_count), [`default_exp_gen`](../../loop.md#DataScienceRDLoop.default_exp_gen), [`merge_hours`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`coding_fail_reanalyze_threshold`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coding_fail_reanalyze_threshold), [`consecutive_errors`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.consecutive_errors), [`MergeExpGen`](merge.md#MergeExpGen)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen)

### `ExpGen2TraceAndMergeV2`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:354`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L354)
- signature: `class ExpGen2TraceAndMergeV2(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None, selection: tuple[int, ...] = (-1,))` — [`L370`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L370) — documented in [rdagent-log-timer](../../../../../../concepts/rdagent-log-timer.md)
  - `reset_exp_gen_version(self, version: str = "v2")` — [`L361`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L361)
  - `exp_gen` — [`L358`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L358)
  - `flag_start_merge` — [`L359`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L359)
  - `merge_exp_gen` — [`L357`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L357)
- protocol/private: `__init__`[`L355`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L355)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`RD_Agent_TIMER_wrapper`](../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`gen`](merge.md#MergeExpGen_MultiTrace.gen), [`hist`](base.md#DSTrace.hist), [`remain_time`](../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../log/timer.md#RDAgentTimerWrapper.timer), [`NEW_ROOT`](../../../../core/proposal.md#Trace.NEW_ROOT), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`scen`](../../../../core/proposal.md#ExpGen.scen), [`DataScienceRDLoop`](../../loop.md#DataScienceRDLoop), [`set_current_selection`](../../../../core/proposal.md#Trace.set_current_selection), [`get_leaves`](base.md#DSTrace.get_leaves), [`RDAgentTimer`](../../../../log/timer.md#RDAgentTimer), [`__init__`](../../../../core/proposal.md#ExpGen.__init__), [`get_current_selection`](../../../../core/proposal.md#Trace.get_current_selection), [`sub_trace_count`](base.md#DSTrace.sub_trace_count), [`default_exp_gen`](../../loop.md#DataScienceRDLoop.default_exp_gen), [`merge_hours`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`coding_fail_reanalyze_threshold`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coding_fail_reanalyze_threshold), [`consecutive_errors`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.consecutive_errors), [`MergeExpGen_MultiTrace`](merge.md#MergeExpGen_MultiTrace), [`enable_multi_version_exp_gen`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.enable_multi_version_exp_gen), [`exp_gen_version_list`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.exp_gen_version_list)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen)

### `ExpGen2TraceAndMergeV3`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:414`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L414)
- signature: `class ExpGen2TraceAndMergeV3(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L420`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L420) — documented in [rdagent-log-timer](../../../../../../concepts/rdagent-log-timer.md)
  - `exp_gen` — [`L418`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L418)
  - `merge_exp_gen` — [`L417`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L417)
- protocol/private: `__init__`[`L415`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L415)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`gen`](merge.md#ExpGen2Hypothesis.gen), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`RD_Agent_TIMER_wrapper`](../../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`remain_time`](../../../../log/timer.md#RDAgentTimer.remain_time), [`timer`](../../../../log/timer.md#RDAgentTimerWrapper.timer), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`scen`](../../../../core/proposal.md#ExpGen.scen), [`DataScienceRDLoop`](../../loop.md#DataScienceRDLoop), [`set_current_selection`](../../../../core/proposal.md#Trace.set_current_selection), [`get_leaves`](base.md#DSTrace.get_leaves), [`RDAgentTimer`](../../../../log/timer.md#RDAgentTimer), [`sota_exp_to_submit`](base.md#DSTrace.sota_exp_to_submit), [`exp2idx`](../../../../core/proposal.md#Trace.exp2idx), [`__init__`](../../../../core/proposal.md#ExpGen.__init__), [`default_exp_gen`](../../loop.md#DataScienceRDLoop.default_exp_gen), [`merge_hours`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.merge_hours), [`coding_fail_reanalyze_threshold`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coding_fail_reanalyze_threshold), [`consecutive_errors`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.consecutive_errors), [`ExpGen2Hypothesis`](merge.md#ExpGen2Hypothesis), [`is_parent`](../../../../core/proposal.md#Trace.is_parent)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen)

### `MergeExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:26`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L26)
- signature: `class MergeExpGen(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L27) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`hist`](base.md#DSTrace.hist), [`DSHypothesis`](base.md#DSHypothesis), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`sota_experiment_fb`](base.md#DSTrace.sota_experiment_fb), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`PipelineTask`](../../../../components/coder/data_science/pipeline/exp.md#PipelineTask), [`set_current_selection`](../../../../core/proposal.md#Trace.set_current_selection), [`get_leaves`](base.md#DSTrace.get_leaves), [`coder_on_whole_pipeline`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`inject_code_from_file_dict`](../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](merge.md#ExpGen2TraceAndMerge.gen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`merge_exp_gen`](merge.md#ExpGen2TraceAndMerge.merge_exp_gen)

### `MergeExpGen_MultiTrace`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/merge.py:275`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L275)
- signature: `class MergeExpGen_MultiTrace(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L276`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/merge.py#L276)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`hist`](base.md#DSTrace.hist), [`DSHypothesis`](base.md#DSHypothesis), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`sota_experiment_fb`](base.md#DSTrace.sota_experiment_fb), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`PipelineTask`](../../../../components/coder/data_science/pipeline/exp.md#PipelineTask), [`get_leaves`](base.md#DSTrace.get_leaves), [`coder_on_whole_pipeline`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.coder_on_whole_pipeline), [`inject_code_from_file_dict`](../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict)
- used by: [`gen`](merge.md#ExpGen2TraceAndMergeV2.gen), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen), [`merge_exp_gen`](merge.md#ExpGen2TraceAndMergeV2.merge_exp_gen)

