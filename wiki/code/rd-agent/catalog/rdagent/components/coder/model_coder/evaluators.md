---
title: 'Module: rdagent/components/coder/model_coder/evaluators.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/evaluators.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.evaluators`/Model
symbols:
  ModelCoSTEEREvaluator.evaluate: CoSTEEREvaluator#evaluate().
  ModelSingleFeedback: SingleFeedback.
  ModelCoSTEEREvaluator: CoSTEEREvaluator#
  ModelMultiFeedback: MultiFeedback.
---
# Module: [`rdagent/components/coder/model_coder/evaluators.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evaluators.py)

## Classes
### `ModelCoSTEEREvaluator`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/model_coder/evaluators.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evaluators.py#L20)
- signature: `class ModelCoSTEEREvaluator(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: Task, implementation: Workspace, gt_implementation: Workspace, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evaluators.py#L21)
- uses (calls/refs, reference-scoped): [`Task`](../../../core/experiment.md#Task), [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`Workspace`](../../../core/experiment.md#Workspace), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`ModelTask`](model.md#ModelTask), [`evaluate`](eva_utils.md#ModelCodeEvaluator.evaluate), [`execute`](model.md#ModelFBWorkspace.execute), [`evaluate`](eva_utils.md#ModelFinalEvaluator.evaluate), [`ModelFBWorkspace`](model.md#ModelFBWorkspace), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`ModelSingleFeedback`](evaluators.md#ModelSingleFeedback), [`ModelCodeEvaluator`](eva_utils.md#ModelCodeEvaluator), [`ModelFinalEvaluator`](eva_utils.md#ModelFinalEvaluator), [`shape_evaluator`](eva_utils.md#shape_evaluator), [`value_evaluator`](eva_utils.md#value_evaluator)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#ModelCoSTEER.__init__)

## Module values
- `ModelMultiFeedback` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evaluators.py#L17)
- `ModelSingleFeedback` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/evaluators.py#L16)

