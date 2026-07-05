---
title: 'Module: rdagent/components/coder/rl/costeer.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/rl/costeer.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.rl.costeer`/RL
symbols:
  RLEvolvingStrategy._generate_code: EvolvingStrategy#_generate_code().
  RLCoderEvaluator.evaluate: CoderEvaluator#evaluate().
  RLEvolvingStrategy.evolve_iter: EvolvingStrategy#evolve_iter().
  RLCoSTEER.__init__: CoSTEER#__init__().
  RLEvolvingStrategy.__init__: EvolvingStrategy#__init__().
  RLCoderCoSTEERSettings: CoderCoSTEERSettings#
  RLEvolvingStrategy: EvolvingStrategy#
  RLCoSTEER: CoSTEER#
  RLCoderEvaluator.__init__: CoderEvaluator#__init__().
  RLCoderEvaluator: CoderEvaluator#
  RLEvolvingStrategy.scen: EvolvingStrategy#scen.
  RLEvolvingStrategy.settings: EvolvingStrategy#settings.
  RLEvolvingStrategy._mock_code: EvolvingStrategy#_mock_code().
  RLCoderEvaluator.scen: CoderEvaluator#scen.
---
# Module: [`rdagent/components/coder/rl/costeer.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py)

## Classes
### `RLCoSTEER`  ·  implements/extends CoSTEER
- def: [`rdagent/components/coder/rl/costeer.py:121`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L121)
- doc: RL CoSTEER - orchestrates code generation and evaluation.
- signature: `class RLCoSTEER(CoSTEER):`
- protocol/private: `__init__`[`L124`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L124)
- uses (calls/refs, reference-scoped): [`Scenario`](../../../core/scenario.md#Scenario), [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER), [`CoSTEERMultiEvaluator`](../CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../CoSTEER/__init__.md#CoSTEER.__init__), [`RLCoderCoSTEERSettings`](costeer.md#RLCoderCoSTEERSettings), [`RLEvolvingStrategy`](costeer.md#RLEvolvingStrategy), [`RLCoderEvaluator`](costeer.md#RLCoderEvaluator)
- used by: [`CoSTEER`](../CoSTEER/__init__.md#CoSTEER)

### `RLCoderCoSTEERSettings`  ·  implements/extends CoSTEERSettings
- def: [`rdagent/components/coder/rl/costeer.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L23)
- doc: RL Coder settings.
- signature: `class RLCoderCoSTEERSettings(CoSTEERSettings):`
- uses (calls/refs, reference-scoped): [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings)
- used by: [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`__init__`](costeer.md#RLCoSTEER.__init__)

### `RLCoderEvaluator`
- def: [`rdagent/components/coder/rl/costeer.py:98`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L98)
- doc: RL code evaluator (mock implementation).
- signature: `class RLCoderEvaluator:`
- members:
  - `evaluate(self, target_task: Task, implementation: FBWorkspace, gt_implementation: FBWorkspace | None, queried_knowledge: CoSTEERQueriedKnowledge | None = None)` — [`L104`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L104) — Evaluate RL code. Currently returns mock success.
  - `scen` — [`L102`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L102)
- protocol/private: `__init__`[`L101`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L101)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`Scenario`](../../../core/scenario.md#Scenario), [`CoSTEERSingleFeedback`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../core/experiment.md#Task), [`final_decision`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.final_decision), [`CoSTEERQueriedKnowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`return_checking`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.return_checking), [`code`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.code), [`execution`](../CoSTEER/evaluators.md#CoSTEERSingleFeedback.execution)
- used by: [`__init__`](costeer.md#RLCoSTEER.__init__)

### `RLEvolvingStrategy`  ·  implements/extends EvolvingStrategy
- def: [`rdagent/components/coder/rl/costeer.py:29`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L29)
- doc: RL code generation strategy using LLM.
- signature: `class RLEvolvingStrategy(EvolvingStrategy):`
- members:
  - `_generate_code(self, task: Task, evolving_trace: list[EvoStep] = [])` — [`L54`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L54) — Generate RL training code using LLM.
  - `_mock_code(self)` — [`L85`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L85) — Fallback mock code.
  - `evolve_iter(self, *, evo: EvolvingItem, queried_knowledge: CoSTEERQueriedKnowledge | None = None, evolving_trace: list[EvoStep] = [], **kwargs)` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L36) — Generate code for all tasks using LLM.
  - `scen` — [`L33`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L33)
  - `settings` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L34)
- protocol/private: `__init__`[`L32`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/rl/costeer.py#L32)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Scenario`](../../../core/scenario.md#Scenario), [`Task`](../../../core/experiment.md#Task), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`build_chat_completion`](../../../oai/backend/base.md#ChatSession.build_chat_completion), [`CoSTEERQueriedKnowledge`](../CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`CoSTEERSettings`](../CoSTEER/config.md#CoSTEERSettings), [`name`](../../../core/experiment.md#AbsTask.name), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`EvoStep`](../../../core/evolving_framework.md#EvoStep), [`EvolvingStrategy`](../../../core/evolving_framework.md#EvolvingStrategy), [`EvolvingItem`](../CoSTEER/evolvable_subjects.md#EvolvingItem), [`RL_RD_SETTING`](../../../app/rl/conf.md#RL_RD_SETTING), [`build_chat_session`](../../../oai/backend/base.md#APIBackend.build_chat_session), [`feedback`](../../../core/evolving_framework.md#EvoStep.feedback), [`description`](../../../core/experiment.md#Task.description), [`base_model`](../../../app/rl/conf.md#RLPostTrainingPropSetting.base_model), [`benchmark`](../../../app/rl/conf.md#RLPostTrainingPropSetting.benchmark)
- used by: [`EvolvingStrategy`](../../../core/evolving_framework.md#EvolvingStrategy), [`__init__`](costeer.md#RLCoSTEER.__init__), [`evolve_iter`](../../../core/evolving_framework.md#EvolvingStrategy.evolve_iter)

