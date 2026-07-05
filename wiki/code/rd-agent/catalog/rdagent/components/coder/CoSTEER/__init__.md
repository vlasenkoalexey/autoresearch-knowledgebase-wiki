---
title: 'Module: rdagent/components/coder/CoSTEER/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/CoSTEER/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.CoSTEER`/CoSTEER#
symbols:
  CoSTEER.evolve_agent: evolve_agent.
  CoSTEER: ''
  CoSTEER.develop: develop().
  CoSTEER.__init__: __init__().
  CoSTEER._exp_postprocess_by_feedback: _exp_postprocess_by_feedback().
  CoSTEER.rag: rag.
  CoSTEER._get_last_fb: _get_last_fb().
  CoSTEER.get_develop_max_seconds: get_develop_max_seconds().
  CoSTEER.should_use_new_evo: should_use_new_evo().
  CoSTEER.settings: settings.
  CoSTEER.knowledge_base_path: knowledge_base_path.
  CoSTEER.new_knowledge_base_path: new_knowledge_base_path.
  CoSTEER.max_loop: max_loop.
  CoSTEER.evolving_version: evolving_version.
  CoSTEER.with_knowledge: with_knowledge.
  CoSTEER.knowledge_self_gen: knowledge_self_gen.
  CoSTEER.evolving_strategy: evolving_strategy.
  CoSTEER.evaluator: evaluator.
  CoSTEER.stop_eval_chain_on_fail: stop_eval_chain_on_fail.
---
# Module: [`rdagent/components/coder/CoSTEER/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py)

## Classes
### `CoSTEER`  ·  implements/extends Developer
- def: [`rdagent/components/coder/CoSTEER/__init__.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L20)
- signature: `class CoSTEER(Developer[Experiment]):`
- members:
  - `_exp_postprocess_by_feedback(self, evo: Experiment, feedback: CoSTEERMultiFeedback)` — [`L157`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L157) — Responsibility:
  - `develop(self, exp: Experiment)` — [`L93`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L93)
  - `get_develop_max_seconds(self)` — [`L69`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L69) — Get the maximum seconds for the develop task.
  - `should_use_new_evo(self, base_fb: CoSTEERMultiFeedback | None, new_fb: CoSTEERMultiFeedback)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L82) — Compare new feedback with the fallback feedback.
  - `evaluator` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L48)
  - `evolve_agent` — [`L99`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L99) — documented in [rdagent-core-experiment](../../../../../concepts/rdagent-core-experiment.md)
  - `evolving_strategy` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L47)
  - `evolving_version` — [`L49`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L49)
  - `knowledge_base_path` — [`L38`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L38)
  - `knowledge_self_gen` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L46)
  - `max_loop` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L37)
  - `new_knowledge_base_path` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L41)
  - `rag` — [`L53`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L53)
  - `settings` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L35)
  - `stop_eval_chain_on_fail` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L50)
  - `with_knowledge` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L45)
- protocol/private: `__init__`[`L21`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L21), `_get_last_fb`[`L76`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/__init__.py#L76)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../core/experiment.md#Experiment), [`log_object`](../../../log/logger.md#RDAgentLog.log_object), [`multistep_evolve`](../../../core/evolving_agent.md#RAGEvoAgent.multistep_evolve), [`CoderError`](../../../core/exception.md#CoderError), [`Developer`](../../../core/developer.md#Developer), [`RD_Agent_TIMER_wrapper`](../../../log/timer.md#RD_Agent_TIMER_wrapper.RD_Agent_TIMER_wrapper), [`CoSTEERSettings`](config.md#CoSTEERSettings), [`return_checking`](evaluators.md#CoSTEERSingleFeedback.return_checking), [`sub_workspace_list`](../../../core/experiment.md#Experiment.sub_workspace_list), [`develop`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`CoSTEERMultiFeedback`](evaluators.md#CoSTEERMultiFeedback), [`DSCoSTEER`](../data_science/share/ds_costeer.md#DSCoSTEER), [`timer`](../../../log/timer.md#RDAgentTimerWrapper.timer), [`code`](evaluators.md#CoSTEERSingleFeedback.code), [`develop`](../data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.develop), [`execution`](evaluators.md#CoSTEERSingleFeedback.execution), [`EvolvingStrategy`](../../../core/evolving_framework.md#EvolvingStrategy), [`EvolvingItem`](evolvable_subjects.md#EvolvingItem), [`started`](../../../log/timer.md#RDAgentTimer.started), [`develop`](../factor_coder/__init__.md#FactorCoSTEER.develop), [`feedback`](../../../core/evolving_framework.md#EvoStep.feedback), [`from_experiment`](evolvable_subjects.md#EvolvingItem.from_experiment), [`evolving_trace`](../../../core/evolving_agent.md#RAGEvoAgent.evolving_trace), [`RAGEvaluator`](../../../core/evolving_agent.md#RAGEvaluator), [`is_acceptable`](../../../core/evaluation.md#Feedback.is_acceptable), [`RAGEvoAgent`](../../../core/evolving_agent.md#RAGEvoAgent), [`is_timeout`](../../../log/timer.md#RDAgentTimer.is_timeout), [`ModelCoSTEER`](../model_coder/__init__.md#ModelCoSTEER), [`create_ws_ckp`](../../../core/experiment.md#Experiment.create_ws_ckp), [`recover_ws_ckp`](../../../core/experiment.md#Experiment.recover_ws_ckp), [`develop`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.develop), [`get_develop_max_seconds`](../data_science/share/ds_costeer.md#DSCoSTEER.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.get_develop_max_seconds), [`should_use_new_evo`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.should_use_new_evo), [`is_acceptable`](evaluators.md#CoSTEERMultiFeedback.is_acceptable), [`FactorCoSTEER`](../factor_coder/__init__.md#FactorCoSTEER)  (+13 more)
- used by: [`coding`](../../../scenarios/data_science/loop.md#DataScienceRDLoop.coding), [`Developer`](../../../core/developer.md#Developer), [`develop`](../../../core/developer.md#Developer.develop), [`__init__`](../data_science/pipeline/__init__.md#PipelineCoSTEER.__init__), [`develop`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`DSCoSTEER`](../data_science/share/ds_costeer.md#DSCoSTEER), [`develop_one_competition`](../data_science/model/test.md#develop_one_competition), [`develop_one_competition`](../data_science/workflow/test.md#develop_one_competition), [`__init__`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.__init__), [`extract_models_and_implement`](../../../app/general_model/general_model.md#extract_models_and_implement), [`develop_one_competition`](../data_science/ensemble/test.md#develop_one_competition), [`develop_one_competition`](../data_science/feature/test.md#develop_one_competition), [`__init__`](../finetune/__init__.md#LLMFinetuneCoSTEER.__init__), [`develop`](../data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.develop), [`__init__`](../data_science/ensemble/__init__.md#EnsembleCoSTEER.__init__), [`__init__`](../data_science/feature/__init__.md#FeatureCoSTEER.__init__), [`__init__`](../data_science/model/__init__.md#ModelCoSTEER.__init__), [`__init__`](../data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.__init__), [`__init__`](../data_science/workflow/__init__.md#WorkflowCoSTEER.__init__), [`__init__`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.__init__), [`__init__`](../factor_coder/__init__.md#FactorCoSTEER.__init__), [`__init__`](../model_coder/__init__.md#ModelCoSTEER.__init__), [`__init__`](../rl/costeer.md#RLCoSTEER.__init__), [`develop`](../factor_coder/__init__.md#FactorCoSTEER.develop), [`ModelCoSTEER`](../model_coder/__init__.md#ModelCoSTEER), [`develop`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.develop), [`get_develop_max_seconds`](../data_science/share/ds_costeer.md#DSCoSTEER.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.get_develop_max_seconds), [`get_develop_max_seconds`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner.get_develop_max_seconds), [`FactorCoSTEER`](../factor_coder/__init__.md#FactorCoSTEER), [`DSCoSTEERRunner`](../../../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner), [`LLMFinetuneCoSTEER`](../finetune/__init__.md#LLMFinetuneCoSTEER), [`RLCoSTEER`](../rl/costeer.md#RLCoSTEER), [`LLMFinetuneRunner`](../../../scenarios/finetune/train/runner.md#LLMFinetuneRunner)  (2 test-only)

