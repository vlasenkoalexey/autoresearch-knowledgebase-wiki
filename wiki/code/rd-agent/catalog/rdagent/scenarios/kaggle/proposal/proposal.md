---
title: 'Module: rdagent/scenarios/kaggle/proposal/proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/proposal/proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.proposal.proposal`/
symbols:
  generate_RAG_content: generate_RAG_content().
  KGHypothesis2Experiment.convert_model_experiment: KGHypothesis2Experiment#convert_model_experiment().
  KGHypothesis2Experiment.convert_response: KGHypothesis2Experiment#convert_response().
  KGHypothesis2Experiment.current_action: KGHypothesis2Experiment#current_action.
  KGHypothesis2Experiment.prepare_context: KGHypothesis2Experiment#prepare_context().
  KGHypothesisGen.prepare_context: KGHypothesisGen#prepare_context().
  KGHypothesis.__str__: KGHypothesis#__str__().
  KGHypothesis2Experiment.convert_feature_experiment: KGHypothesis2Experiment#convert_feature_experiment().
  KGTrace: KGTrace#
  KGHypothesisGen.update_reward_estimates: KGHypothesisGen#update_reward_estimates().
  KGHypothesisGen.execute_next_action: KGHypothesisGen#execute_next_action().
  KGHypothesisGen.__init__: KGHypothesisGen#__init__().
  KGHypothesisGen.convert_response: KGHypothesisGen#convert_response().
  KGHypothesis: KGHypothesis#
  KGHypothesis.action: KGHypothesis#action.
  KGHypothesis.__init__: KGHypothesis#__init__().
  KGHypothesisGen: KGHypothesisGen#
  KGHypothesis2Experiment: KGHypothesis2Experiment#
---
# Module: [`rdagent/scenarios/kaggle/proposal/proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py)

## Classes
### `KGHypothesis`  ·  implements/extends Hypothesis
- def: [`rdagent/scenarios/kaggle/proposal/proposal.py:31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L31)
- signature: `class KGHypothesis(Hypothesis):`
- members:
  - `action` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L45)
- protocol/private: `__init__`[`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L32), `__str__`[`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L47)
- uses (calls/refs, reference-scoped): [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`reason`](../../../core/proposal.md#Hypothesis.reason), [`concise_reason`](../../../core/proposal.md#Hypothesis.concise_reason), [`__init__`](../../../core/proposal.md#Hypothesis.__init__), [`concise_justification`](../../../core/proposal.md#Hypothesis.concise_justification), [`concise_knowledge`](../../../core/proposal.md#Hypothesis.concise_knowledge), [`concise_observation`](../../../core/proposal.md#Hypothesis.concise_observation)
- used by: [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`current_action`](proposal.md#KGHypothesis2Experiment.current_action), [`prepare_context`](proposal.md#KGHypothesis2Experiment.prepare_context), [`convert_response`](proposal.md#KGHypothesisGen.convert_response)

### `KGHypothesis2Experiment`  ·  implements/extends FactorAndModelHypothesis2Experiment
- def: [`rdagent/scenarios/kaggle/proposal/proposal.py:307`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L307)
- signature: `class KGHypothesis2Experiment(FactorAndModelHypothesis2Experiment):`
- members:
  - `convert_feature_experiment(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L348`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L348)
  - `convert_model_experiment(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L376`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L376)
  - `convert_response(self, response: str, hypothesis: Hypothesis, trace: Trace)` — [`L412`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L412)
  - `prepare_context(self, hypothesis: Hypothesis, trace: Trace)` — [`L308`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L308)
  - `current_action` — [`L316`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L316)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`hist`](../../../core/proposal.md#Trace.hist), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`ModelTask`](../../../components/coder/model_coder/model.md#ModelTask), [`scen`](../../../core/proposal.md#Trace.scen), [`generate_RAG_content`](proposal.md#generate_RAG_content), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`KGModelExperiment`](../experiment/kaggle_experiment.md#KGModelExperiment), [`KGFactorExperiment`](../experiment/kaggle_experiment.md#KGFactorExperiment), [`ModelExperiment`](../../../components/coder/model_coder/model.md#ModelExperiment), [`KG_SELECT_MAPPING`](../experiment/kaggle_experiment.md#KG_SELECT_MAPPING), [`ModelEmptyError`](../../../core/exception.md#ModelEmptyError), [`KG_MODEL_MAPPING`](../experiment/kaggle_experiment.md#KG_MODEL_MAPPING), [`FactorAndModelHypothesis2Experiment`](../../../components/proposal/__init__.md#FactorAndModelHypothesis2Experiment), [`KG_ACTION_FEATURE_ENGINEERING`](../experiment/scenario.md#KG_ACTION_FEATURE_ENGINEERING), [`KG_ACTION_FEATURE_PROCESSING`](../experiment/scenario.md#KG_ACTION_FEATURE_PROCESSING), [`KG_ACTION_MODEL_FEATURE_SELECTION`](../experiment/scenario.md#KG_ACTION_MODEL_FEATURE_SELECTION), [`KGHypothesis`](proposal.md#KGHypothesis), [`action`](proposal.md#KGHypothesis.action), [`KG_ACTION_MODEL_TUNING`](../experiment/scenario.md#KG_ACTION_MODEL_TUNING)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesis2Experiment.prepare_context), [`FactorAndModelHypothesis2Experiment`](../../../components/proposal/__init__.md#FactorAndModelHypothesis2Experiment)

### `KGHypothesisGen`  ·  implements/extends FactorAndModelHypothesisGen
- def: [`rdagent/scenarios/kaggle/proposal/proposal.py:185`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L185)
- doc: # NOTE: we can share this class across different data mining scenarios
- signature: `class KGHypothesisGen(FactorAndModelHypothesisGen):`
- members:
  - `convert_response(self, response: str)` — [`L291`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L291)
  - `execute_next_action(self, trace: Trace)` — [`L228`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L228)
  - `prepare_context(self, trace: Trace)` — [`L250`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L250)
  - `update_reward_estimates(self, trace: Trace)` — [`L200`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L200)
- protocol/private: `__init__`[`L197`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L197)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`hist`](../../../core/proposal.md#Trace.hist), [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`based_experiments`](../../../core/experiment.md#Experiment.based_experiments), [`generate_RAG_content`](proposal.md#generate_RAG_content), [`scen`](../../../core/proposal.md#HypothesisGen.scen), [`FactorAndModelHypothesisGen`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen), [`__init__`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen.__init__), [`KGHypothesis`](proposal.md#KGHypothesis)
- used by: [`convert_response`](../../../components/proposal/__init__.md#LLMHypothesisGen.convert_response), [`prepare_context`](../../../components/proposal/__init__.md#LLMHypothesisGen.prepare_context), [`FactorAndModelHypothesisGen`](../../../components/proposal/__init__.md#FactorAndModelHypothesisGen)

### `KGTrace`  ·  implements/extends Trace
- def: [`rdagent/scenarios/kaggle/proposal/proposal.py:419`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L419)
- signature: `class KGTrace(Trace[KGScenario, KGKnowledgeGraph]):`
- uses (calls/refs, reference-scoped): [`Trace`](../../../core/proposal.md#Trace), [`KGScenario`](../experiment/scenario.md#KGScenario), [`KGKnowledgeGraph`](../knowledge_management/graph.md#KGKnowledgeGraph)
- used by: [`Trace`](../../../core/proposal.md#Trace), [`trace`](../../../app/kaggle/loop.md#KaggleRDLoop.trace)

## Functions
- `generate_RAG_content(scen: KGScenario, trace: Trace, hypothesis_and_feedback: str, target: str = None, chosen_hypothesis: str = None, chosen_hypothesis_type: str = None)` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/proposal/proposal.py#L58)

