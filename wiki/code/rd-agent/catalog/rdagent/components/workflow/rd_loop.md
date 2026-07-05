---
title: 'Module: rdagent/components/workflow/rd_loop.py'
type: catalog
provenance: extracted
module: rdagent/components/workflow/rd_loop.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.workflow.rd_loop`/RDLoop#
symbols:
  RDLoop: ''
  RDLoop.direct_exp_gen: direct_exp_gen().
  RDLoop.feedback: feedback().
  RDLoop.coding: coding().
  RDLoop.plan: plan.
  RDLoop.__init__: __init__().
  RDLoop.running: running().
  RDLoop._propose: _propose().
  RDLoop._interact_init_params: _interact_init_params().
  RDLoop._exp_gen: _exp_gen().
  RDLoop._init_base_features: _init_base_features().
  RDLoop.record: record().
  RDLoop._interact_feedback: _interact_feedback().
  RDLoop._interact_hypo: _interact_hypo().
  RDLoop.summarizer: summarizer.
  RDLoop.runner: runner.
  RDLoop.coder: coder.
  RDLoop.hypothesis_gen: hypothesis_gen.
  RDLoop.trace: trace.
  RDLoop.hypothesis2experiment: hypothesis2experiment.
  RDLoop.user_request_q: user_request_q.
  RDLoop.user_response_q: user_response_q.
  RDLoop._set_interactor: _set_interactor().
---
# Module: [`rdagent/components/workflow/rd_loop.py`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py)

## Classes
### `RDLoop`  ·  implements/extends LoopBase
- def: [`rdagent/components/workflow/rd_loop.py:31`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L31) — documented in [rdagent-utils-workflow-loop](../../../../concepts/rdagent-utils-workflow-loop.md)
- signature: `class RDLoop(LoopBase, metaclass=LoopMeta):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L212`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L212)
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L199`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L199)
  - `feedback(self, prev_out: dict[str, Any])` — [`L222`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L222)
  - `record(self, prev_out: dict[str, Any])` — [`L238`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L238)
  - `running(self, prev_out: dict[str, Any])` — [`L217`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L217)
  - `coder` — [`L55`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L55)
  - `hypothesis2experiment` — [`L49`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L49)
  - `hypothesis_gen` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L38)
  - `plan` — [`L44`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L44)
  - `runner` — [`L58`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L58)
  - `summarizer` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L62)
  - `trace` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L67)
  - `user_request_q` — [`L72`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L72)
  - `user_response_q` — [`L73`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L73)
- protocol/private: `__init__`[`L33`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L33), `_exp_gen`[`L193`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L193), `_init_base_features`[`L75`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L75), `_interact_feedback`[`L169`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L169), `_interact_hypo`[`L154`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L154), `_interact_init_params`[`L112`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L112), `_propose`[`L184`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L184), `_set_interactor`[`L71`](../../../../../../../raw/code/rd-agent/rdagent/components/workflow/rd_loop.py#L71)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`warning`](../../log/logger.md#RDAgentLog.warning), [`Scenario`](../../core/scenario.md#Scenario), [`record`](../../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`Trace`](../../core/proposal.md#Trace), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`Hypothesis`](../../core/proposal.md#Hypothesis), [`direct_exp_gen`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`import_class`](../../core/utils.md#import_class), [`coding`](../../scenarios/data_science/loop.md#DataScienceRDLoop.coding), [`Developer`](../../core/developer.md#Developer), [`develop`](../../core/developer.md#Developer.develop), [`HypothesisFeedback`](../../core/proposal.md#HypothesisFeedback), [`Experiment2Feedback`](../../core/proposal.md#Experiment2Feedback), [`feedback`](../../scenarios/data_science/loop.md#DataScienceRDLoop.feedback), [`direct_exp_gen`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.direct_exp_gen), [`running`](../../app/kaggle/loop.md#KaggleRDLoop.running), [`generate_feedback`](../../core/proposal.md#Experiment2Feedback.generate_feedback), [`running`](../../scenarios/data_science/loop.md#DataScienceRDLoop.running), [`validate_qlib_features`](../../utils/qlib.md#validate_qlib_features), [`coding`](../../app/kaggle/loop.md#KaggleRDLoop.coding), [`feedback`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.feedback), [`BasePropSetting`](conf.md#BasePropSetting), [`sync_dag_parent_and_hist`](../../core/proposal.md#Trace.sync_dag_parent_and_hist), [`direct_exp_gen`](../../scenarios/data_science/loop.md#DataScienceRDLoop.direct_exp_gen), [`LoopBase`](../../utils/workflow/loop.md#LoopBase), [`running`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.running), [`ExperimentPlan`](../../core/experiment.md#ExperimentPlan), [`feedback`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.feedback), [`feedback`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.feedback), [`loop_idx`](../../utils/workflow/loop.md#LoopBase.loop_idx), [`running`](../../app/qlib_rd_loop/factor.md#FactorRDLoop.running), [`Hypothesis2Experiment`](../../core/proposal.md#Hypothesis2Experiment), [`convert`](../../core/proposal.md#Hypothesis2Experiment.convert), [`coding`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.coding), [`gen`](../../core/proposal.md#HypothesisGen.gen), [`HypothesisGen`](../../core/proposal.md#HypothesisGen), [`get_max_parallel`](../../core/conf.md#RDAgentSettings.get_max_parallel)  (+25 more)
- used by: [`direct_exp_gen`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`trace`](../../scenarios/data_science/loop.md#DataScienceRDLoop.trace), [`feedback`](../../scenarios/data_science/loop.md#DataScienceRDLoop.feedback), [`direct_exp_gen`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.direct_exp_gen), [`running`](../../scenarios/data_science/loop.md#DataScienceRDLoop.running), [`feedback`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.feedback), [`main`](../../app/qlib_rd_loop/factor.md#main), [`main`](../../app/qlib_rd_loop/model.md#main), [`main`](../../app/qlib_rd_loop/quant.md#main), [`DataScienceRDLoop`](../../scenarios/data_science/loop.md#DataScienceRDLoop), [`LoopBase`](../../utils/workflow/loop.md#LoopBase), [`feedback`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.feedback), [`feedback`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.feedback), [`running`](../../app/qlib_rd_loop/factor.md#FactorRDLoop.running), [`pipeline_coder`](../../scenarios/data_science/loop.md#DataScienceRDLoop.pipeline_coder), [`trace`](../../app/qlib_rd_loop/quant.md#QuantRDLoop.trace), [`coding`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.coding), [`coding`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.coding), [`coding`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.coding), [`direct_exp_gen`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.direct_exp_gen), [`direct_exp_gen`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.direct_exp_gen), [`FactorRDLoop`](../../app/qlib_rd_loop/factor.md#FactorRDLoop), [`trace`](../../app/kaggle/loop.md#KaggleRDLoop.trace), [`ModelRDLoop`](../../app/qlib_rd_loop/model.md#ModelRDLoop), [`LLMFinetuneRDLoop`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop), [`__init__`](../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.__init__), [`model`](../../scenarios/finetune/loop.md#LLMFinetuneRDLoop.model), [`KaggleRDLoop`](../../app/kaggle/loop.md#KaggleRDLoop), [`QuantRDLoop`](../../app/qlib_rd_loop/quant.md#QuantRDLoop), [`RLPostTrainingRDLoop`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop), [`rl_rd_setting`](../../scenarios/rl/loop.md#RLPostTrainingRDLoop.rl_rd_setting)

