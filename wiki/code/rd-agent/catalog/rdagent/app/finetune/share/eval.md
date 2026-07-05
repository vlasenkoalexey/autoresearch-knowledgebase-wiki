---
title: 'Module: rdagent/app/finetune/share/eval.py'
type: catalog
provenance: extracted
module: rdagent/app/finetune/share/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.finetune.share.eval`/PrevModelLoadEvaluator#
symbols:
  PrevModelLoadEvaluator.evaluate: evaluate().
  PrevModelLoadEvaluator.__init__: __init__().
  PrevModelLoadEvaluator: ''
---
# Module: [`rdagent/app/finetune/share/eval.py`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/share/eval.py)

## Classes
### `PrevModelLoadEvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/app/finetune/share/eval.py:13`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/share/eval.py#L13)
- doc: This evaluator checks whether the code actually loads a model from `prev_model`.
- signature: `class PrevModelLoadEvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace, *args, **kwargs)` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/share/eval.py#L19)
- protocol/private: `__init__`[`L16`](../../../../../../../../raw/code/rd-agent/rdagent/app/finetune/share/eval.py#L16)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`Scenario`](../../../core/scenario.md#Scenario), [`CoSTEERSingleFeedback`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`final_decision`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`build_cls_from_json_with_retry`](../../../utils/agent/workflow.md#build_cls_from_json_with_retry), [`return_checking`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`code`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution), [`all_codes`](../../../core/experiment.md#FBWorkspace.all_codes), [`__init__`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.__init__)
- used by: [`CoSTEEREvaluator`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../../../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate)

