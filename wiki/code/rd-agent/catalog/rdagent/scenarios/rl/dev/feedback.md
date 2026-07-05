---
title: 'Module: rdagent/scenarios/rl/dev/feedback.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/dev/feedback.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.dev.feedback`/RLExperiment2Feedback#
symbols:
  RLExperiment2Feedback._gen_feedback_with_llm: _gen_feedback_with_llm().
  RLExperiment2Feedback._gen_error_feedback: _gen_error_feedback().
  RLExperiment2Feedback.generate_feedback: generate_feedback().
  RLExperiment2Feedback.__init__: __init__().
  RLExperiment2Feedback: ''
  RLExperiment2Feedback.version: version.
---
# Module: [`rdagent/scenarios/rl/dev/feedback.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py)

## Classes
### `RLExperiment2Feedback`  ·  implements/extends Experiment2Feedback
- def: [`rdagent/scenarios/rl/dev/feedback.py:11`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L11)
- doc: Generate feedback for RL post-training experiments using LLM.
- signature: `class RLExperiment2Feedback(Experiment2Feedback):`
- members:
  - `_gen_error_feedback(self, hypothesis: str, error_info: str)` — [`L91`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L91) — Generate feedback for failed experiments.
  - `_gen_feedback_with_llm(self, hypothesis: str, task_desc: str, exit_code: int, stdout: str, running_time: float, benchmark: str | None)` — [`L51`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L51) — Generate feedback using LLM.
  - `generate_feedback(self, exp: Any, trace: Any | None = None, exception: Exception | None = None)` — [`L18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L18) — Generate feedback using LLM.
  - `version` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L16)
- protocol/private: `__init__`[`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/dev/feedback.py#L14)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`Scenario`](../../../core/scenario.md#Scenario), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`error`](../../../log/logger.md#RDAgentLog.error), [`HypothesisFeedback`](../../../core/proposal.md#HypothesisFeedback), [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`__init__`](../../../core/proposal.md#Experiment2Feedback.__init__)
- used by: [`Experiment2Feedback`](../../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../../core/proposal.md#Experiment2Feedback.generate_feedback)

