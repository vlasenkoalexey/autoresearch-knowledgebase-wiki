---
title: 'Module: rdagent/components/coder/data_science/ensemble/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/ensemble/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.ensemble.eval`/
symbols:
  EnsembleCoSTEEREvaluator.evaluate: EnsembleCoSTEEREvaluator#evaluate().
  EnsembleEvalFeedback: EnsembleEvalFeedback.
  EnsembleCoSTEEREvaluator: EnsembleCoSTEEREvaluator#
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/data_science/ensemble/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/ensemble/eval.py)

## Classes
### `EnsembleCoSTEEREvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/data_science/ensemble/eval.py:24`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/ensemble/eval.py#L24)
- signature: `class EnsembleCoSTEEREvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/ensemble/eval.py#L25) — documented in [rdagent-utils-env](../../../../../../concepts/rdagent-utils-env.md)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../conf.md#get_ds_env), [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`scen`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../../utils/env.md#EnvResult.stdout), [`run`](../../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../../core/evolving_framework.md#QueriedKnowledge), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`all_codes`](../../../../core/experiment.md#FBWorkspace.all_codes), [`remove_eda_part`](../utils.md#remove_eda_part), [`val_and_update_init_dict`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`EnsembleEvalFeedback`](eval.md#EnsembleEvalFeedback), [`DIRNAME`](eval.md#DIRNAME)
- used by: [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#EnsembleCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L19`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/ensemble/eval.py#L19)
- `EnsembleEvalFeedback` — [`L21`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/ensemble/eval.py#L21)

