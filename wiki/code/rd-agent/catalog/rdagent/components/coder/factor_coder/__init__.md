---
title: 'Module: rdagent/components/coder/factor_coder/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder`/FactorCoSTEER#
symbols:
  FactorCoSTEER.__init__: __init__().
  FactorCoSTEER.develop: develop().
  FactorCoSTEER: ''
---
# Module: [`rdagent/components/coder/factor_coder/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/__init__.py)

## Classes
### `FactorCoSTEER`  ·  implements/extends CoSTEER
- def: [`rdagent/components/coder/factor_coder/__init__.py:12`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/__init__.py#L12)
- signature: `class FactorCoSTEER(CoSTEER):`
- members:
  - `develop(self, exp: Experiment)` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/__init__.py#L25)
- protocol/private: `__init__`[`L13`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/__init__.py#L13)
- uses (calls/refs, reference-scoped): [`Scenario`](../../../core/scenario.md#Scenario), [`Experiment`](../../../core/experiment.md#Experiment), [`evolve_agent`](../CoSTEER/__init__.md#CoSTEER.evolve_agent), [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER), [`develop`](../CoSTEER/__init__.md#CoSTEER.develop), [`FACTOR_COSTEER_SETTINGS`](config.md#FACTOR_COSTEER_SETTINGS), [`CoSTEERMultiEvaluator`](../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../CoSTEER/__init__.md#CoSTEER.__init__), [`feedback`](../../../core/evolving_framework.md#EvoStep.feedback), [`evolving_trace`](../../../core/evolving_agent.md#RAGEvoAgent.evolving_trace), [`prop_dev_feedback`](../../../core/experiment.md#Experiment.prop_dev_feedback), [`FactorEvaluatorForCoder`](evaluators.md#FactorEvaluatorForCoder), [`FactorMultiProcessEvolvingStrategy`](evolving_strategy.md#FactorMultiProcessEvolvingStrategy)
- used by: [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER), [`develop`](../CoSTEER/__init__.md#CoSTEER.develop), [`KGFactorCoSTEER`](../../../scenarios/kaggle/developer/coder.md#KGFactorCoSTEER), [`QlibFactorCoSTEER`](../../../scenarios/qlib/developer/factor_coder.md#QlibFactorCoSTEER)

