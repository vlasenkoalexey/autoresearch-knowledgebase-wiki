---
title: 'Module: rdagent/app/qlib_rd_loop/conf.py'
type: catalog
provenance: extracted
module: rdagent/app/qlib_rd_loop/conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.qlib_rd_loop.conf`/
symbols:
  QUANT_PROP_SETTING: QUANT_PROP_SETTING.
  FACTOR_PROP_SETTING: FACTOR_PROP_SETTING.
  MODEL_PROP_SETTING: MODEL_PROP_SETTING.
  FactorBasePropSetting: FactorBasePropSetting#
  FACTOR_FROM_REPORT_PROP_SETTING: FACTOR_FROM_REPORT_PROP_SETTING.
  ModelBasePropSetting: ModelBasePropSetting#
  FactorFromReportPropSetting: FactorFromReportPropSetting#
  QuantBasePropSetting: QuantBasePropSetting#
  ModelBasePropSetting.test_end: ModelBasePropSetting#test_end.
  FactorBasePropSetting.test_end: FactorBasePropSetting#test_end.
  QuantBasePropSetting.action_selection: QuantBasePropSetting#action_selection.
  ModelBasePropSetting.train_start: ModelBasePropSetting#train_start.
  ModelBasePropSetting.train_end: ModelBasePropSetting#train_end.
  ModelBasePropSetting.valid_start: ModelBasePropSetting#valid_start.
  ModelBasePropSetting.valid_end: ModelBasePropSetting#valid_end.
  ModelBasePropSetting.test_start: ModelBasePropSetting#test_start.
  FactorBasePropSetting.train_start: FactorBasePropSetting#train_start.
  FactorBasePropSetting.train_end: FactorBasePropSetting#train_end.
  FactorBasePropSetting.valid_start: FactorBasePropSetting#valid_start.
  FactorBasePropSetting.valid_end: FactorBasePropSetting#valid_end.
  FactorBasePropSetting.test_start: FactorBasePropSetting#test_start.
  FactorFromReportPropSetting.max_factors_per_exp: FactorFromReportPropSetting#max_factors_per_exp.
  FactorBasePropSetting.scen: FactorBasePropSetting#scen.
  FactorFromReportPropSetting.report_result_json_file_path: FactorFromReportPropSetting#report_result_json_file_path.
  FactorFromReportPropSetting.report_limit: FactorFromReportPropSetting#report_limit.
  QuantBasePropSetting.train_start: QuantBasePropSetting#train_start.
  QuantBasePropSetting.train_end: QuantBasePropSetting#train_end.
  QuantBasePropSetting.valid_start: QuantBasePropSetting#valid_start.
  QuantBasePropSetting.valid_end: QuantBasePropSetting#valid_end.
  QuantBasePropSetting.test_start: QuantBasePropSetting#test_start.
  QuantBasePropSetting.test_end: QuantBasePropSetting#test_end.
  ModelBasePropSetting.model_config: ModelBasePropSetting#model_config.
  ModelBasePropSetting.scen: ModelBasePropSetting#scen.
  ModelBasePropSetting.hypothesis_gen: ModelBasePropSetting#hypothesis_gen.
  ModelBasePropSetting.hypothesis2experiment: ModelBasePropSetting#hypothesis2experiment.
  ModelBasePropSetting.coder: ModelBasePropSetting#coder.
  ModelBasePropSetting.runner: ModelBasePropSetting#runner.
  ModelBasePropSetting.summarizer: ModelBasePropSetting#summarizer.
  ModelBasePropSetting.evolving_n: ModelBasePropSetting#evolving_n.
  FactorBasePropSetting.model_config: FactorBasePropSetting#model_config.
  FactorBasePropSetting.hypothesis_gen: FactorBasePropSetting#hypothesis_gen.
  FactorBasePropSetting.hypothesis2experiment: FactorBasePropSetting#hypothesis2experiment.
  FactorBasePropSetting.coder: FactorBasePropSetting#coder.
  FactorBasePropSetting.runner: FactorBasePropSetting#runner.
  FactorBasePropSetting.summarizer: FactorBasePropSetting#summarizer.
  FactorBasePropSetting.evolving_n: FactorBasePropSetting#evolving_n.
  FactorFromReportPropSetting.scen: FactorFromReportPropSetting#scen.
  QuantBasePropSetting.model_config: QuantBasePropSetting#model_config.
  QuantBasePropSetting.scen: QuantBasePropSetting#scen.
  QuantBasePropSetting.quant_hypothesis_gen: QuantBasePropSetting#quant_hypothesis_gen.
  QuantBasePropSetting.model_hypothesis2experiment: QuantBasePropSetting#model_hypothesis2experiment.
  QuantBasePropSetting.model_coder: QuantBasePropSetting#model_coder.
  QuantBasePropSetting.model_runner: QuantBasePropSetting#model_runner.
  QuantBasePropSetting.model_summarizer: QuantBasePropSetting#model_summarizer.
  QuantBasePropSetting.factor_hypothesis2experiment: QuantBasePropSetting#factor_hypothesis2experiment.
  QuantBasePropSetting.factor_coder: QuantBasePropSetting#factor_coder.
  QuantBasePropSetting.factor_runner: QuantBasePropSetting#factor_runner.
  QuantBasePropSetting.factor_summarizer: QuantBasePropSetting#factor_summarizer.
  QuantBasePropSetting.evolving_n: QuantBasePropSetting#evolving_n.
---
# Module: [`rdagent/app/qlib_rd_loop/conf.py`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py)

## Classes
### `FactorBasePropSetting`  ·  implements/extends BasePropSetting
- def: [`rdagent/app/qlib_rd_loop/conf.py:52`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L52)
- signature: `class FactorBasePropSetting(BasePropSetting):`
- members:
  - `coder` — [`L65`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L65) — ---
  - `evolving_n` — [`L74`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L74) — ---
  - `hypothesis2experiment` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L62) — ---
  - `hypothesis_gen` — [`L59`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L59) — ---
  - `model_config` — [`L53`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L53)
  - `runner` — [`L68`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L68) — ---
  - `scen` — [`L56`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L56) — ---
  - `summarizer` — [`L71`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L71) — ---
  - `test_end` — [`L92`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L92) — ---
  - `test_start` — [`L89`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L89) — ---
  - `train_end` — [`L80`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L80) — ---
  - `train_start` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L77) — ---
  - `valid_end` — [`L86`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L86) — ---
  - `valid_start` — [`L83`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L83) — ---
- uses (calls/refs, reference-scoped): [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`FactorFromReportPropSetting`](conf.md#FactorFromReportPropSetting)
- used by: [`develop`](../../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`_experiment_setting`](../../scenarios/qlib/experiment/factor_experiment.md#QlibFactorScenario._experiment_setting), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`FACTOR_PROP_SETTING`](conf.md#FACTOR_PROP_SETTING), [`FactorFromReportPropSetting`](conf.md#FactorFromReportPropSetting)  (1 test-only)

### `FactorFromReportPropSetting`  ·  implements/extends FactorBasePropSetting
- def: [`rdagent/app/qlib_rd_loop/conf.py:96`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L96)
- signature: `class FactorFromReportPropSetting(FactorBasePropSetting):`
- members:
  - `max_factors_per_exp` — [`L105`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L105) — ---
  - `report_limit` — [`L108`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L108) — ---
  - `report_result_json_file_path` — [`L102`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L102) — ---
  - `scen` — [`L98`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L98) — ---
- uses (calls/refs, reference-scoped): [`FactorBasePropSetting`](conf.md#FactorBasePropSetting)
- used by: [`direct_exp_gen`](factor_from_report.md#FactorReportLoop.direct_exp_gen), [`judge_pdf_data_items`](factor_from_report.md#FactorReportLoop.judge_pdf_data_items), [`FactorBasePropSetting`](conf.md#FactorBasePropSetting), [`FACTOR_FROM_REPORT_PROP_SETTING`](conf.md#FACTOR_FROM_REPORT_PROP_SETTING)

### `ModelBasePropSetting`  ·  implements/extends BasePropSetting
- def: [`rdagent/app/qlib_rd_loop/conf.py:8`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L8)
- signature: `class ModelBasePropSetting(BasePropSetting):`
- members:
  - `coder` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L21) — ---
  - `evolving_n` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L30) — ---
  - `hypothesis2experiment` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L18) — ---
  - `hypothesis_gen` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L15) — ---
  - `model_config` — [`L9`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L9)
  - `runner` — [`L24`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L24) — ---
  - `scen` — [`L12`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L12) — ---
  - `summarizer` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L27) — ---
  - `test_end` — [`L48`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L48) — ---
  - `test_start` — [`L45`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L45) — ---
  - `train_end` — [`L36`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L36) — ---
  - `train_start` — [`L33`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L33) — ---
  - `valid_end` — [`L42`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L42) — ---
  - `valid_start` — [`L39`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L39) — ---
- uses (calls/refs, reference-scoped): [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting)
- used by: [`develop`](../../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`_experiment_setting`](../../scenarios/qlib/experiment/model_experiment.md#QlibModelScenario._experiment_setting), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`MODEL_PROP_SETTING`](conf.md#MODEL_PROP_SETTING)

### `QuantBasePropSetting`  ·  implements/extends BasePropSetting
- def: [`rdagent/app/qlib_rd_loop/conf.py:112`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L112)
- signature: `class QuantBasePropSetting(BasePropSetting):`
- members:
  - `action_selection` — [`L151`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L151) — ---
  - `evolving_n` — [`L148`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L148) — ---
  - `factor_coder` — [`L139`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L139) — ---
  - `factor_hypothesis2experiment` — [`L134`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L134) — ---
  - `factor_runner` — [`L142`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L142) — ---
  - `factor_summarizer` — [`L145`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L145) — ---
  - `model_coder` — [`L125`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L125) — ---
  - `model_config` — [`L113`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L113)
  - `model_hypothesis2experiment` — [`L122`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L122) — ---
  - `model_runner` — [`L128`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L128) — ---
  - `model_summarizer` — [`L131`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L131) — ---
  - `quant_hypothesis_gen` — [`L119`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L119) — ---
  - `scen` — [`L116`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L116) — ---
  - `test_end` — [`L169`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L169) — ---
  - `test_start` — [`L166`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L166) — ---
  - `train_end` — [`L157`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L157) — ---
  - `train_start` — [`L154`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L154) — ---
  - `valid_end` — [`L163`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L163) — ---
  - `valid_start` — [`L160`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L160) — ---
- uses (calls/refs, reference-scoped): [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting)
- used by: [`prepare_context`](../../scenarios/qlib/proposal/quant_proposal.md#QlibQuantHypothesisGen.prepare_context), [`_experiment_setting`](../../scenarios/qlib/experiment/quant_experiment.md#QlibQuantScenario._experiment_setting), [`BasePropSetting`](../../components/workflow/conf.md#BasePropSetting), [`QUANT_PROP_SETTING`](conf.md#QUANT_PROP_SETTING)

## Module values
- `FACTOR_FROM_REPORT_PROP_SETTING` — [`L174`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L174)
- `FACTOR_PROP_SETTING` — [`L173`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L173)
- `MODEL_PROP_SETTING` — [`L175`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L175)
- `QUANT_PROP_SETTING` — [`L176`](../../../../../../../raw/code/rd-agent/rdagent/app/qlib_rd_loop/conf.py#L176)

