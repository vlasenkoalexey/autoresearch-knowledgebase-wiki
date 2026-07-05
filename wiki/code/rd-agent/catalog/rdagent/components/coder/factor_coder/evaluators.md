---
title: 'Module: rdagent/components/coder/factor_coder/evaluators.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/evaluators.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder.evaluators`/
symbols:
  FactorEvaluatorForCoder.evaluate: FactorEvaluatorForCoder#evaluate().
  FactorSingleFeedback: FactorSingleFeedback.
  FactorEvaluatorForCoder.code_evaluator: FactorEvaluatorForCoder#code_evaluator.
  FactorEvaluatorForCoder.value_evaluator: FactorEvaluatorForCoder#value_evaluator.
  FactorEvaluatorForCoder.final_decision_evaluator: FactorEvaluatorForCoder#final_decision_evaluator.
  FactorEvaluatorForCoder: FactorEvaluatorForCoder#
  FactorEvaluatorForCoder.__init__: FactorEvaluatorForCoder#__init__().
  shorten_prompt: shorten_prompt().
---
# Module: [`rdagent/components/coder/factor_coder/evaluators.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py)

## Classes
### `FactorEvaluatorForCoder`  ·  implements/extends CoSTEEREvaluator
- def: [`rdagent/components/coder/factor_coder/evaluators.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L20)
- doc: This class is the v1 version of evaluator for a single factor implementation.
- signature: `class FactorEvaluatorForCoder(CoSTEEREvaluator):`
- members:
  - `evaluate(self, target_task: FactorTask, implementation: Workspace, gt_implementation: Workspace = None, queried_knowledge: QueriedKnowledge = None, **kwargs)` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L31) — documented in [rdagent-components-coder-CoSTEER-evaluators](../../../../../concepts/rdagent-components-coder-CoSTEER-evaluators.md)
  - `code_evaluator` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L28) — documented in [rdagent-components-coder-CoSTEER-evaluators](../../../../../concepts/rdagent-components-coder-CoSTEER-evaluators.md)
  - `final_decision_evaluator` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L29)
  - `value_evaluator` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L27)
- protocol/private: `__init__`[`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L25)
- uses (calls/refs, reference-scoped): [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`final_decision`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`Workspace`](../../../core/experiment.md#Workspace), [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`scen`](../CoSTEER/evaluators.md#CoSTEEREvaluator.scen), [`FactorTask`](factor.md#FactorTask), [`evaluate`](eva_utils.md#FactorCodeEvaluator.evaluate), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`evaluate`](eva_utils.md#FactorFinalDecisionEvaluator.evaluate), [`get_task_information`](factor.md#FactorTask.get_task_information), [`value_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.value_feedback), [`FactorSingleFeedback`](evaluators.md#FactorSingleFeedback), [`code_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.code_feedback), [`execution_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.execution_feedback), [`final_feedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.final_feedback), [`__init__`](../CoSTEER/evaluators.md#CoSTEEREvaluator.__init__), [`execute`](../../../core/experiment.md#Workspace.execute), [`FactorCodeEvaluator`](eva_utils.md#FactorCodeEvaluator), [`FactorFinalDecisionEvaluator`](eva_utils.md#FactorFinalDecisionEvaluator), [`FactorValueEvaluator`](eva_utils.md#FactorValueEvaluator), [`final_decision_based_on_gt`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.final_decision_based_on_gt), [`value_generated_flag`](../CoSTEER/evaluators.md#CoSTEERSingleFeedbackDeprecated.value_generated_flag), [`version`](../../../core/experiment.md#AbsTask.version)
- used by: [`CoSTEEREvaluator`](../CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`__init__`](__init__.md#FactorCoSTEER.__init__)

## Functions
- `shorten_prompt(tpl: str, render_kwargs: dict, shorten_key: str, max_trail: int = 10)` — [`L124`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L124) — When the prompt is too long. We have to shorten it.

## Module values
- `FactorSingleFeedback` — [`L17`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/evaluators.py#L17)

