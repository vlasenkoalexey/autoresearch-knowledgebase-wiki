---
title: 'Module: rdagent/components/coder/CoSTEER/evolvable_subjects.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/CoSTEER/evolvable_subjects.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.CoSTEER.evolvable_subjects`/EvolvingItem#
symbols:
  EvolvingItem: ''
  EvolvingItem.from_experiment: from_experiment().
  EvolvingItem.__init__: __init__().
  EvolvingItem.sub_gt_implementations: sub_gt_implementations.
---
# Module: [`rdagent/components/coder/CoSTEER/evolvable_subjects.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/evolvable_subjects.py)

## Classes
### `EvolvingItem`  ·  implements/extends EvolvableSubjects, Experiment
- def: [`rdagent/components/coder/CoSTEER/evolvable_subjects.py:6`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/evolvable_subjects.py#L6) — documented in [rdagent-app-CI-run](../../../../../concepts/rdagent-app-CI-run.md)
- doc: Intermediate item of factor implementation.
- signature: `class EvolvingItem(Experiment, EvolvableSubjects):`
- members:
  - `from_experiment(cls, exp: Experiment)` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/evolvable_subjects.py#L28)
  - `sub_gt_implementations` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/evolvable_subjects.py#L20)
- protocol/private: `__init__`[`L11`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/evolvable_subjects.py#L11)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`Experiment`](../../../core/experiment.md#Experiment), [`Task`](../../../core/experiment.md#Task), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`EvolvableSubjects`](../../../core/evolving_framework.md#EvolvableSubjects), [`__init__`](../../../core/experiment.md#Experiment.__init__)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`evolve_agent`](__init__.md#CoSTEER.evolve_agent), [`evolve_iter`](evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`develop`](__init__.md#CoSTEER.develop), [`evaluate_iter`](evaluators.md#CoSTEERMultiEvaluator.evaluate_iter), [`assign_code_list_to_evo`](evolving_strategy.md#MultiProcessEvolvingStrategy.assign_code_list_to_evo), [`EvolvableSubjects`](../../../core/evolving_framework.md#EvolvableSubjects), [`evolve_iter`](../rl/costeer.md#RLEvolvingStrategy.evolve_iter)

