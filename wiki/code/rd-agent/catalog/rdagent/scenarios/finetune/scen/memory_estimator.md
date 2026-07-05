---
title: 'Module: rdagent/scenarios/finetune/scen/memory_estimator.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/scen/memory_estimator.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.scen.memory_estimator`/MemoryEstimator#
symbols:
  MemoryEstimator.format: format().
  MemoryEstimator._base_memory: _base_memory().
  MemoryEstimator._find_max_seq_len: _find_max_seq_len().
  MemoryEstimator.MEM_FACTOR: MEM_FACTOR.
  MemoryEstimator.params_b: params_b.
  MemoryEstimator.layers: layers.
  MemoryEstimator.from_model_name: from_model_name().
  MemoryEstimator.estimate: estimate().
  MemoryEstimator: ''
  MemoryEstimator.total_mem: total_mem.
  MemoryEstimator.hidden: hidden.
  MemoryEstimator.ARCH: ARCH.
  MemoryEstimator.DEFAULT_LORA_RANK: DEFAULT_LORA_RANK.
  MemoryEstimator.gpu_mem: gpu_mem.
  MemoryEstimator.num_gpus: num_gpus.
  MemoryEstimator.max_ctx: max_ctx.
  MemoryEstimator._activation_factor: _activation_factor().
  MemoryEstimator.__init__: __init__().
---
# Module: [`rdagent/scenarios/finetune/scen/memory_estimator.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py)

## Classes
### `MemoryEstimator`
- def: [`rdagent/scenarios/finetune/scen/memory_estimator.py:10`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L10)
- doc: Calculate memory constraints for fine-tuning methods.
- signature: `class MemoryEstimator:`
- members:
  - `_activation_factor(self, method: str)` — [`L87`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L87) — Activation memory factor (gradient checkpointing reduces this).
  - `_base_memory(self, method: str)` — [`L73`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L73) — Base memory without activations (GB).
  - `_find_max_seq_len(self, method: str, batch_size: int = 1)` — [`L91`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L91) — Find max seq_len that fits in memory.
  - `estimate(self)` — [`L105`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L105) — Calculate max seq_len for each method (batch=1).
  - `format(self, estimates: dict[str, int] = None)` — [`L110`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L110) — Format as constraint table.
  - `from_model_name(cls, name: str, gpu_mem: float, num_gpus: int, model_specs: str = "")` — [`L52`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L52) — Create from model name and specs.
  - `ARCH` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L22)
  - `DEFAULT_LORA_RANK` — [`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L30)
  - `MEM_FACTOR` — [`L14`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L14)
  - `gpu_mem` — [`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L40)
  - `hidden` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L46)
  - `layers` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L46)
  - `max_ctx` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L43)
  - `num_gpus` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L41)
  - `params_b` — [`L39`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L39)
  - `total_mem` — [`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L42)
- protocol/private: `__init__`[`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/scen/memory_estimator.py#L32)
- used by: [`_generate_memory_report`](scenario.md#LLMFinetuneScen._generate_memory_report)

