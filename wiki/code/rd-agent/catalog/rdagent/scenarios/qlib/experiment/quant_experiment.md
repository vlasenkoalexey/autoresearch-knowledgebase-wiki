---
title: 'Module: rdagent/scenarios/qlib/experiment/quant_experiment.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/qlib/experiment/quant_experiment.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.qlib.experiment.quant_experiment`/Qlib
symbols:
  QlibQuantScenario._experiment_setting: QuantScenario#_experiment_setting.
  QlibQuantScenario: QuantScenario#
  QlibQuantScenario.get_scenario_all_desc: QuantScenario#get_scenario_all_desc().
  QlibQuantScenario.simulator: QuantScenario#simulator().
  QlibQuantScenario.interface: QuantScenario#interface().
  QlibQuantScenario.get_runtime_environment: QuantScenario#get_runtime_environment().
  QlibFactorExperiment: FactorExperiment#
  QlibModelExperiment: ModelExperiment#
  QlibQuantScenario.common_description: QuantScenario#common_description().
  QlibQuantScenario.background: QuantScenario#background().
  QlibFactorExperiment.__init__: FactorExperiment#__init__().
  QlibModelExperiment.__init__: ModelExperiment#__init__().
  QlibQuantScenario._rich_style_description: QuantScenario#_rich_style_description.
  QlibQuantScenario.output_format: QuantScenario#output_format().
  QlibQuantScenario.output: QuantScenario#output().
  QlibQuantScenario.get_source_data_desc: QuantScenario#get_source_data_desc().
  QlibQuantScenario._source_data: QuantScenario#_source_data.
  QlibQuantScenario.rich_style_description: QuantScenario#rich_style_description().
  QlibQuantScenario.experiment_setting: QuantScenario#experiment_setting().
  QlibQuantScenario.source_data: QuantScenario#source_data().
  QlibQuantScenario.__init__: QuantScenario#__init__().
---
# Module: [`rdagent/scenarios/qlib/experiment/quant_experiment.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py)

## Classes
### `QlibFactorExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/qlib/experiment/quant_experiment.py:29`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L29)
- signature: `class QlibFactorExperiment(FactorExperiment[FactorTask, QlibFBWorkspace, FactorFBWorkspace]):`
- protocol/private: `__init__`[`L30`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L30)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`FactorTask`](../../../components/coder/factor_coder/factor.md#FactorTask), [`FactorFBWorkspace`](../../../components/coder/factor_coder/factor.md#FactorFBWorkspace), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`QlibFBWorkspace`](workspace.md#QlibFBWorkspace), [`FactorExperiment`](../../../components/coder/factor_coder/factor.md#FactorExperiment)
- used by: [`Experiment`](../../../core/experiment.md#Experiment)

### `QlibModelExperiment`  ·  implements/extends Experiment
- def: [`rdagent/scenarios/qlib/experiment/quant_experiment.py:35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L35)
- signature: `class QlibModelExperiment(ModelExperiment[ModelTask, QlibFBWorkspace, ModelFBWorkspace]):`
- protocol/private: `__init__`[`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L36)
- uses (calls/refs, reference-scoped): [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`ModelTask`](../../../components/coder/model_coder/model.md#ModelTask), [`ModelFBWorkspace`](../../../components/coder/model_coder/model.md#ModelFBWorkspace), [`ModelExperiment`](../../../components/coder/model_coder/model.md#ModelExperiment), [`__init__`](../../../core/experiment.md#Experiment.__init__), [`QlibFBWorkspace`](workspace.md#QlibFBWorkspace)
- used by: [`Experiment`](../../../core/experiment.md#Experiment)

### `QlibQuantScenario`  ·  implements/extends Scenario
- def: [`rdagent/scenarios/qlib/experiment/quant_experiment.py:41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L41)
- signature: `class QlibQuantScenario(Scenario):`
- members:
  - `background(self, tag=None)` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L58)
  - `common_description(action: str | None = None)` — [`L144`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L144)
  - `experiment_setting(self)` — [`L134`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L134)
  - `get_runtime_environment(self, tag: str = None)` — [`L187`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L187)
  - `get_scenario_all_desc(self, task: Task | None = None, filtered_tag: str | None = None, simple_background: bool | None = None, action: str | None = None)` — [`L137`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L137)
  - `get_source_data_desc(self)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L82)
  - `interface(self, tag=None)` — [`L101`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L101)
  - `output(tag: str | None)` — [`L164`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L164)
  - `output_format(self, tag=None)` — [`L85`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L85)
  - `rich_style_description(self)` — [`L130`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L130)
  - `simulator(self, tag=None)` — [`L117`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L117)
  - `source_data()` — [`L152`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L152)
- protocol/private: `__init__`[`L42`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L42), `_experiment_setting`[`L47`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L47), `_rich_style_description`[`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L46), `_source_data`[`L44`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/qlib/experiment/quant_experiment.py#L44)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`Scenario`](../../../core/scenario.md#Scenario), [`Task`](../../../core/experiment.md#Task), [`get_model_env`](../../../components/coder/model_coder/conf.md#get_model_env), [`get_factor_env`](../../../components/coder/factor_coder/config.md#get_factor_env), [`get_runtime_environment_by_env`](../../shared/get_runtime_info.md#get_runtime_environment_by_env), [`get_data_folder_intro`](utils.md#get_data_folder_intro), [`QUANT_PROP_SETTING`](../../../app/qlib_rd_loop/conf.md#QUANT_PROP_SETTING), [`test_end`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.test_end), [`test_start`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.test_start), [`train_end`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.train_end), [`train_start`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.train_start), [`valid_end`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.valid_end), [`valid_start`](../../../app/qlib_rd_loop/conf.md#QuantBasePropSetting.valid_start)
- used by: [`Scenario`](../../../core/scenario.md#Scenario), [`generate_feedback`](../developer/feedback.md#QlibFactorExperiment2Feedback.generate_feedback), [`generate_feedback`](../developer/feedback.md#QlibModelExperiment2Feedback.generate_feedback), [`get_scenario_all_desc`](../../../core/scenario.md#Scenario.get_scenario_all_desc), [`feedback_window`](../../../log/ui/app.md#feedback_window), [`summary_window`](../../../log/ui/app.md#summary_window), [`get_msgs_until`](../../../log/ui/app.md#get_msgs_until), [`prepare_context`](../proposal/model_proposal.md#QlibModelHypothesis2Experiment.prepare_context), [`prepare_context`](../proposal/factor_proposal.md#QlibFactorHypothesis2Experiment.prepare_context), [`SIMILAR_SCENARIOS`](../../../log/ui/app.md#SIMILAR_SCENARIOS), [`get_runtime_environment`](../../../core/scenario.md#Scenario.get_runtime_environment), [`background`](../../../core/scenario.md#Scenario.background), [`rich_style_description`](../../../core/scenario.md#Scenario.rich_style_description), [`get_source_data_desc`](../../../core/scenario.md#Scenario.get_source_data_desc), [`experiment_setting`](../../../core/scenario.md#Scenario.experiment_setting)

