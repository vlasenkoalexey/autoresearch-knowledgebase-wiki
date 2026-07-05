---
title: 'Module: rdagent/components/proposal/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/proposal/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.proposal`/
symbols:
  LLMHypothesisGen.gen: LLMHypothesisGen#gen().
  LLMHypothesis2Experiment.convert: LLMHypothesis2Experiment#convert().
  LLMHypothesis2Experiment.convert_response: LLMHypothesis2Experiment#convert_response().
  LLMHypothesis2Experiment: LLMHypothesis2Experiment#
  LLMHypothesisGen.prepare_context: LLMHypothesisGen#prepare_context().
  LLMHypothesisGen.convert_response: LLMHypothesisGen#convert_response().
  LLMHypothesis2Experiment.prepare_context: LLMHypothesis2Experiment#prepare_context().
  LLMHypothesisGen: LLMHypothesisGen#
  FactorAndModelHypothesisGen: FactorAndModelHypothesisGen#
  LLMHypothesisGen.__init__: LLMHypothesisGen#__init__().
  FactorHypothesisGen: FactorHypothesisGen#
  ModelHypothesisGen: ModelHypothesisGen#
  FactorAndModelHypothesisGen.__init__: FactorAndModelHypothesisGen#__init__().
  FactorHypothesis2Experiment: FactorHypothesis2Experiment#
  ModelHypothesis2Experiment: ModelHypothesis2Experiment#
  FactorAndModelHypothesis2Experiment: FactorAndModelHypothesis2Experiment#
  FactorHypothesisGen.__init__: FactorHypothesisGen#__init__().
  ModelHypothesisGen.__init__: ModelHypothesisGen#__init__().
  FactorHypothesisGen.targets: FactorHypothesisGen#targets.
  ModelHypothesisGen.targets: ModelHypothesisGen#targets.
  FactorAndModelHypothesisGen.targets: FactorAndModelHypothesisGen#targets.
  FactorHypothesis2Experiment.__init__: FactorHypothesis2Experiment#__init__().
  FactorHypothesis2Experiment.targets: FactorHypothesis2Experiment#targets.
  ModelHypothesis2Experiment.__init__: ModelHypothesis2Experiment#__init__().
  ModelHypothesis2Experiment.targets: ModelHypothesis2Experiment#targets.
  FactorAndModelHypothesis2Experiment.__init__: FactorAndModelHypothesis2Experiment#__init__().
  FactorAndModelHypothesis2Experiment.targets: FactorAndModelHypothesis2Experiment#targets.
---
# Module: [`rdagent/components/proposal/__init__.py`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py)

## Classes
### `FactorAndModelHypothesis2Experiment`  ·  implements/extends LLMHypothesis2Experiment
- def: [`rdagent/components/proposal/__init__.py:136`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L136)
- signature: `class FactorAndModelHypothesis2Experiment(LLMHypothesis2Experiment):`
- members:
  - `targets` — [`L139`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L139)
- protocol/private: `__init__`[`L137`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L137)
- uses (calls/refs, reference-scoped): [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`KGHypothesis2Experiment`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment)
- used by: [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`KGHypothesis2Experiment`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment)

### `FactorAndModelHypothesisGen`  ·  implements/extends LLMHypothesisGen
- def: [`rdagent/components/proposal/__init__.py:80`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L80)
- signature: `class FactorAndModelHypothesisGen(LLMHypothesisGen):`
- members:
  - `targets` — [`L83`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L83)
- protocol/private: `__init__`[`L81`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L81)
- uses (calls/refs, reference-scoped): [`Scenario`](../../core/scenario.md#Scenario), [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](__init__.md#LLMHypothesisGen.__init__), [`KGHypothesisGen`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen), [`QlibQuantHypothesisGen`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen)
- used by: [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.__init__), [`__init__`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.__init__), [`KGHypothesisGen`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen), [`QlibQuantHypothesisGen`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen)

### `FactorHypothesis2Experiment`  ·  implements/extends LLMHypothesis2Experiment
- def: [`rdagent/components/proposal/__init__.py:124`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L124)
- signature: `class FactorHypothesis2Experiment(LLMHypothesis2Experiment):`
- members:
  - `targets` — [`L127`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L127)
- protocol/private: `__init__`[`L125`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L125)
- uses (calls/refs, reference-scoped): [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`QlibFactorHypothesis2Experiment`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment)
- used by: [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`QlibFactorHypothesis2Experiment`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment)

### `FactorHypothesisGen`  ·  implements/extends LLMHypothesisGen
- def: [`rdagent/components/proposal/__init__.py:68`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L68)
- signature: `class FactorHypothesisGen(LLMHypothesisGen):`
- members:
  - `targets` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L71)
- protocol/private: `__init__`[`L69`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L69)
- uses (calls/refs, reference-scoped): [`Scenario`](../../core/scenario.md#Scenario), [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](__init__.md#LLMHypothesisGen.__init__), [`QlibFactorHypothesisGen`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesisGen)
- used by: [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesisGen.__init__), [`QlibFactorHypothesisGen`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesisGen)

### `LLMHypothesis2Experiment`  ·  implements/extends Hypothesis2Experiment
- def: [`rdagent/components/proposal/__init__.py:86`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L86)
- signature: `class LLMHypothesis2Experiment(Hypothesis2Experiment[Experiment]):`
- members:
  - `convert(self, hypothesis: Hypothesis, trace: Trace)` — [`L94`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L94) — documented in [rdagent-core-proposal](../../../../concepts/rdagent-core-proposal.md)
  - `convert_response(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L91`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L91)
  - `prepare_context(self, hypothesis: Hypothesis, trace: Trace)` — [`L88`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L88)
- uses (calls/refs, reference-scoped): [`T`](../../utils/agent/tpl.md#T), [`r`](../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../oai/llm_utils.md#APIBackend), [`Experiment`](../../core/experiment.md#Experiment), [`Trace`](../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Hypothesis`](../../core/proposal.md#Hypothesis), [`scen`](../../core/proposal.md#Trace.scen), [`prepare_context`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.prepare_context), [`wait_retry`](../../utils/workflow/misc.md#wait_retry), [`convert_response`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.convert_response), [`convert_response`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`prepare_context`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.prepare_context), [`prepare_context`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesis2Experiment.prepare_context), [`convert_response`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment.convert_response), [`Hypothesis2Experiment`](../../core/proposal.md#Hypothesis2Experiment), [`FactorAndModelHypothesis2Experiment`](__init__.md#FactorAndModelHypothesis2Experiment), [`FactorHypothesis2Experiment`](__init__.md#FactorHypothesis2Experiment), [`ModelHypothesis2Experiment`](__init__.md#ModelHypothesis2Experiment)
- used by: [`Hypothesis2Experiment`](../../core/proposal.md#Hypothesis2Experiment), [`convert`](../../core/proposal.md#Hypothesis2Experiment.convert), [`FactorAndModelHypothesis2Experiment`](__init__.md#FactorAndModelHypothesis2Experiment), [`FactorHypothesis2Experiment`](__init__.md#FactorHypothesis2Experiment), [`ModelHypothesis2Experiment`](__init__.md#ModelHypothesis2Experiment)

### `LLMHypothesisGen`  ·  implements/extends HypothesisGen
- def: [`rdagent/components/proposal/__init__.py:18`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L18)
- signature: `class LLMHypothesisGen(HypothesisGen):`
- members:
  - `convert_response(self, response: str)` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L27)
  - `gen(self, trace: Trace, plan: ExperimentPlan | None = None)` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L29) — documented in [rdagent-core-proposal](../../../../concepts/rdagent-core-proposal.md)
  - `prepare_context(self, trace: Trace)` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L24)
- protocol/private: `__init__`[`L19`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L19)
- uses (calls/refs, reference-scoped): [`T`](../../utils/agent/tpl.md#T), [`r`](../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../oai/llm_utils.md#APIBackend), [`Scenario`](../../core/scenario.md#Scenario), [`Trace`](../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Hypothesis`](../../core/proposal.md#Hypothesis), [`get_scenario_all_desc`](../../core/scenario.md#Scenario.get_scenario_all_desc), [`prepare_context`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.prepare_context), [`prepare_context`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.prepare_context), [`scen`](../../core/proposal.md#HypothesisGen.scen), [`ExperimentPlan`](../../core/experiment.md#ExperimentPlan), [`prepare_context`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen.prepare_context), [`FactorAndModelHypothesisGen`](__init__.md#FactorAndModelHypothesisGen), [`HypothesisGen`](../../core/proposal.md#HypothesisGen), [`prepare_context`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesisGen.prepare_context), [`FactorHypothesisGen`](__init__.md#FactorHypothesisGen), [`ModelHypothesisGen`](__init__.md#ModelHypothesisGen), [`convert_response`](../../scenarios/kaggle/proposal/proposal.md#KGHypothesisGen.convert_response), [`convert_response`](../../scenarios/qlib/proposal/factor_proposal.md#QlibFactorHypothesisGen.convert_response), [`convert_response`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen.convert_response), [`convert_response`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.convert_response), [`__init__`](../../core/proposal.md#HypothesisGen.__init__)
- used by: [`FactorAndModelHypothesisGen`](__init__.md#FactorAndModelHypothesisGen), [`gen`](../../core/proposal.md#HypothesisGen.gen), [`HypothesisGen`](../../core/proposal.md#HypothesisGen), [`FactorHypothesisGen`](__init__.md#FactorHypothesisGen), [`ModelHypothesisGen`](__init__.md#ModelHypothesisGen), [`__init__`](__init__.md#FactorAndModelHypothesisGen.__init__), [`__init__`](__init__.md#FactorHypothesisGen.__init__), [`__init__`](__init__.md#ModelHypothesisGen.__init__)

### `ModelHypothesis2Experiment`  ·  implements/extends LLMHypothesis2Experiment
- def: [`rdagent/components/proposal/__init__.py:130`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L130)
- signature: `class ModelHypothesis2Experiment(LLMHypothesis2Experiment):`
- members:
  - `targets` — [`L133`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L133)
- protocol/private: `__init__`[`L131`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L131)
- uses (calls/refs, reference-scoped): [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`QlibModelHypothesis2Experiment`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment)
- used by: [`LLMHypothesis2Experiment`](__init__.md#LLMHypothesis2Experiment), [`QlibModelHypothesis2Experiment`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesis2Experiment)

### `ModelHypothesisGen`  ·  implements/extends LLMHypothesisGen
- def: [`rdagent/components/proposal/__init__.py:74`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L74)
- signature: `class ModelHypothesisGen(LLMHypothesisGen):`
- members:
  - `targets` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L77)
- protocol/private: `__init__`[`L75`](../../../../../../../raw/code/rd-agent/rdagent/components/proposal/__init__.py#L75)
- uses (calls/refs, reference-scoped): [`Scenario`](../../core/scenario.md#Scenario), [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](__init__.md#LLMHypothesisGen.__init__), [`QlibModelHypothesisGen`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen)
- used by: [`LLMHypothesisGen`](__init__.md#LLMHypothesisGen), [`__init__`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen.__init__), [`QlibModelHypothesisGen`](../../scenarios/qlib/proposal/model_proposal.md#QlibModelHypothesisGen)

