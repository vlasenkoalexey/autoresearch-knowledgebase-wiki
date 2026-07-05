---
title: 'Module: rdagent/scenarios/data_science/loop.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.loop`/
symbols:
  DataScienceRDLoop.record: DataScienceRDLoop#record().
  DataScienceRDLoop.trace: DataScienceRDLoop#trace.
  DataScienceRDLoop.coding: DataScienceRDLoop#coding().
  DataScienceRDLoop.feedback: DataScienceRDLoop#feedback().
  DataScienceRDLoop.load: DataScienceRDLoop#load().
  DataScienceRDLoop.running: DataScienceRDLoop#running().
  DataScienceRDLoop: DataScienceRDLoop#
  DataScienceRDLoop.direct_exp_gen: DataScienceRDLoop#direct_exp_gen().
  DataScienceRDLoop.docdev: DataScienceRDLoop#docdev.
  DataScienceRDLoop.__init__: DataScienceRDLoop#__init__().
  DataScienceRDLoop.pipeline_coder: DataScienceRDLoop#pipeline_coder.
  DataScienceRDLoop.exp_gen: DataScienceRDLoop#exp_gen.
  backup_folder: backup_folder().
  DataScienceRDLoop.default_exp_gen: DataScienceRDLoop#default_exp_gen.
  DataScienceRDLoop.dump: DataScienceRDLoop#dump().
  DataScienceRDLoop.interactor: DataScienceRDLoop#interactor.
  DataScienceRDLoop.skip_loop_error: DataScienceRDLoop#skip_loop_error.
  DataScienceRDLoop._check_exit_conditions_on_step: DataScienceRDLoop#_check_exit_conditions_on_step().
  DataScienceRDLoop.ckp_selector: DataScienceRDLoop#ckp_selector.
  DataScienceRDLoop.sota_exp_selector: DataScienceRDLoop#sota_exp_selector.
  DataScienceRDLoop.data_loader_coder: DataScienceRDLoop#data_loader_coder.
  DataScienceRDLoop.feature_coder: DataScienceRDLoop#feature_coder.
  DataScienceRDLoop.model_coder: DataScienceRDLoop#model_coder.
  DataScienceRDLoop.ensemble_coder: DataScienceRDLoop#ensemble_coder.
  DataScienceRDLoop.workflow_coder: DataScienceRDLoop#workflow_coder.
  DataScienceRDLoop.withdraw_loop_error: DataScienceRDLoop#withdraw_loop_error.
  clean_workspace: clean_workspace().
  DataScienceRDLoop.skip_loop_error_stepname: DataScienceRDLoop#skip_loop_error_stepname.
---
# Module: [`rdagent/scenarios/data_science/loop.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py)

## Classes
### `DataScienceRDLoop`
- def: [`rdagent/scenarios/data_science/loop.py:87`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L87)
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L154`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L154) — documented in [rdagent-log-logger](../../../../concepts/rdagent-log-logger.md)
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L139`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L139)
  - `dump(self, path: str | Path)` — [`L373`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L373) — Since knowledge_base is big and we don't want to dump it every time
  - `feedback(self, prev_out: dict[str, Any])` — [`L187`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L187) — Assumption:
  - `load(cls, path: str | Path, checkout: bool | str | Path = False, replace_timer: bool = True)` — [`L359`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L359) — documented in [rdagent-app-data_science-conf](../../../../concepts/rdagent-app-data_science-conf.md)
  - `record(self, prev_out: dict[str, Any])` — [`L211`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L211) — documented in [rdagent-app-data_science-conf](../../../../concepts/rdagent-app-data_science-conf.md)
  - `running(self, prev_out: dict[str, Any])` — [`L177`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L177)
  - `ckp_selector` — [`L108`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L108)
  - `data_loader_coder` — [`L115`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L115)
  - `default_exp_gen` — [`L94`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L94)
  - `docdev` — [`L125`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L125)
  - `ensemble_coder` — [`L118`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L118)
  - `exp_gen` — [`L110`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L110)
  - `feature_coder` — [`L116`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L116)
  - `interactor` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L112)
  - `model_coder` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L117)
  - `pipeline_coder` — [`L121`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L121)
  - `skip_loop_error` — [`L89`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L89)
  - `skip_loop_error_stepname` — [`L91`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L91)
  - `sota_exp_selector` — [`L109`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L109)
  - `trace` — [`L131`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L131) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
  - `withdraw_loop_error` — [`L90`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L90)
  - `workflow_coder` — [`L119`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L119)
- protocol/private: `__init__`[`L96`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L96), `_check_exit_conditions_on_step`[`L353`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L353)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../app/data_science/conf.md#DS_RD_SETTING), [`Scenario`](../../core/scenario.md#Scenario), [`DSExperiment`](experiment/experiment.md#DSExperiment), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`DSTrace`](proposal/exp_gen/base.md#DSTrace), [`ExpGen`](../../core/proposal.md#ExpGen), [`import_class`](../../core/utils.md#import_class), [`sub_tasks`](../../core/experiment.md#Experiment.sub_tasks), [`CoderError`](../../core/exception.md#CoderError), [`hypothesis`](../../core/experiment.md#Experiment.hypothesis), [`load`](../../utils/workflow/loop.md#LoopBase.load), [`error`](../../log/logger.md#RDAgentLog.error), [`develop`](../../core/developer.md#Developer.develop), [`ExperimentFeedback`](../../core/proposal.md#ExperimentFeedback), [`scen`](../../core/proposal.md#Trace.scen), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`develop`](../../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`hist`](proposal/exp_gen/base.md#DSTrace.hist), [`develop`](../../components/coder/data_science/share/doc.md#DocDev.develop), [`generate_feedback`](../../core/proposal.md#Experiment2Feedback.generate_feedback), [`knowledge_base`](../../core/proposal.md#Trace.knowledge_base), [`_check_exit_conditions_on_step`](../../utils/workflow/loop.md#LoopBase._check_exit_conditions_on_step), [`async_gen`](../../core/proposal.md#ExpGen.async_gen), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`develop`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.develop), [`sync_dag_parent_and_hist`](proposal/exp_gen/base.md#DSTrace.sync_dag_parent_and_hist), [`timer`](../../utils/workflow/loop.md#LoopBase.timer), [`DataScienceScen`](scen/__init__.md#DataScienceScen), [`competition`](../../app/kaggle/conf.md#KaggleBasePropSetting.competition), [`reanalyze_competition_description`](scen/__init__.md#DataScienceScen.reanalyze_competition_description), [`dump`](../../utils/workflow/loop.md#LoopBase.dump), [`PipelineTask`](../../components/coder/data_science/pipeline/exp.md#PipelineTask), [`WorkflowTask`](../../components/coder/data_science/workflow/exp.md#WorkflowTask), [`add_duration`](../../log/timer.md#RDAgentTimer.add_duration), [`set_current_selection`](../../core/proposal.md#Trace.set_current_selection), [`steps`](../../utils/workflow/loop.md#LoopBase.steps), [`loop_idx`](../../utils/workflow/loop.md#LoopBase.loop_idx)  (+53 more)
- used by: [`load`](../../utils/workflow/loop.md#LoopBase.load), [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`feedback`](../../components/workflow/rd_loop.md#RDLoop.feedback), [`main`](../../app/data_science/loop.md#main), [`_check_exit_conditions_on_step`](../../utils/workflow/loop.md#LoopBase._check_exit_conditions_on_step), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`running`](../../components/workflow/rd_loop.md#RDLoop.running), [`dump`](../../utils/workflow/loop.md#LoopBase.dump), [`record`](../../components/workflow/rd_loop.md#RDLoop.record), [`main`](../../app/finetune/data_science/loop.md#main), [`exp_gen`](proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV2.exp_gen), [`exp_gen`](proposal/exp_gen/merge.md#ExpGen2TraceAndMerge.exp_gen), [`exp_gen`](proposal/exp_gen/merge.md#ExpGen2TraceAndMergeV3.exp_gen), [`exp_gen`](proposal/exp_gen/router/__init__.md#ParallelMultiTraceExpGen.exp_gen), [`load_times_deprecated`](../../log/ui/utils.md#load_times_deprecated), [`first_li_si_after_one_time`](../../log/utils/folder.md#first_li_si_after_one_time)

## Functions
- `backup_folder(path: str | Path)` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L64)
- `clean_workspace(workspace_root: Path)` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/loop.py#L43) — Clean the workspace folder and only keep the essential files to save more space.

