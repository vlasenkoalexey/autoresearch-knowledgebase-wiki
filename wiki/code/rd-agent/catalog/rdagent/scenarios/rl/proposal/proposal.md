---
title: 'Module: rdagent/scenarios/rl/proposal/proposal.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/proposal/proposal.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.proposal.proposal`/RLPostTrainingExpGen#
symbols:
  RLPostTrainingExpGen.gen: gen().
  RLPostTrainingExpGen._build_trace_summary: _build_trace_summary().
  RLPostTrainingExpGen._gen_hypothesis_with_llm: _gen_hypothesis_with_llm().
  RLPostTrainingExpGen.__init__: __init__().
  RLPostTrainingExpGen: ''
---
# Module: [`rdagent/scenarios/rl/proposal/proposal.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py)

## Classes
### `RLPostTrainingExpGen`  ·  implements/extends ExpGen
- def: [`rdagent/scenarios/rl/proposal/proposal.py:12`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py#L12)
- doc: RL post-training experiment generator with LLM.
- signature: `class RLPostTrainingExpGen(ExpGen):`
- members:
  - `_build_trace_summary(self, trace: Trace)` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py#L44) — Build summary of historical experiments. — documented in [rdagent-core-proposal](../../../../../concepts/rdagent-core-proposal.md)
  - `_gen_hypothesis_with_llm(self, trace_summary: str)` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py#L64) — Generate hypothesis using LLM.
  - `gen(self, trace: Trace)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py#L18) — Generate RL post-training experiment using LLM. — documented in [rdagent-core-proposal](../../../../../concepts/rdagent-core-proposal.md)
- protocol/private: `__init__`[`L15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/proposal/proposal.py#L15)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`hist`](../../../core/proposal.md#Trace.hist), [`Scenario`](../../../core/scenario.md#Scenario), [`Trace`](../../../core/proposal.md#Trace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Hypothesis`](../../../core/proposal.md#Hypothesis), [`ExpGen`](../../../core/proposal.md#ExpGen), [`hypothesis`](../../../core/experiment.md#Experiment.hypothesis), [`hypothesis`](../../../core/proposal.md#Hypothesis.hypothesis), [`RL_RD_SETTING`](../../../app/rl/conf.md#RL_RD_SETTING), [`decision`](../../../core/proposal.md#ExperimentFeedback.decision), [`RLExperiment`](../experiment/experiment.md#RLExperiment), [`__init__`](../../../core/proposal.md#ExpGen.__init__), [`RLTask`](../experiment/experiment.md#RLTask), [`reason`](../../../core/proposal.md#ExperimentFeedback.reason), [`base_model`](../../../app/rl/conf.md#RLPostTrainingPropSetting.base_model), [`code_change_summary`](../../../core/proposal.md#ExperimentFeedback.code_change_summary)
- used by: [`ExpGen`](../../../core/proposal.md#ExpGen), [`gen`](../../../core/proposal.md#ExpGen.gen)

