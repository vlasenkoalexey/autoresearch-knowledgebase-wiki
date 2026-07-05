---
title: 'Module: rdagent/scenarios/qlib/proposal/model_proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/proposal/model_proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.proposal.model_proposal`/QlibModelHypothesis
symbols:
  QlibModelHypothesis2Experiment.prepare_context: 2Experiment#prepare_context().
  QlibModelHypothesis2Experiment.convert_response: 2Experiment#convert_response().
  QlibModelHypothesisGen.prepare_context: Gen#prepare_context().
  QlibModelHypothesis2Experiment: 2Experiment#
  QlibModelHypothesisGen.__init__: Gen#__init__().
  QlibModelHypothesisGen.convert_response: Gen#convert_response().
  QlibModelHypothesis: .
  QlibModelHypothesisGen: Gen#
---
# Module: [`rdagent/scenarios/qlib/proposal/model_proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py)

## Classes
### `QlibModelHypothesis2Experiment`  ·  implements/extends ModelHypothesis2Experiment
- def: [`rdagent/scenarios/qlib/proposal/model_proposal.py:73`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L73)
- signature: `class QlibModelHypothesis2Experiment(ModelHypothesis2Experiment):`
- members:
  - `convert_response(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L134`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L134)
  - `prepare_context(self, hypothesis: Hypothesis, trace: Trace)` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L74)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`hist`](../../../core/proposal.md#Trace.hist), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`ModelTask`](../../../components/coder/model_coder/model.md#ModelTask), [`scen`](../../../core/proposal.md#Trace.scen), [`QlibModelExperiment`](../experiment/model_experiment.md#QlibModelExperiment), [`decision`](../../../core/proposal.md#ExperimentFeedback.decision), [`ModelExperiment`](../../../components/coder/model_coder/model.md#ModelExperiment), [`QlibQuantScenario`](../experiment/quant_experiment.md#QlibQuantScenario), [`get_scenario_all_desc`](../experiment/quant_experiment.md#QlibQuantScenario.get_scenario_all_desc), [`ModelHypothesis2Experiment`](../../../components/proposal/__init__.md#ModelHypothesis2Experiment)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.prepare_context), [`ModelHypothesis2Experiment`](../../../components/proposal/__init__.md#ModelHypothesis2Experiment)  (3 test-only)

### `QlibModelHypothesisGen`  ·  implements/extends ModelHypothesisGen
- def: [`rdagent/scenarios/qlib/proposal/model_proposal.py:14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L14)
- signature: `class QlibModelHypothesisGen(ModelHypothesisGen):`
- members:
  - `convert_response(self, response: str)` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L60)
  - `prepare_context(self, trace: Trace)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L18)
- protocol/private: `__init__`[`L15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L15)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`hist`](../../../core/proposal.md#Trace.hist), [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`decision`](../../../core/proposal.md#ExperimentFeedback.decision), [`ModelHypothesisGen`](../../../components/proposal/__init__.md#ModelHypothesisGen), [`__init__`](../../../components/proposal/__init__.md#ModelHypothesisGen.__init__), [`QlibModelHypothesis`](model_proposal.md#QlibModelHypothesis)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesisGen.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesisGen.prepare_context), [`ModelHypothesisGen`](../../../components/proposal/__init__.md#ModelHypothesisGen)

## Module values
- `QlibModelHypothesis` — [`L11`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/proposal/model_proposal.py#L11)

