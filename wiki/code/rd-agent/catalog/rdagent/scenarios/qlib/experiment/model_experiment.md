---
title: 'Module: rdagent/scenarios/qlib/experiment/model_experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/experiment/model_experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.experiment.model_experiment`/QlibModel
symbols:
  QlibModelExperiment: Experiment#
  QlibModelScenario._experiment_setting: Scenario#_experiment_setting.
  QlibModelScenario.get_scenario_all_desc: Scenario#get_scenario_all_desc().
  QlibModelScenario: Scenario#
  QlibModelScenario._background: Scenario#_background.
  QlibModelExperiment.__init__: Experiment#__init__().
  QlibModelScenario._output_format: Scenario#_output_format.
  QlibModelScenario._interface: Scenario#_interface.
  QlibModelScenario._simulator: Scenario#_simulator.
  QlibModelScenario._rich_style_description: Scenario#_rich_style_description.
  QlibModelScenario.get_runtime_environment: Scenario#get_runtime_environment().
  QlibModelScenario.background: Scenario#background().
  QlibModelScenario.output_format: Scenario#output_format().
  QlibModelScenario.interface: Scenario#interface().
  QlibModelScenario.simulator: Scenario#simulator().
  QlibModelScenario.rich_style_description: Scenario#rich_style_description().
  QlibModelScenario.experiment_setting: Scenario#experiment_setting().
  QlibModelExperiment.base_features: Experiment#base_features.
  QlibModelExperiment.stdout: Experiment#stdout.
  QlibModelScenario.__init__: Scenario#__init__().
  QlibModelScenario.source_data: Scenario#source_data().
---
# Module: [`rdagent/scenarios/qlib/experiment/model_experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py)

## Classes
### `QlibModelExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/qlib/experiment/model_experiment.py:18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L18) — documented in [rdagent-log-ui-web](../../../../../concepts/rdagent-log-ui-web.md)
- signature: `class QlibModelExperiment(ModelExperiment[ModelTask, QlibFBWorkspace, ModelFBWorkspace]):`
- members:
  - `base_features` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L23)
  - `stdout` — [`L22`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L22)
- protocol/private: `__init__`[`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L19)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`ModelTask`](../../../components/coder/model_coder/model.md#ModelTask), [`ModelFBWorkspace`](../../../components/coder/model_coder/model.md#ModelFBWorkspace), [`ModelExperiment`](../../../components/coder/model_coder/model.md#ModelExperiment), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`QlibFBWorkspace`](workspace.md#QlibFBWorkspace)
- used by: [`Experiment`](../../../core/experiment.md#Experiment), [`develop`](../developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../developer/model_runner.md#QlibModelRunner.develop), [`consume_msg`](../../../log/ui/web.md#SimpleTraceWindow.consume_msg), [`consume_msg`](../../../log/ui/web.md#FeedbackWindow.consume_msg), [`consume_msg`](../../../log/ui/web.md#QlibModelExpWindow.consume_msg), [`convert_response`](../proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.convert_response), [`research_window`](../../../log/ui/app.md#research_window), [`load`](../../../components/coder/model_coder/task_loader.md#ModelExperimentLoaderFromPDFfiles.load), [`convert_response`](../proposal/model_proposal.md#QlibModelHypothesis2Experiment.convert_response), [`load`](../../../components/coder/model_coder/task_loader.md#ModelExperimentLoaderFromDict.load), [`QlibModelRunner`](../developer/model_runner.md#QlibModelRunner)  (1 test-only)

### `QlibModelScenario`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/qlib/experiment/model_experiment.py:26`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L26)
- signature: `class QlibModelScenario(Scenario):`
- members:
  - `background(self)` — [`L50`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L50)
  - `experiment_setting(self)` — [`L74`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L74)
  - `get_runtime_environment(self)` — [`L90`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L90)
  - `get_scenario_all_desc(self, task: Task | None = None, filtered_tag: str | None = None, simple_background: bool | None = None)` — [`L77`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L77)
  - `interface(self)` — [`L62`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L62)
  - `output_format(self)` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L58)
  - `rich_style_description(self)` — [`L70`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L70)
  - `simulator(self)` — [`L66`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L66)
  - `source_data(self)` — [`L54`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L54)
- protocol/private: `__init__`[`L27`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L27), `_background`[`L29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L29), `_experiment_setting`[`L38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L38), `_interface`[`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L35), `_output_format`[`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L34), `_rich_style_description`[`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L37), `_simulator`[`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/model_experiment.py#L36)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`Scenario`](../../../core/scenario.md#Scenario), [`Task`](../../../core/experiment.md#Task), [`get_model_env`](../../../components/coder/model_coder/conf.md#get_model_env), [`get_runtime_environment_by_env`](../../shared/get_runtime_info.md#get_runtime_environment_by_env), [`MODEL_PROP_SETTING`](../../../app/qlib_rd_loop/conf.md#MODEL_PROP_SETTING), [`test_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.test_end), [`test_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.test_start), [`train_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.train_end), [`train_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.train_start), [`valid_end`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.valid_end), [`valid_start`](../../../app/qlib_rd_loop/conf.md#ModelBasePropSetting.valid_start)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`feedback_window`](../../../log/ui/app.md#feedback_window), [`get_msgs_until`](../../../log/ui/app.md#get_msgs_until), [`SIMILAR_SCENARIOS`](../../../log/ui/app.md#SIMILAR_SCENARIOS), [`get_runtime_environment`](../../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../../core/scenario.md#Scenario.background), [`rich_style_description`](../../../core/scenario.md#Scenario.rich_style_description), [`source_data`](../../../core/scenario.md#Scenario.source_data), [`experiment_setting`](../../../core/scenario.md#Scenario.experiment_setting), [`show_common_logs`](../../../log/ui/web.md#TraceWindow.show_common_logs)  (1 test-only)

