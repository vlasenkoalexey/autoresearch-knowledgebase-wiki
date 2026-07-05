---
title: 'Module: rdagent/app/qlib_rd_loop/factor_from_report.py'
type: catalog
provenance: extracted
module: rdagent/app/qlib_rd_loop/factor_from_report.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.qlib_rd_loop.factor_from_report`/
symbols:
  FactorReportLoop.direct_exp_gen: FactorReportLoop#direct_exp_gen().
  extract_hypothesis_and_exp_from_reports: extract_hypothesis_and_exp_from_reports().
  FactorReportLoop.judge_pdf_data_items: FactorReportLoop#judge_pdf_data_items.
  generate_hypothesis: generate_hypothesis().
  main: main().
  FactorReportLoop.coding: FactorReportLoop#coding().
  FactorReportLoop: FactorReportLoop#
  FactorReportLoop.__init__: FactorReportLoop#__init__().
  FactorReportLoop.shift_report: FactorReportLoop#shift_report.
---
# Module: [`rdagent/app/qlib_rd_loop/factor_from_report.py`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py)

## Classes
### `FactorReportLoop`  ·  implements/extends FactorRDLoop
- def: [`rdagent/app/qlib_rd_loop/factor_from_report.py:97`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L97)
- signature: `class FactorReportLoop(FactorRDLoop, metaclass=LoopMeta):`
- members:
  - `coding(self, prev_out: dict[str, Any])` — [`L137`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L137)
  - `direct_exp_gen(self, prev_out: dict[str, Any])` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L112)
  - `judge_pdf_data_items` — [`L101`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L101)
  - `shift_report` — [`L108`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L108)
- protocol/private: `__init__`[`L98`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L98)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`hist`](../../core/proposal.md#Trace.hist), [`log_object`](../../log/logger.md#RDAgentLog.log_object), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`based_experiments`](../../core/experiment.md#Experiment.based_experiments), [`sub_tasks`](../../core/experiment.md#Experiment.sub_tasks), [`hypothesis`](../../core/experiment.md#Experiment.hypothesis), [`develop`](../../core/developer.md#Developer.develop), [`QlibFactorExperiment`](../../scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment), [`extract_hypothesis_and_exp_from_reports`](factor_from_report.md#extract_hypothesis_and_exp_from_reports), [`sub_workspace_list`](../../core/experiment.md#Experiment.sub_workspace_list), [`plan`](../../components/workflow/rd_loop.md#RDLoop.plan), [`__init__`](../../components/workflow/rd_loop.md#RDLoop.__init__), [`loop_idx`](../../utils/workflow/loop.md#LoopBase.loop_idx), [`coder`](../../components/workflow/rd_loop.md#RDLoop.coder), [`get_max_parallel`](../../core/conf.md#RDAgentSettings.get_max_parallel), [`get_unfinished_loop_cnt`](../../utils/workflow/loop.md#LoopBase.get_unfinished_loop_cnt), [`trace`](../../components/workflow/rd_loop.md#RDLoop.trace), [`FactorRDLoop`](factor.md#FactorRDLoop), [`FACTOR_FROM_REPORT_PROP_SETTING`](conf.md#FACTOR_FROM_REPORT_PROP_SETTING), [`LoopMeta`](../../utils/workflow/loop.md#LoopMeta), [`loop_n`](../../utils/workflow/loop.md#LoopBase.loop_n), [`base_features`](../../scenarios/qlib/experiment/factor_experiment.md#QlibFactorExperiment.base_features), [`LoopTerminationError`](../../utils/workflow/loop.md#LoopBase.LoopTerminationError), [`max_factors_per_exp`](conf.md#FactorFromReportPropSetting.max_factors_per_exp), [`report_limit`](conf.md#FactorFromReportPropSetting.report_limit), [`report_result_json_file_path`](conf.md#FactorFromReportPropSetting.report_result_json_file_path)
- used by: [`direct_exp_gen`](../../components/workflow/rd_loop.md#RDLoop.direct_exp_gen), [`coding`](../../components/workflow/rd_loop.md#RDLoop.coding), [`main`](factor_from_report.md#main), [`FactorRDLoop`](factor.md#FactorRDLoop)

## Functions
- `extract_hypothesis_and_exp_from_reports(report_file_path: str)` — [`L61`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L61) — Extract hypothesis and experiment details from report files.
- `generate_hypothesis(factor_result: dict, report_content: str)` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L26) — Generate a hypothesis based on factor results and report content.
- `main(report_folder=None, path=None, all_duration=None, checkout=True)` — [`L143`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/factor_from_report.py#L143) — Auto R&D Evolving loop for fintech factors (the factors are extracted from finance reports).

