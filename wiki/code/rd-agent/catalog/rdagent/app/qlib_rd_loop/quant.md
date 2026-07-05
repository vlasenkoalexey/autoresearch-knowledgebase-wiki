---
title: 'Module: rdagent/app/qlib_rd_loop/quant.py'
type: catalog
provenance: extracted
module: rdagent/app/qlib_rd_loop/quant.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.qlib_rd_loop.quant`/
symbols:
  QuantRDLoop.direct_exp_gen: QuantRDLoop#direct_exp_gen().
  QuantRDLoop.feedback: QuantRDLoop#feedback().
  main: main().
  QuantRDLoop.running: QuantRDLoop#running().
  QuantRDLoop.__init__: QuantRDLoop#__init__().
  QuantRDLoop.factor_hypothesis2experiment: QuantRDLoop#factor_hypothesis2experiment.
  QuantRDLoop.model_hypothesis2experiment: QuantRDLoop#model_hypothesis2experiment.
  QuantRDLoop.factor_coder: QuantRDLoop#factor_coder.
  QuantRDLoop.model_coder: QuantRDLoop#model_coder.
  QuantRDLoop.factor_runner: QuantRDLoop#factor_runner.
  QuantRDLoop.model_runner: QuantRDLoop#model_runner.
  QuantRDLoop.factor_summarizer: QuantRDLoop#factor_summarizer.
  QuantRDLoop.model_summarizer: QuantRDLoop#model_summarizer.
  QuantRDLoop.hypothesis_gen: QuantRDLoop#hypothesis_gen.
  QuantRDLoop.coding: QuantRDLoop#coding().
  QuantRDLoop.trace: QuantRDLoop#trace.
  QuantRDLoop.plan: QuantRDLoop#plan.
  QuantRDLoop.skip_loop_error: QuantRDLoop#skip_loop_error.
  QuantRDLoop: QuantRDLoop#
---
# Module: [`rdagent/app/qlib_rd_loop/quant.py`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py)

## Classes
### `QuantRDLoop`  ·  implements/extends RDLoop
- def: [`rdagent/app/qlib_rd_loop/quant.py:30`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L30)
- signature: `class QuantRDLoop(RDLoop):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L92)
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L74`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L74)
  - `feedback(self, prev_out: dict[str, Any])` — [`L111`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L111)
  - `running(self, prev_out: dict[str, Any])` — [`L100`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L100)
  - `factor_coder` — [`L52`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L52)
  - `factor_hypothesis2experiment` — [`L43`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L43)
  - `factor_runner` — [`L57`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L57)
  - `factor_summarizer` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L62)
  - `hypothesis_gen` — [`L40`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L40)
  - `model_coder` — [`L54`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L54)
  - `model_hypothesis2experiment` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L47)
  - `model_runner` — [`L59`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L59)
  - `model_summarizer` — [`L64`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L64)
  - `plan` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L67)
  - `skip_loop_error` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L31)
  - `trace` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L71)
- protocol/private: `__init__`[`L36`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L36)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`Scenario`](../../core/scenario.md#Scenario), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`import_class`](../../core/utils.md#import_class), [`error`](../../log/logger.md#RDAgentLog.error), [`Developer`](../../core/developer.md#Developer), [`develop`](../../core/developer.md#Developer.develop), [`HypothesisFeedback`](../../core/proposal.md#HypothesisFeedback), [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`Experiment2Feedback`](../../core/proposal.md#Experiment2Feedback), [`generate_feedback`](../../core/proposal.md#Experiment2Feedback.generate_feedback), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`FactorEmptyError`](../../core/exception.md#FactorEmptyError), [`_propose`](../../components/workflow/rd_loop.md#RDLoop._propose), [`ExperimentPlan`](../../core/experiment.md#ExperimentPlan), [`ModelEmptyError`](../../core/exception.md#ModelEmptyError), [`loop_idx`](../../utils/workflow/loop.md#LoopBase.loop_idx), [`_interact_feedback`](../../components/workflow/rd_loop.md#RDLoop._interact_feedback), [`Hypothesis2Experiment`](../../core/proposal.md#Hypothesis2Experiment), [`convert`](../../core/proposal.md#Hypothesis2Experiment.convert), [`HypothesisGen`](../../core/proposal.md#HypothesisGen), [`get_max_parallel`](../../core/conf.md#RDAgentSettings.get_max_parallel), [`get_unfinished_loop_cnt`](../../utils/workflow/loop.md#LoopBase.get_unfinished_loop_cnt), [`EXCEPTION_KEY`](../../utils/workflow/loop.md#LoopBase.EXCEPTION_KEY), [`QuantTrace`](../../scenarios/qlib/proposal/quant_proposal.md#QuantTrace), [`ALPHA20`](../../utils/qlib.md#ALPHA20), [`__init__`](../../utils/workflow/loop.md#LoopBase.__init__), [`scen`](../../components/workflow/conf.md#BasePropSetting.scen)
- used by: [`RDLoop`](../../components/workflow/rd_loop.md#RDLoop), [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`feedback`](../../components/workflow/rd_loop.md#RDLoop.feedback), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`main`](quant.md#main), [`running`](../../components/workflow/rd_loop.md#RDLoop.running)

## Functions
- `main(path=None, step_n: int | None = None, loop_n: int | None = None, all_duration: str | None = None, checkout: bool = True, base_features_path: str | None = None, **kwargs)` — [`L131`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/quant.py#L131) — Auto R&D Evolving loop for fintech factors. — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)

