---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/naive.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/naive.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.naive`/NaiveExpGen#
symbols:
  NaiveExpGen.gen: gen().
  NaiveExpGen: ''
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/naive.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/naive.py)

## Classes
### `NaiveExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/naive.py:14`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/naive.py#L14)
- signature: `class NaiveExpGen(ExpGen):`
- members:
  - `gen(self, trace: DSTrace, plan: DSExperimentPlan | None = None)` — [`L15`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/naive.py#L15) — documented in [rdagent-scenarios-data_science-proposal-exp_gen-base](../../../../../../concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`DSExperiment`](../../experiment/experiment.md#DSExperiment), [`DSTrace`](base.md#DSTrace), [`ExpGen`](../../../../core/proposal.md#ExpGen), [`get_scenario_all_desc`](../../scen/__init__.md#DataScienceScen.get_scenario_all_desc), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`scen`](../../../../core/proposal.md#Trace.scen), [`DSHypothesis`](base.md#DSHypothesis), [`experiment_and_feedback_list_after_init`](base.md#DSTrace.experiment_and_feedback_list_after_init), [`DSExperimentPlan`](planner/__init__.md#DSExperimentPlan), [`PipelineTask`](../../../../components/coder/data_science/pipeline/exp.md#PipelineTask), [`inject_code_from_file_dict`](../../../../core/experiment.md#FBWorkspace.inject_code_from_file_dict), [`sota_experiment`](base.md#DSTrace.sota_experiment), [`description`](../../../../core/experiment.md#Task.description)
- used by: [`ExpGen`](../../../../core/proposal.md#ExpGen), [`gen`](../../../../core/proposal.md#ExpGen.gen)

