---
title: 'Module: rdagent/scenarios/qlib/experiment/factor_experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/experiment/factor_experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.experiment.factor_experiment`/QlibFactor
symbols:
  QlibFactorExperiment: Experiment#
  QlibFactorScenario._experiment_setting: Scenario#_experiment_setting.
  QlibFactorScenario.get_scenario_all_desc: Scenario#get_scenario_all_desc().
  QlibFactorScenario: Scenario#
  QlibFactorScenario._background: Scenario#_background.
  QlibFactorExperiment.__init__: Experiment#__init__().
  QlibFactorScenario._output_format: Scenario#_output_format.
  QlibFactorScenario._interface: Scenario#_interface.
  QlibFactorScenario._simulator: Scenario#_simulator.
  QlibFactorScenario._rich_style_description: Scenario#_rich_style_description.
  QlibFactorScenario.get_source_data_desc: Scenario#get_source_data_desc().
  QlibFactorScenario.get_runtime_environment: Scenario#get_runtime_environment().
  QlibFactorExperiment.base_features: Experiment#base_features.
  QlibFactorScenario._strategy: Scenario#_strategy.
  QlibFactorScenario.rich_style_description: Scenario#rich_style_description().
  QlibFactorScenario.background: Scenario#background().
  QlibFactorScenario._source_data: Scenario#_source_data.
  QlibFactorScenario.output_format: Scenario#output_format().
  QlibFactorScenario.interface: Scenario#interface().
  QlibFactorScenario.simulator: Scenario#simulator().
  QlibFactorScenario.experiment_setting: Scenario#experiment_setting().
  QlibFactorExperiment.base_feature_codes: Experiment#base_feature_codes.
  QlibFactorExperiment.stdout: Experiment#stdout.
  QlibFactorScenario.__init__: Scenario#__init__().
---
# Module: [`rdagent/scenarios/qlib/experiment/factor_experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py)

## Classes
### `QlibFactorExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/qlib/experiment/factor_experiment.py:19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L19) — documented in [rdagent-core-experiment](../../../../../concepts/rdagent-core-experiment.md)
- signature: `class QlibFactorExperiment(FactorExperiment[FactorTask, QlibFBWorkspace, FactorFBWorkspace]):`
- members:
  - `base_feature_codes` — [`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L27)
  - `base_features` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L24)
  - `stdout` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L23)
- protocol/private: `__init__`[`L20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L20)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`FactorFBWorkspace`](../../../components/coder/factor_coder/factor.md#FactorFBWorkspace), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`QlibFBWorkspace`](workspace.md#QlibFBWorkspace), [`FactorExperiment`](../../../components/coder/factor_coder/factor.md#FactorExperiment)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`develop`](../developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../developer/model_runner.md#QlibModelRunner.develop), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`direct_exp_gen`](../../../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.direct_exp_gen), [`extract_hypothesis_and_exp_from_reports`](../../../app/qlib_rd_loop/factor_from_report.md#extract_hypothesis_and_exp_from_reports), [`process_factor_data`](../developer/utils.md#process_factor_data), [`consume_msg`](../../../log/ui/web.md#TraceObjWindow.consume_msg), [`consume_msg`](../../../log/ui/web.md#FeedbackWindow.consume_msg), [`consume_msg`](../../../log/ui/web.md#QlibFactorExpWindow.consume_msg), [`load`](../factor_experiment_loader/pdf_loader.md#FactorExperimentLoaderFromPDFfiles.load), [`convert_response`](../proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`_build_execute_calls`](../developer/utils.md#_build_execute_calls), [`_build_base_feature_workspaces`](../developer/utils.md#_build_base_feature_workspaces), [`load`](../factor_experiment_loader/json_loader.md#FactorExperimentLoaderFromDict.load), [`QlibFactorRunner`](../developer/factor_runner.md#QlibFactorRunner)

### `QlibFactorScenario`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/qlib/experiment/factor_experiment.py:30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L30)
- signature: `class QlibFactorScenario(Scenario):`
- members:
  - `background(self)` — [`L56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L56)
  - `experiment_setting(self)` — [`L79`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L79)
  - `get_runtime_environment(self)` — [`L101`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L101)
  - `get_scenario_all_desc(self, task: Task | None = None, filtered_tag: str | None = None, simple_background: bool | None = None)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L82) — A static scenario describer
  - `get_source_data_desc(self, task: Task | None = None)` — [`L59`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L59)
  - `interface(self)` — [`L67`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L67)
  - `output_format(self)` — [`L63`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L63)
  - `rich_style_description(self)` — [`L75`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L75)
  - `simulator(self)` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L71)
- protocol/private: `__init__`[`L31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L31), `_background`[`L33`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L33), `_experiment_setting`[`L44`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L44), `_interface`[`L40`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L40), `_output_format`[`L39`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L39), `_rich_style_description`[`L43`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L43), `_simulator`[`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L42), `_source_data`[`L38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L38), `_strategy`[`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/factor_experiment.py#L41)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`Scenario`](../../../core/scenario.md#Scenario), [`Task`](../../../core/experiment.md#Task), [`get_factor_env`](../../../components/coder/factor_coder/config.md#get_factor_env), [`get_runtime_environment_by_env`](../../shared/get_runtime_info.md#get_runtime_environment_by_env), [`get_data_folder_intro`](utils.md#get_data_folder_intro), [`FACTOR_PROP_SETTING`](../../../app/qlib_rd_loop/conf.md#FACTOR_PROP_SETTING), [`QlibFactorFromReportScenario`](factor_from_report_experiment.md#QlibFactorFromReportScenario), [`test_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.test_end), [`rich_style_description`](factor_from_report_experiment.md#QlibFactorFromReportScenario.rich_style_description), [`test_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.test_start), [`train_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.train_end), [`train_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.train_start), [`valid_end`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.valid_end), [`valid_start`](../../../app/qlib_rd_loop/conf.md#FactorBasePropSetting.valid_start)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`feedback_window`](../../../log/ui/app.md#feedback_window), [`summary_window`](../../../log/ui/app.md#summary_window), [`get_msgs_until`](../../../log/ui/app.md#get_msgs_until), [`SIMILAR_SCENARIOS`](../../../log/ui/app.md#SIMILAR_SCENARIOS), [`get_runtime_environment`](../../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../../core/scenario.md#Scenario.background), [`rich_style_description`](../../../core/scenario.md#Scenario.rich_style_description), [`get_source_data_desc`](../../../core/scenario.md#Scenario.get_source_data_desc), [`QlibFactorFromReportScenario`](factor_from_report_experiment.md#QlibFactorFromReportScenario), [`__init__`](factor_from_report_experiment.md#QlibFactorFromReportScenario.__init__), [`experiment_setting`](../../../core/scenario.md#Scenario.experiment_setting)

