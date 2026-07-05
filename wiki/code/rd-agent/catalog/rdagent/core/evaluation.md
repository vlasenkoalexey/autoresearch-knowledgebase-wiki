---
title: 'Module: rdagent/core/evaluation.py'
type: catalog
provenance: extracted
module: rdagent/core/evaluation.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.evaluation`/
symbols:
  Feedback: Feedback#
  Evaluator: Evaluator#
  Evaluator.evaluate: Evaluator#evaluate().
  Feedback.is_acceptable: Feedback#is_acceptable().
  EvaluableObj: EvaluableObj#
  Feedback.finished: Feedback#finished().
  Feedback.__bool__: Feedback#__bool__().
---
# Module: [`rdagent/core/evaluation.py`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py)

## Classes
### `EvaluableObj`
- def: [`rdagent/core/evaluation.py:33`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L33)
- doc: A set of information that is evaluable. Following things can be included.
- signature: `class EvaluableObj:`
- uses (calls/refs, reference-scoped): [`EvolvableSubjects`](evolving_framework.md#EvolvableSubjects)
- used by: [`EvolvableSubjects`](evolving_framework.md#EvolvableSubjects), [`evaluate`](evaluation.md#Evaluator.evaluate), [`_get_overall_feedback`](evolving_agent.md#RAGEvoAgent._get_overall_feedback), [`evaluate_iter`](evolving_agent.md#RAGEvaluator.evaluate_iter), [`evaluate_iter`](evolving_framework.md#IterEvaluator.evaluate_iter), [`evaluate`](evolving_framework.md#IterEvaluator.evaluate)

### `Evaluator`  ·  implements/extends ABC
- def: [`rdagent/core/evaluation.py:42`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L42)
- doc: Design Principle:
- signature: `class Evaluator(ABC):`
- members:
  - `evaluate(self, eo: EvaluableObj)` — [`L53`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L53) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- uses (calls/refs, reference-scoped): [`CoSTEEREvaluator`](../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`evaluate`](../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator.evaluate), [`evaluate`](../app/CI/run.md#MypyEvaluator.evaluate), [`evaluate`](../app/CI/run.md#RuffEvaluator.evaluate), [`Feedback`](evaluation.md#Feedback), [`evaluate`](../app/CI/run.md#MultiEvaluator.evaluate), [`EvaluableObj`](evaluation.md#EvaluableObj), [`evaluate`](evolving_framework.md#IterEvaluator.evaluate), [`IterEvaluator`](evolving_framework.md#IterEvaluator), [`RuffEvaluator`](../app/CI/run.md#RuffEvaluator), [`MultiEvaluator`](../app/CI/run.md#MultiEvaluator), [`MypyEvaluator`](../app/CI/run.md#MypyEvaluator)
- used by: [`CoSTEEREvaluator`](../components/coder/CoSTEER/evaluators.md#CoSTEEREvaluator), [`multistep_evolve`](../app/CI/run.md#CIEvoAgent.multistep_evolve), [`evaluate`](../app/CI/run.md#MultiEvaluator.evaluate), [`IterEvaluator`](evolving_framework.md#IterEvaluator), [`ASpecificEvaluator`](evolving_agent.md#ASpecificEvaluator), [`RuffEvaluator`](../app/CI/run.md#RuffEvaluator), [`MultiEvaluator`](../app/CI/run.md#MultiEvaluator), [`MypyEvaluator`](../app/CI/run.md#MypyEvaluator), [`__init__`](../app/CI/run.md#MultiEvaluator.__init__)

### `Feedback`
- def: [`rdagent/core/evaluation.py:8`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L8) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- doc: Design Principle:
- signature: `class Feedback:`
- members:
  - `finished(self)` — [`L22`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L22) — In some implementations, tasks may fail multiple times, leading agents to skip the implementation.
  - `is_acceptable(self)` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L15) — Sometimes, the solution is already acceptable, but we still want to refine it.
- protocol/private: `__bool__`[`L29`](../../../../../../raw/code/rd-agent/rdagent/core/evaluation.py#L29)
- uses (calls/refs, reference-scoped): [`CoSTEERSingleFeedback`](../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`CoSTEERMultiFeedback`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback), [`CIFeedback`](../app/CI/run.md#CIFeedback), [`is_acceptable`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback.is_acceptable), [`finished`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback.finished), [`is_acceptable`](../scenarios/data_science/dev/runner/eval.md#DSRunnerFeedback.is_acceptable)
- used by: [`CoSTEERSingleFeedback`](../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`ExperimentFeedback`](proposal.md#ExperimentFeedback), [`CoSTEERMultiFeedback`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback), [`_exp_postprocess_by_feedback`](../components/coder/CoSTEER/__init__.md#CoSTEER._exp_postprocess_by_feedback), [`evaluate`](evaluation.md#Evaluator.evaluate), [`_get_overall_feedback`](evolving_agent.md#RAGEvoAgent._get_overall_feedback), [`feedback`](evolving_framework.md#EvoStep.feedback), [`evaluate_iter`](evolving_agent.md#RAGEvaluator.evaluate_iter), [`CIFeedback`](../app/CI/run.md#CIFeedback), [`evaluate_iter`](evolving_framework.md#IterEvaluator.evaluate_iter), [`__init__`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledge.__init__), [`evaluate`](evolving_framework.md#IterEvaluator.evaluate), [`is_acceptable`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiFeedback.is_acceptable), [`prop_dev_feedback`](experiment.md#Experiment.prop_dev_feedback), [`is_acceptable`](../scenarios/data_science/dev/runner/eval.md#DSRunnerFeedback.is_acceptable), [`ASpecificFeedback`](experiment.md#ASpecificFeedback)

