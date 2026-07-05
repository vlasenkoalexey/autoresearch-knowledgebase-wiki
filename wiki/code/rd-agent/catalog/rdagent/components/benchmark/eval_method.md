---
title: 'Module: rdagent/components/benchmark/eval_method.py'
type: catalog
provenance: extracted
module: rdagent/components/benchmark/eval_method.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.benchmark.eval_method`/
symbols:
  FactorImplementEval.__init__: FactorImplementEval#__init__().
  FactorImplementEval.eval: FactorImplementEval#eval().
  BaseEval.eval_case: BaseEval#eval_case().
  FactorImplementEval.develop: FactorImplementEval#develop().
  BaseEval.load_cases_to_eval: BaseEval#load_cases_to_eval().
  TestCases.get_exp: TestCases#get_exp().
  BaseEval.__init__: BaseEval#__init__().
  TestCases.ground_truth: TestCases#ground_truth().
  FactorImplementEval: FactorImplementEval#
  EVAL_RES: EVAL_RES.
  TestCases.test_case_l: TestCases#test_case_l.
  TestCase.__init__: TestCase#__init__().
  TestCases: TestCases#
  TestCases.target_task: TestCases#target_task().
  BaseEval.test_cases: BaseEval#test_cases.
  BaseEval: BaseEval#
  FactorImplementEval.summarize_res: FactorImplementEval#summarize_res().
  TestCase: TestCase#
  TestCases.__init__: TestCases#__init__().
  TestCases.__getitem__: TestCases#__getitem__().
  TestCases.__len__: TestCases#__len__().
  TestCase.target_task: TestCase#target_task.
  FactorImplementEval.test_round: FactorImplementEval#test_round.
  TestCase.ground_truth: TestCase#ground_truth.
  BaseEval.evaluator_l: BaseEval#evaluator_l.
  BaseEval.generate_method: BaseEval#generate_method.
  BaseEval.catch_eval_except: BaseEval#catch_eval_except.
---
# Module: [`rdagent/components/benchmark/eval_method.py`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py)

## Classes
### `BaseEval`
- def: [`rdagent/components/benchmark/eval_method.py:64`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L64)
- doc: The benchmark benchmark evaluation.
- signature: `class BaseEval:`
- members:
  - `__init__(self, evaluator_l: List[FactorEvaluator], test_cases: TestCases, generate_method: Developer, catch_eval_except: bool = True)` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L69) — Parameters
  - `eval_case(self, case_gt: Workspace, case_gen: Workspace)` — [`L105`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L105) — Parameters
  - `load_cases_to_eval(self, path: Union[Path, str], **kwargs)` — [`L90`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L90)
  - `catch_eval_except` — [`L88`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L88)
  - `evaluator_l` — [`L85`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L85)
  - `generate_method` — [`L87`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L87)
  - `test_cases` — [`L86`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L86)
- uses (calls/refs, reference-scoped): [`Workspace`](../../core/experiment.md#Workspace), [`CoderError`](../../core/exception.md#CoderError), [`Developer`](../../core/developer.md#Developer), [`FactorEvaluator`](../coder/factor_coder/eva_utils.md#FactorEvaluator), [`evaluate`](../coder/factor_coder/eva_utils.md#FactorEvaluator.evaluate), [`FactorFBWorkspace`](../coder/factor_coder/factor.md#FactorFBWorkspace), [`from_folder`](../coder/factor_coder/factor.md#FactorFBWorkspace.from_folder)  (2 test-only)
- used by: (4 test-only callers)

### `FactorImplementEval`  ·  implements/extends BaseEval
- def: [`rdagent/components/benchmark/eval_method.py:140`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L140)
- signature: `class FactorImplementEval(BaseEval):`
- members:
  - `develop(self)` — [`L160`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L160)
  - `eval(self, gen_factor_l_all_rounds)` — [`L181`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L181)
  - `summarize_res(res: EVAL_RES)` — [`L200`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L200)
  - `test_round` — [`L158`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L158)
- protocol/private: `__init__`[`L141`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L141)
- uses (calls/refs, reference-scoped): [`Scenario`](../../core/scenario.md#Scenario), [`RD_AGENT_SETTINGS`](../../core/conf.md#RD_AGENT_SETTINGS), [`Developer`](../../core/developer.md#Developer), [`develop`](../../core/developer.md#Developer.develop), [`multiprocessing_wrapper`](../../core/utils.md#multiprocessing_wrapper), [`multi_proc_n`](../../core/conf.md#RDAgentSettings.multi_proc_n), [`FactorCorrelationEvaluator`](../coder/factor_coder/eva_utils.md#FactorCorrelationEvaluator), [`FactorEqualValueRatioEvaluator`](../coder/factor_coder/eva_utils.md#FactorEqualValueRatioEvaluator), [`FactorIndexEvaluator`](../coder/factor_coder/eva_utils.md#FactorIndexEvaluator), [`FactorRowCountEvaluator`](../coder/factor_coder/eva_utils.md#FactorRowCountEvaluator), [`FactorSingleColumnEvaluator`](../coder/factor_coder/eva_utils.md#FactorSingleColumnEvaluator)  (9 test-only)
- used by: (4 test-only callers)

### `TestCase`
- def: [`rdagent/components/benchmark/eval_method.py:31`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L31)
- signature: `class TestCase:`
- members:
  - `ground_truth` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L38)
  - `target_task` — [`L37`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L37)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L32)
- uses (calls/refs, reference-scoped): [`Task`](../../core/experiment.md#Task), [`Workspace`](../../core/experiment.md#Workspace)
- used by: [`load`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorTestCaseLoaderFromJsonFile.load)  (4 test-only)

### `TestCases`
- def: [`rdagent/components/benchmark/eval_method.py:41`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L41)
- signature: `class TestCases:`
- members:
  - `get_exp(self)` — [`L52`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L52)
  - `ground_truth(self)` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L60)
  - `target_task(self)` — [`L56`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L56)
  - `test_case_l` — [`L44`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L44)
- protocol/private: `__getitem__`[`L46`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L46), `__init__`[`L42`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L42), `__len__`[`L49`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L49)
- uses (calls/refs, reference-scoped): [`Experiment`](../../core/experiment.md#Experiment)  (3 test-only)
- used by: [`load`](../../scenarios/qlib/factor_experiment_loader/json_loader.md#FactorTestCaseLoaderFromJsonFile.load)  (4 test-only)

## Module values
- `EVAL_RES` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/components/benchmark/eval_method.py#L25)

