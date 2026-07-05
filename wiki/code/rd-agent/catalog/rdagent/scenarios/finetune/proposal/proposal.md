---
title: 'Module: rdagent/scenarios/finetune/proposal/proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/proposal/proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.proposal.proposal`/
symbols:
  LLMFinetuneExpGen._gen_hypothesis: LLMFinetuneExpGen#_gen_hypothesis().
  LLMFinetuneExpGen.gen: LLMFinetuneExpGen#gen().
  FTHypothesis.__str__: FTHypothesis#__str__().
  LLMFinetuneExpGen.__init__: LLMFinetuneExpGen#__init__().
  FTHypothesis: FTHypothesis#
  FTHypothesis.__init__: FTHypothesis#__init__().
  LLMFinetuneExpGen: LLMFinetuneExpGen#
  FTHypothesis.base_model: FTHypothesis#base_model.
---
# Module: [`rdagent/scenarios/finetune/proposal/proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py)

## Classes
### `FTHypothesis`  ·  implements/extends Hypothesis
- def: [`rdagent/scenarios/finetune/proposal/proposal.py:24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L24)
- doc: LLM fine-tuning hypothesis class.
- signature: `class FTHypothesis(Hypothesis):`
- members:
  - `base_model` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L41)
- protocol/private: `__init__`[`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L27), `__str__`[`L43`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L43)
- uses (calls/refs, reference-scoped): [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`reason`](../../../core/proposal.md#Hypothesis.reason), [`__init__`](../../../core/proposal.md#Hypothesis.__init__)
- used by: [`_gen_hypothesis`](proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`Hypothesis`](../../../core/proposal.md#Hypothesis)

### `LLMFinetuneExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/finetune/proposal/proposal.py:56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L56)
- doc: LLM fine-tuning experiment generator.
- signature: `class LLMFinetuneExpGen(ExpGen):`
- members:
  - `_gen_hypothesis(self, trace: Trace, base_model: str, parent_exp: FTExperiment | None = None)` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L74) — Generate hypothesis covering both data processing and training configuration. — documented in [rdagent-app-finetune-llm-conf](../../../../../concepts/rdagent-app-finetune-llm-conf.md)
  - `gen(self, trace: Trace)` — [`L65`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L65) — Generate LLM fine-tuning experiment. — documented in [rdagent-core-proposal](../../../../../concepts/rdagent-core-proposal.md)
- protocol/private: `__init__`[`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/proposal/proposal.py#L62)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`Trace`](../../../core/proposal.md#Trace), [`ExpGen`](../../../core/proposal.md#ExpGen), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`build_chat_completion`](../../../oai/backend/base.md#ChatSession.build_chat_completion), [`NEW_ROOT`](../../../core/proposal.md#Trace.NEW_ROOT), [`scen`](../../../core/proposal.md#ExpGen.scen), [`FTExperiment`](../experiment/experiment.md#FTExperiment), [`ensure_ft_assets_exist`](../utils.md#ensure_ft_assets_exist), [`get_sota_experiment`](../../../core/proposal.md#Trace.get_sota_experiment), [`build_chat_session`](../../../oai/backend/base.md#APIBackend.build_chat_session), [`LLaMAFactory_manager`](../scen/llama_factory_manager.md#LLaMAFactory_manager), [`exp2idx`](../../../core/proposal.md#Trace.exp2idx), [`get_children`](../../../core/proposal.md#Trace.get_children), [`local_selection`](../../../core/experiment.md#Experiment.local_selection), [`__init__`](../../../core/proposal.md#ExpGen.__init__), [`base_model`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.base_model), [`FTTask`](../../../components/coder/finetune/exp.md#FTTask), [`format_method_specific_params`](../scen/llama_factory_manager.md#LLaMAFactoryManager.format_method_specific_params), [`format_shared_params`](../scen/llama_factory_manager.md#LLaMAFactoryManager.format_shared_params), [`inject_from_workspace`](../../../core/experiment.md#FBWorkspace.inject_from_workspace), [`LLMFinetuneScen`](../scen/scenario.md#LLMFinetuneScen), [`force_think_token`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.force_think_token), [`methods`](../scen/llama_factory_manager.md#LLaMAFactoryManager.methods), [`FTHypothesis`](proposal.md#FTHypothesis), [`target_benchmark`](../../../app/finetune/llm/conf.md#LLMFinetunePropSetting.target_benchmark), [`models`](../scen/llama_factory_manager.md#LLaMAFactoryManager.models)
- used by: [`ExpGen`](../../../core/proposal.md#ExpGen), [`gen`](../../../core/proposal.md#ExpGen.gen)

