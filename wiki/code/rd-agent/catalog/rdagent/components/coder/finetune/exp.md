---
title: 'Module: rdagent/components/coder/finetune/exp.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/finetune/exp.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.finetune.exp`/FTTask#
symbols:
  FTTask.get_task_information: get_task_information().
  FTTask: ''
  FTTask.base_model: base_model.
  FTTask.__init__: __init__().
  FTTask.benchmark: benchmark.
  FTTask.involving_datasets: involving_datasets.
  FTTask.skip_data_processing: skip_data_processing.
---
# Module: [`rdagent/components/coder/finetune/exp.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py)

## Classes
### `FTTask`  ·  implements/extends CoSTEERTask
- def: [`rdagent/components/coder/finetune/exp.py:12`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L12)
- doc: Training task class for LLM fine-tuning operations - follows data science pattern
- signature: `class FTTask(CoSTEERTask):`
- members:
  - `get_task_information(self)` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L31) — Get task information for coder prompt generation
  - `base_model` — [`L26`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L26)
  - `benchmark` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L27)
  - `involving_datasets` — [`L28`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L28)
  - `skip_data_processing` — [`L29`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L29)
- protocol/private: `__init__`[`L15`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/finetune/exp.py#L15)
- uses (calls/refs, reference-scoped): [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask), [`name`](../../../core/experiment.md#AbsTask.name), [`description`](../../../core/experiment.md#Task.description), [`__init__`](../CoSTEER/task.md#CoSTEERTask.__init__)
- used by: [`evaluate`](../../../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`_gen_hypothesis`](../../../scenarios/finetune/proposal/proposal.md#LLMFinetuneExpGen._gen_hypothesis), [`get_task_information`](../../../core/experiment.md#Task.get_task_information), [`_generate_llm_feedback`](../../../scenarios/finetune/train/eval.md#FTRunnerEvaluator._generate_llm_feedback), [`CoSTEERTask`](../CoSTEER/task.md#CoSTEERTask)  (1 test-only)

