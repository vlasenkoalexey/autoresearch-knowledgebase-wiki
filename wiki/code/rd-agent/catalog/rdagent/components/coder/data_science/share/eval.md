---
title: 'Module: rdagent/components/coder/data_science/share/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/share/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.share.eval`/
symbols:
  ModelDumpEvaluator.evaluate: ModelDumpEvaluator#evaluate().
  ModelDumpEvaluator: ModelDumpEvaluator#
  ModelDumpEvaluator.__init__: ModelDumpEvaluator#__init__().
  PipelineSingleFeedback: PipelineSingleFeedback.
  PipelineMultiFeedback: PipelineMultiFeedback.
  NO_SUB: NO_SUB.
  NO_SCORE: NO_SCORE.
  ModelDumpEvaluator.data_type: ModelDumpEvaluator#data_type.
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/data_science/share/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py)

## Classes
### `ModelDumpEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/data_science/share/eval.py:29`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L29)
- doc: This evaluator assumes that it runs after the model
- signature: `class ModelDumpEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, *kargs, **kwargs)` — [`L36`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L36)
  - `data_type` — [`L34`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L34)
- protocol/private: `__init__`[`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L32)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`Scenario`](../../../../core/scenario.md#Scenario), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../conf.md#get_ds_env), [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`scen`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`local_data_path`](../../../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`generate_tree`](../../../../scenarios/data_science/scen/utils.md#FileTreeGenerator.generate_tree), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`all_codes`](../../../../core/experiment.md#FBWorkspace.all_codes), [`remove_eda_part`](../utils.md#remove_eda_part), [`get_clear_ws_cmd`](../conf.md#get_clear_ws_cmd), [`FileTreeGenerator`](../../../../scenarios/data_science/scen/utils.md#FileTreeGenerator), [`__init__`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.__init__), [`NO_SCORE`](eval.md#NO_SCORE), [`NO_SUB`](eval.md#NO_SUB), [`model_dump_check_level`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.model_dump_check_level)
- used by: [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](../pipeline/__init__.md#PipelineCoSTEER.__init__), [`__init__`](../../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.__init__)

## Module values
- `DIRNAME` — [`L20`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L20)
- `NO_SCORE` — [`L26`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L26)
- `NO_SUB` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L25)
- `PipelineMultiFeedback` — [`L23`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L23)
- `PipelineSingleFeedback` — [`L22`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/eval.py#L22)

