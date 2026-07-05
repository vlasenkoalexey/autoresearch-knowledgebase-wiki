---
title: 'Module: rdagent/scenarios/finetune/loop.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.loop`/LLMFinetuneRDLoop#
symbols:
  LLMFinetuneRDLoop.feedback: feedback().
  LLMFinetuneRDLoop.trace: trace.
  LLMFinetuneRDLoop.direct_exp_gen: direct_exp_gen().
  LLMFinetuneRDLoop.coding: coding().
  LLMFinetuneRDLoop.record: record().
  LLMFinetuneRDLoop: ''
  LLMFinetuneRDLoop.model: model.
  LLMFinetuneRDLoop.skip_loop_error: skip_loop_error.
  LLMFinetuneRDLoop.__init__: __init__().
  LLMFinetuneRDLoop.dataset: dataset.
  LLMFinetuneRDLoop.withdraw_loop_error: withdraw_loop_error.
  LLMFinetuneRDLoop.ft_rd_setting: ft_rd_setting.
---
# Module: [`rdagent/scenarios/finetune/loop.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py)

## Classes
### `LLMFinetuneRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/scenarios/finetune/loop.py:14`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L14)
- doc: LLM fine-tuning loop using standard RDLoop workflow
- signature: `class LLMFinetuneRDLoop(RDLoop):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L39`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L39) — Generate fine-tuning code
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L32`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L32) — Generate LLM fine-tuning experiment
  - `feedback(self, prev_out: dict[str, Any])` — [`L46`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L46) — Generate feedback for LLM fine-tuning experiment - always call LLM
  - `record(self, prev_out: dict[str, Any])` — [`L57`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L57) — Record the experiment and feedback into trace
  - `dataset` — [`L23`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L23)
  - `ft_rd_setting` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L22)
  - `model` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L24)
  - `skip_loop_error` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L17)
  - `trace` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L30)
  - `withdraw_loop_error` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L18)
- protocol/private: `__init__`[`L20`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/loop.py#L20)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`CoderError`](../../core/exception.md#CoderError), [`develop`](../../core/developer.md#Developer.develop), [`scen`](../../core/proposal.md#Trace.scen), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`generate_feedback`](../../core/proposal.md#Experiment2Feedback.generate_feedback), [`__init__`](../../components/workflow/rd_loop.md#RDLoop.__init__), [`sync_dag_parent_and_hist`](../../core/proposal.md#Trace.sync_dag_parent_and_hist), [`summarizer`](../../components/workflow/rd_loop.md#RDLoop.summarizer), [`coder`](../../components/workflow/rd_loop.md#RDLoop.coder), [`hypothesis_gen`](../../components/workflow/rd_loop.md#RDLoop.hypothesis_gen), [`FTTrace`](proposal/trace.md#FTTrace), [`base_model`](../../app/finetune/llm/conf.md#LLMFinetunePropSetting.base_model), [`EXCEPTION_KEY`](../../utils/workflow/loop.md#LoopBase.EXCEPTION_KEY), [`LLMFinetunePropSetting`](../../app/finetune/llm/conf.md#LLMFinetunePropSetting), [`LOOP_IDX_KEY`](../../utils/workflow/loop.md#LoopBase.LOOP_IDX_KEY), [`dataset`](../../app/finetune/llm/conf.md#LLMFinetunePropSetting.dataset)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`main`](../../app/finetune/llm/loop.md#main), [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`feedback`](../../components/workflow/rd_loop.md#RDLoop.feedback), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`record`](../../components/workflow/rd_loop.md#RDLoop.record)

