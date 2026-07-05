---
title: 'Module: rdagent/core/exception.py'
type: catalog
provenance: extracted
module: rdagent/core/exception.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.exception`/
symbols:
  CoderError: CoderError#
  FactorEmptyError: FactorEmptyError.
  ModelEmptyError: ModelEmptyError.
  FormatError: FormatError#
  CustomRuntimeError: CustomRuntimeError#
  WorkflowError: WorkflowError#
  NoOutputError: NoOutputError#
  RunnerError: RunnerError#
  CodeBlockParseError: CodeBlockParseError#
  CodeFormatError: CodeFormatError#
  PolicyError: PolicyError#
  CoderError.caused_by_timeout: CoderError#caused_by_timeout.
  KaggleError: KaggleError#
  EvaluatorDidNotTerminateError: EvaluatorDidNotTerminateError#
  CodeBlockParseError.__init__: CodeBlockParseError#__init__().
  CodeBlockParseError.message: CodeBlockParseError#message.
  CodeBlockParseError.content: CodeBlockParseError#content.
  CodeBlockParseError.language: CodeBlockParseError#language.
---
# Module: [`rdagent/core/exception.py`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py)

## Classes
### `CodeBlockParseError`  ·  implements/extends FormatError
- def: [`rdagent/core/exception.py:13`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L13)
- doc: Raised when code block extraction fails after all strategies.
- signature: `class CodeBlockParseError(FormatError):`
- members:
  - `content` — [`L18`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L18)
  - `language` — [`L19`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L19)
  - `message` — [`L17`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L17)
- protocol/private: `__init__`[`L16`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L16)
- uses (calls/refs, reference-scoped): [`FormatError`](exception.md#FormatError)
- used by: [`parse`](../oai/backend/base.md#CodeBlockParser.parse), [`FormatError`](exception.md#FormatError)

### `CodeFormatError`  ·  implements/extends CoderError
- def: [`rdagent/core/exception.py:36`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L36)
- doc: The generated code is not found due format error.
- signature: `class CodeFormatError(CoderError):`
- uses (calls/refs, reference-scoped): [`CoderError`](exception.md#CoderError)
- used by: [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`CoderError`](exception.md#CoderError)

### `CoderError`  ·  implements/extends WorkflowError
- def: [`rdagent/core/exception.py:23`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L23) — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- doc: Exceptions raised when Implementing and running code.
- signature: `class CoderError(WorkflowError):`
- members:
  - `caused_by_timeout` — [`L33`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L33)
- uses (calls/refs, reference-scoped): [`CustomRuntimeError`](exception.md#CustomRuntimeError), [`WorkflowError`](exception.md#WorkflowError), [`NoOutputError`](exception.md#NoOutputError), [`CodeFormatError`](exception.md#CodeFormatError)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`evaluate`](../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`implement_one_task`](../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`develop`](../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`implement_one_task`](../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`develop`](../scenarios/kaggle/developer/runner.md#KGModelRunner.develop), [`_exp_postprocess_by_feedback`](../components/coder/CoSTEER/__init__.md#CoSTEER._exp_postprocess_by_feedback), [`FactorEmptyError`](exception.md#FactorEmptyError), [`ModelEmptyError`](exception.md#ModelEmptyError), [`CustomRuntimeError`](exception.md#CustomRuntimeError), [`skip_loop_error`](../app/kaggle/loop.md#KaggleRDLoop.skip_loop_error), [`WorkflowError`](exception.md#WorkflowError), [`NoOutputError`](exception.md#NoOutputError), [`skip_loop_error`](../app/qlib_rd_loop/factor.md#FactorRDLoop.skip_loop_error), [`skip_loop_error`](../scenarios/data_science/loop.md#DataScienceRDLoop.skip_loop_error), [`CodeFormatError`](exception.md#CodeFormatError), [`skip_loop_error`](../scenarios/finetune/loop.md#LLMFinetuneRDLoop.skip_loop_error), [`skip_loop_error`](../scenarios/rl/loop.md#RLPostTrainingRDLoop.skip_loop_error)  (2 test-only)

### `CustomRuntimeError`  ·  implements/extends CoderError
- def: [`rdagent/core/exception.py:42`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L42)
- doc: The generated code fail to execute the script.
- signature: `class CustomRuntimeError(CoderError):`
- uses (calls/refs, reference-scoped): [`CoderError`](exception.md#CoderError)
- used by: [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`CoderError`](exception.md#CoderError)

### `EvaluatorDidNotTerminateError`  ·  implements/extends RuntimeError
- def: [`rdagent/core/exception.py:79`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L79)
- doc: Evaluator generator did not terminate with a final Feedback.
- signature: `class EvaluatorDidNotTerminateError(RuntimeError):`
- used by: [`_get_overall_feedback`](evolving_agent.md#RAGEvoAgent._get_overall_feedback)

### `FormatError`  ·  implements/extends WorkflowError
- def: [`rdagent/core/exception.py:7`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L7)
- doc: After multiple attempts, we are unable to obtain the answer in the correct format to proceed.
- signature: `class FormatError(WorkflowError):`
- uses (calls/refs, reference-scoped): [`WorkflowError`](exception.md#WorkflowError), [`CodeBlockParseError`](exception.md#CodeBlockParseError)
- used by: [`build_cls_from_json_with_retry`](../utils/agent/workflow.md#build_cls_from_json_with_retry), [`WorkflowError`](exception.md#WorkflowError), [`CodeBlockParseError`](exception.md#CodeBlockParseError)

### `KaggleError`  ·  implements/extends Exception
- def: [`rdagent/core/exception.py:67`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L67)
- doc: Exceptions raised when calling Kaggle API
- signature: `class KaggleError(Exception):`
- used by: [`download_data`](../scenarios/kaggle/kaggle_crawler.md#download_data)

### `NoOutputError`  ·  implements/extends CoderError
- def: [`rdagent/core/exception.py:48`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L48)
- doc: The code fail to generate output file.
- signature: `class NoOutputError(CoderError):`
- uses (calls/refs, reference-scoped): [`CoderError`](exception.md#CoderError)
- used by: [`execute`](../components/coder/factor_coder/factor.md#FactorFBWorkspace.execute), [`CoderError`](exception.md#CoderError)

### `PolicyError`  ·  implements/extends Exception
- def: [`rdagent/core/exception.py:73`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L73)
- doc: Exceptions raised due to content management policy
- signature: `class PolicyError(Exception):`
- used by: [`_try_create_chat_completion_or_embedding`](../oai/backend/base.md#APIBackend._try_create_chat_completion_or_embedding), [`withdraw_loop_error`](../scenarios/data_science/loop.md#DataScienceRDLoop.withdraw_loop_error)

### `RunnerError`  ·  implements/extends Exception
- def: [`rdagent/core/exception.py:54`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L54)
- doc: Exceptions raised when running the code output.
- signature: `class RunnerError(Exception):`
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`develop`](../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.develop), [`skip_loop_error`](../scenarios/data_science/loop.md#DataScienceRDLoop.skip_loop_error)

### `WorkflowError`  ·  implements/extends Exception
- def: [`rdagent/core/exception.py:1`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L1)
- doc: Exception indicating an error that the current loop cannot handle, preventing further progress.
- signature: `class WorkflowError(Exception):`
- uses (calls/refs, reference-scoped): [`CoderError`](exception.md#CoderError), [`FormatError`](exception.md#FormatError)
- used by: [`CoderError`](exception.md#CoderError), [`FormatError`](exception.md#FormatError)

## Module values
- `FactorEmptyError` — [`L62`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L62)
- `ModelEmptyError` — [`L64`](../../../../../../raw/code/rd-agent/rdagent/core/exception.py#L64)

