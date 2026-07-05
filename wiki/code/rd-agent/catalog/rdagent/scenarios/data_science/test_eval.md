---
title: 'Module: rdagent/scenarios/data_science/test_eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/test_eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.test_eval`/
symbols:
  TestEval.valid: TestEval#valid().
  TestEval.eval: TestEval#eval().
  get_test_eval: get_test_eval().
  MLETestEval.env: MLETestEval#env.
  MLETestEval.valid: MLETestEval#valid().
  MLETestEval.eval: MLETestEval#eval().
  TestEvalBase.valid: TestEvalBase#valid().
  TestEvalBase.eval: TestEvalBase#eval().
  TestEvalBase: TestEvalBase#
  TestEval.enabled: TestEval#enabled().
  TestEvalBase.enabled: TestEvalBase#enabled().
  TestEvalBase.get_sample_submission_name: TestEvalBase#get_sample_submission_name().
  MLETestEval: MLETestEval#
  TestEval.env: TestEval#env.
  NoTestEvalError: NoTestEvalError#
  TestEvalBase.is_sub_enabled: TestEvalBase#is_sub_enabled().
  TestEval: TestEval#
  TestEval.__init__: TestEval#__init__().
  MLETestEval.__init__: MLETestEval#__init__().
  MLETestEval.enabled: MLETestEval#enabled().
---
# Module: [`rdagent/scenarios/data_science/test_eval.py`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py)

## Classes
### `MLETestEval`  ·  implements/extends TestEvalBase
- def: [`rdagent/scenarios/data_science/test_eval.py:107`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L107)
- doc: Evaluation for test data for MLE-Bench competition
- signature: `class MLETestEval(TestEvalBase):`
- members:
  - `enabled(self, competition)` — [`L138`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L138)
  - `eval(self, competition: str, workspace: FBWorkspace)` — [`L117`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L117)
  - `valid(self, competition: str, workspace: FBWorkspace)` — [`L126`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L126)
  - `env` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L112)
- protocol/private: `__init__`[`L110`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L110)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../core/experiment.md#FBWorkspace), [`workspace_path`](../../core/experiment.md#FBWorkspace.workspace_path), [`get_ds_env`](../../components/coder/data_science/conf.md#get_ds_env), [`inject_files`](../../core/experiment.md#FBWorkspace.inject_files), [`exit_code`](../../utils/env.md#EnvResult.exit_code), [`stdout`](../../utils/env.md#EnvResult.stdout), [`run`](../../core/experiment.md#FBWorkspace.run), [`execute`](../../core/experiment.md#FBWorkspace.execute), [`local_data_path`](../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`prepare`](../../utils/env.md#Env.prepare)  (1 test-only)
- used by: [`summarize_folder`](../../log/mle_summary.md#summarize_folder)  (5 test-only)

### `NoTestEvalError`  ·  implements/extends Exception
- def: [`rdagent/scenarios/data_science/test_eval.py:9`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L9)
- doc: Test evaluation is not provided
- signature: `class NoTestEvalError(Exception):`
- used by: [`save_all_grade_info`](../../log/mle_summary.md#save_all_grade_info)  (2 test-only)

### `TestEval`  ·  implements/extends TestEvalBase
- def: [`rdagent/scenarios/data_science/test_eval.py:62`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L62)
- doc: The most basic version of evaluation for test data
- signature: `class TestEval(TestEvalBase):`
- members:
  - `enabled(self, competition)` — [`L101`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L101)
  - `eval(self, competition: str, workspace: FBWorkspace)` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L69)
  - `valid(self, competition: str, workspace: FBWorkspace)` — [`L84`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L84)
  - `env` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L67)
- protocol/private: `__init__`[`L65`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L65)
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../core/experiment.md#FBWorkspace), [`workspace_path`](../../core/experiment.md#FBWorkspace.workspace_path), [`get_ds_env`](../../components/coder/data_science/conf.md#get_ds_env), [`inject_files`](../../core/experiment.md#FBWorkspace.inject_files), [`exit_code`](../../utils/env.md#EnvResult.exit_code), [`stdout`](../../utils/env.md#EnvResult.stdout), [`run`](../../core/experiment.md#FBWorkspace.run), [`execute`](../../core/experiment.md#FBWorkspace.execute), [`local_data_path`](../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path), [`DEL_KEY`](../../core/experiment.md#FBWorkspace.DEL_KEY), [`eval_sub_dir`](../../app/data_science/conf.md#DataScienceBasePropSetting.eval_sub_dir)  (2 test-only)
- used by: (5 test-only callers)

### `TestEvalBase`
- def: [`rdagent/scenarios/data_science/test_eval.py:13`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L13)
- doc: Evaluate a workspace on Test Dataset
- signature: `class TestEvalBase:`
- members:
  - `enabled(self, competition)` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L25) — support `eval` & `valid` or not
  - `eval(self, competition: str, workspace: FBWorkspace)` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L17) — eval the workspace as competition, and return the final evaluation result
  - `get_sample_submission_name(self, competition: str)` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L29) — Get the sample submission file name for the given competition.
  - `is_sub_enabled(self, competition: str)` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L47) — Is submission file enabled
  - `valid(self, competition: str, workspace: FBWorkspace)` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L21) — eval the workspace as competition, and return the final format check result
- uses (calls/refs, reference-scoped): [`DS_RD_SETTING`](../../app/data_science/conf.md#DS_RD_SETTING), [`FBWorkspace`](../../core/experiment.md#FBWorkspace), [`local_data_path`](../../app/kaggle/conf.md#KaggleBasePropSetting.local_data_path)  (8 test-only)
- used by: [`evaluate`](dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../../components/coder/data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`save_grade_info`](../../log/mle_summary.md#save_grade_info)  (3 test-only)

## Functions
- `get_test_eval()` — [`L142`](../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/test_eval.py#L142) — Get the test evaluation instance

