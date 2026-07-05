---
title: 'Module: rdagent/components/coder/data_science/workflow/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/workflow/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.workflow.eval`/
symbols:
  WorkflowGeneralCaseSpecEvaluator.evaluate: WorkflowGeneralCaseSpecEvaluator#evaluate().
  WorkflowSingleFeedback: WorkflowSingleFeedback.
  WorkflowGeneralCaseSpecEvaluator: WorkflowGeneralCaseSpecEvaluator#
  WorkflowMultiFeedback: WorkflowMultiFeedback.
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/data_science/workflow/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py)

## Classes
### `WorkflowGeneralCaseSpecEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/data_science/workflow/eval.py:27`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py#L27)
- doc: Motivation case:
- signature: `class WorkflowGeneralCaseSpecEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L36`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py#L36) — documented in [rdagent-components-coder-CoSTEER-evaluators](../../../../../../concepts/rdagent-components-coder-CoSTEER-evaluators.md)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../conf.md#get_ds_env), [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`scen`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../../utils/env.md#EnvResult.exit_code), [`stdout`](../../../../utils/env.md#EnvResult.stdout), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`run`](../../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`QueriedKnowledge`](../../../../core/evolving_framework.md#QueriedKnowledge), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`remove_eda_part`](../utils.md#remove_eda_part), [`get_clear_ws_cmd`](../conf.md#get_clear_ws_cmd), [`val_and_update_init_dict`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`spec_enabled`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.spec_enabled), [`WorkflowSingleFeedback`](eval.md#WorkflowSingleFeedback)
- used by: [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#WorkflowCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L21`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py#L21)
- `WorkflowMultiFeedback` — [`L24`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py#L24)
- `WorkflowSingleFeedback` — [`L23`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/workflow/eval.py#L23)

