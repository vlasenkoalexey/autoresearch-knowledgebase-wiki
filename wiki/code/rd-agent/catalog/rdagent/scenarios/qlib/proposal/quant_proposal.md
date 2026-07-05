---
title: 'Module: rdagent/scenarios/qlib/proposal/quant_proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/proposal/quant_proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.proposal.quant_proposal`/Q
symbols:
  QlibQuantHypothesisGen.prepare_context: libQuantHypothesisGen#prepare_context().
  QlibQuantHypothesisGen.targets: libQuantHypothesisGen#targets.
  QlibQuantHypothesis.__str__: libQuantHypothesis#__str__().
  QuantTrace.__init__: uantTrace#__init__().
  QlibQuantHypothesisGen.__init__: libQuantHypothesisGen#__init__().
  QlibQuantHypothesisGen.convert_response: libQuantHypothesisGen#convert_response().
  QuantTrace: uantTrace#
  QlibQuantHypothesis: libQuantHypothesis#
  QuantTrace.controller: uantTrace#controller.
  QlibQuantHypothesis.__init__: libQuantHypothesis#__init__().
  QlibQuantHypothesisGen: libQuantHypothesisGen#
  QlibQuantHypothesis.action: libQuantHypothesis#action.
---
# Module: [`rdagent/scenarios/qlib/proposal/quant_proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py)

## Classes
### `QlibQuantHypothesis`  ·  implements/extends Hypothesis
- def: [`rdagent/scenarios/qlib/proposal/quant_proposal.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L23)
- signature: `class QlibQuantHypothesis(Hypothesis):`
- members:
  - `action` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L37)
- protocol/private: `__init__`[`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L24), `__str__`[`L39`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L39)
- uses (calls/refs, reference-scoped): [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`reason`](../../../core/proposal.md#Hypothesis.reason), [`__init__`](../../../core/proposal.md#Hypothesis.__init__)
- used by: [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`convert_response`](quant_proposal.md#QlibQuantHypothesisGen.convert_response)

### `QlibQuantHypothesisGen`  ·  implements/extends FactorAndModelHypothesisGen
- def: [`rdagent/scenarios/qlib/proposal/quant_proposal.py:46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L46)
- signature: `class QlibQuantHypothesisGen(FactorAndModelHypothesisGen):`
- members:
  - `convert_response(self, response: str)` — [`L168`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L168)
  - `prepare_context(self, trace: Trace)` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L50)
  - `targets` — [`L88`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L88)
- protocol/private: `__init__`[`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L47)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`hist`](../../../core/proposal.md#Trace.hist), [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`scen`](../../../core/proposal.md#Trace.scen), [`extract_metrics_from_experiment`](bandit.md#extract_metrics_from_experiment), [`decision`](../../../core/proposal.md#ExperimentFeedback.decision), [`QUANT_PROP_SETTING`](../../../app/qlib_rd_loop/conf.md#QUANT_PROP_SETTING), [`FactorAndModelHypothesisGen`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen), [`__init__`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen.__init__), [`QlibQuantHypothesis`](quant_proposal.md#QlibQuantHypothesis), [`action_selection`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.action_selection)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesisGen.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesisGen.prepare_context), [`FactorAndModelHypothesisGen`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen)

### `QuantTrace`  ·  implements/extends Trace
- def: [`rdagent/scenarios/qlib/proposal/quant_proposal.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L16)
- signature: `class QuantTrace(Trace):`
- members:
  - `controller` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L20)
- protocol/private: `__init__`[`L17`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/quant_proposal.py#L17)
- uses (calls/refs, reference-scoped): [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`__init__`](../../../core/proposal.md#Trace.__init__), [`EnvController`](bandit.md#EnvController)
- used by: [`Trace`](../../../core/proposal.md#Trace), [`trace`](../../../app/qlib_rd_loop/quant.md#QuantRDLoop.trace)

