---
title: 'Module: rdagent/components/coder/data_science/raw_data_loader/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/raw_data_loader/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.raw_data_loader.eval`/D
symbols:
  DataLoaderCoSTEEREvaluator.evaluate: ataLoaderCoSTEEREvaluator#evaluate().
  DataLoaderEvalFeedback: ataLoaderEvalFeedback.
  DataLoaderCoSTEEREvaluator: ataLoaderCoSTEEREvaluator#
  DIRNAME: IRNAME.
---
# Module: [`rdagent/components/coder/data_science/raw_data_loader/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/eval.py)

## Classes
### `DataLoaderCoSTEEREvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/data_science/raw_data_loader/eval.py:26`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/eval.py#L26)
- signature: `class DataLoaderCoSTEEREvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: CoSTEERQueriedKnowledgeV2 = None, **kwargs)` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/eval.py#L27) — documented in [rdagent-utils-env](../../../../../../concepts/rdagent-utils-env.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../conf.md#get_ds_env), [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`scen`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../../utils/env.md#EnvResult.stdout), [`run`](../../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`all_codes`](../../../../core/experiment.md#FBWorkspace.all_codes), [`remove_eda_part`](../utils.md#remove_eda_part), [`CoSTEERQueriedKnowledgeV2`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`val_and_update_init_dict`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`failed_task_info_set`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge.failed_task_info_set), [`DataLoaderEvalFeedback`](eval.md#DataLoaderEvalFeedback), [`success_task_to_knowledge_dict`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge.success_task_to_knowledge_dict), [`DIRNAME`](eval.md#DIRNAME)
- used by: [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#DataLoaderCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L21`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/eval.py#L21)
- `DataLoaderEvalFeedback` — [`L23`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/raw_data_loader/eval.py#L23)

