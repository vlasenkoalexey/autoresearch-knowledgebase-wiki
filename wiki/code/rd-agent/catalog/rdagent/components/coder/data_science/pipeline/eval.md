---
title: 'Module: rdagent/components/coder/data_science/pipeline/eval.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/pipeline/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.pipeline.eval`/
symbols:
  PipelineCoSTEEREvaluator.evaluate: PipelineCoSTEEREvaluator#evaluate().
  DSCoderFeedback.merge: DSCoderFeedback#merge().
  DSCoderFeedback.error_message: DSCoderFeedback#error_message.
  DSCoderFeedback: DSCoderFeedback#
  DSCoderFeedback.__str__: DSCoderFeedback#__str__().
  DSCoderFeedback.requires_documentation_search: DSCoderFeedback#requires_documentation_search.
  PipelineSingleFeedback: PipelineSingleFeedback.
  DSCoderFeedback.val_and_update_init_dict: DSCoderFeedback#val_and_update_init_dict().
  PipelineCoSTEEREvaluator: PipelineCoSTEEREvaluator#
  PipelineMultiFeedback: PipelineMultiFeedback.
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/data_science/pipeline/eval.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py)

## Classes
### `DSCoderFeedback`  ·  implements/extends CoSTEERSingleFeedback
- def: [`rdagent/components/coder/data_science/pipeline/eval.py:33`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L33)
- doc: Feedback for Data Science CoSTEER evaluation.
- signature: `class DSCoderFeedback(CoSTEERSingleFeedback):`
- members:
  - `merge(cls, feedback_li: list[CoSTEERSingleFeedback])` — [`L87`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L87) — documented in [rdagent-components-coder-CoSTEER-evaluators](../../../../../../concepts/rdagent-components-coder-CoSTEER-evaluators.md)
  - `val_and_update_init_dict(data: dict)` — [`L43`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L43)
  - `error_message` — [`L40`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L40)
  - `requires_documentation_search` — [`L39`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L39)
- protocol/private: `__str__`[`L71`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L71)
- uses (calls/refs, reference-scoped): [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`val_and_update_init_dict`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`__str__`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.__str__), [`merge`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.merge)
- used by: [`evaluate`](eval.md#PipelineCoSTEEREvaluator.evaluate), [`CoSTEERSingleFeedback`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`val_and_update_init_dict`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.val_and_update_init_dict), [`merge`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.merge), [`PipelineSingleFeedback`](eval.md#PipelineSingleFeedback)

### `PipelineCoSTEEREvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/data_science/pipeline/eval.py:123`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L123)
- signature: `class PipelineCoSTEEREvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, queried_knowledge: CoSTEERQueriedKnowledgeV2 = None, **kwargs)` — [`L125`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L125) — documented in [rdagent-app-data_science-conf](../../../../../../concepts/rdagent-app-data_science-conf.md)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`DS_RD_SETTING`](../../../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../../core/experiment.md#FBWorkspace.file_dict), [`warning`](../../../../log/logger.md#RDAgentLog.warning), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`conf`](../../../../utils/env.md#Env.conf), [`Task`](../../../../core/experiment.md#Task), [`get_ds_env`](../conf.md#get_ds_env), [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`final_decision`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`scen`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`exit_code`](../../../../utils/env.md#EnvResult.exit_code), [`error`](../../../../log/logger.md#RDAgentLog.error), [`stdout`](../../../../utils/env.md#EnvResult.stdout), [`get_scenario_all_desc`](../../../../core/scenario.md#Scenario.get_scenario_all_desc), [`run`](../../../../core/experiment.md#FBWorkspace.run), [`build_cls_from_json_with_retry`](../../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`execute`](../../../../core/experiment.md#FBWorkspace.execute), [`return_checking`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`convert`](../share/notebook.md#NotebookConverter.convert), [`code`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`remove_eda_part`](../utils.md#remove_eda_part), [`CoSTEERQueriedKnowledgeV2`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`task_to_similar_task_successful_knowledge`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV1.task_to_similar_task_successful_knowledge), [`get_clear_ws_cmd`](../conf.md#get_clear_ws_cmd), [`error_message`](eval.md#DSCoderFeedback.error_message), [`sample_data_by_LLM`](../../../../app/data_science/conf.md#DataScienceBasePropSetting.sample_data_by_LLM), [`query`](../../../agent/context7/__init__.md#Agent.query), [`validate_code_format`](../share/notebook.md#NotebookConverter.validate_code_format), [`Agent`](../../../agent/context7/__init__.md#Agent), [`failed_task_info_set`](../../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge.failed_task_info_set), [`requires_documentation_search`](eval.md#DSCoderFeedback.requires_documentation_search), [`PipelineSingleFeedback`](eval.md#PipelineSingleFeedback)  (+5 more; 5 test-only)
- used by: [`CoSTEEREvaluator`](../../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#PipelineCoSTEER.__init__)

## Module values
- `DIRNAME` — [`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L29)
- `PipelineMultiFeedback` — [`L120`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L120)
- `PipelineSingleFeedback` — [`L119`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/pipeline/eval.py#L119)

