---
title: 'Module: rdagent/scenarios/qlib/proposal/factor_proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/proposal/factor_proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.proposal.factor_proposal`/QlibFactorHypothesis
symbols:
  QlibFactorHypothesis2Experiment.convert_response: 2Experiment#convert_response().
  QlibFactorHypothesis2Experiment.prepare_context: 2Experiment#prepare_context().
  QlibFactorHypothesisGen.prepare_context: Gen#prepare_context().
  QlibFactorHypothesis2Experiment: 2Experiment#
  QlibFactorHypothesisGen.__init__: Gen#__init__().
  QlibFactorHypothesisGen.convert_response: Gen#convert_response().
  QlibFactorHypothesis: .
  QlibFactorHypothesisGen: Gen#
---
# Module: [`rdagent/scenarios/qlib/proposal/factor_proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py)

## Classes
### `QlibFactorHypothesis2Experiment`  ·  implements/extends FactorHypothesis2Experiment
- def: [`rdagent/scenarios/qlib/proposal/factor_proposal.py:61`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L61)
- signature: `class QlibFactorHypothesis2Experiment(FactorHypothesis2Experiment):`
- members:
  - `convert_response(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L94`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L94)
  - `prepare_context(self, hypothesis: Hypothesis, trace: Trace)` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L62)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`hist`](../../../core/proposal.md#Trace.hist), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`QlibFactorExperiment`](../experiment/factor_experiment.md#QlibFactorExperiment), [`scen`](../../../core/proposal.md#Trace.scen), [`QlibModelExperiment`](../experiment/model_experiment.md#QlibModelExperiment), [`QlibQuantScenario`](../experiment/quant_experiment.md#QlibQuantScenario), [`get_scenario_all_desc`](../experiment/quant_experiment.md#QlibQuantScenario.get_scenario_all_desc), [`FactorExperiment`](../../../components/coder/factor_coder/factor.md#FactorExperiment), [`factor_name`](../../../components/coder/factor_coder/factor.md#FactorTask.factor_name), [`FactorHypothesis2Experiment`](../../../components/proposal/__init__.md#FactorHypothesis2Experiment)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.prepare_context), [`FactorHypothesis2Experiment`](../../../components/proposal/__init__.md#FactorHypothesis2Experiment)  (3 test-only)

### `QlibFactorHypothesisGen`  ·  implements/extends FactorHypothesisGen
- def: [`rdagent/scenarios/qlib/proposal/factor_proposal.py:15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L15)
- signature: `class QlibFactorHypothesisGen(FactorHypothesisGen):`
- members:
  - `convert_response(self, response: str)` — [`L48`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L48)
  - `prepare_context(self, trace: Trace)` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L19)
- protocol/private: `__init__`[`L16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L16)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`hist`](../../../core/proposal.md#Trace.hist), [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`FactorHypothesisGen`](../../../components/proposal/__init__.md#FactorHypothesisGen), [`__init__`](../../../components/proposal/__init__.md#FactorHypothesisGen.__init__), [`QlibFactorHypothesis`](factor_proposal.md#QlibFactorHypothesis)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesisGen.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesisGen.prepare_context), [`FactorHypothesisGen`](../../../components/proposal/__init__.md#FactorHypothesisGen)

## Module values
- `QlibFactorHypothesis` — [`L12`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/factor_proposal.py#L12)

