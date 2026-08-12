---
title: 'Module: rlm/utils/exceptions.py'
type: catalog
provenance: extracted
module: rlm/utils/exceptions.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.utils.exceptions`/
symbols:
  BudgetExceededError: BudgetExceededError#
  TimeoutExceededError: TimeoutExceededError#
  TokenLimitExceededError: TokenLimitExceededError#
  ErrorThresholdExceededError: ErrorThresholdExceededError#
  CancellationError: CancellationError#
  BudgetExceededError.spent: BudgetExceededError#spent.
  BudgetExceededError.budget: BudgetExceededError#budget.
  TimeoutExceededError.elapsed: TimeoutExceededError#elapsed.
  TimeoutExceededError.timeout: TimeoutExceededError#timeout.
  TokenLimitExceededError.tokens_used: TokenLimitExceededError#tokens_used.
  TokenLimitExceededError.token_limit: TokenLimitExceededError#token_limit.
  ErrorThresholdExceededError.error_count: ErrorThresholdExceededError#error_count.
  ErrorThresholdExceededError.threshold: ErrorThresholdExceededError#threshold.
  BudgetExceededError.__init__: BudgetExceededError#__init__().
  TimeoutExceededError.__init__: TimeoutExceededError#__init__().
  TimeoutExceededError.partial_answer: TimeoutExceededError#partial_answer.
  TokenLimitExceededError.__init__: TokenLimitExceededError#__init__().
  TokenLimitExceededError.partial_answer: TokenLimitExceededError#partial_answer.
  ErrorThresholdExceededError.__init__: ErrorThresholdExceededError#__init__().
  ErrorThresholdExceededError.last_error: ErrorThresholdExceededError#last_error.
  ErrorThresholdExceededError.partial_answer: ErrorThresholdExceededError#partial_answer.
  CancellationError.__init__: CancellationError#__init__().
  CancellationError.partial_answer: CancellationError#partial_answer.
---
# Module: [`rlm/utils/exceptions.py`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py)

## Classes
### `BudgetExceededError`  ·  implements/extends Exception
- def: [`rlm/utils/exceptions.py:4`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L4)
- doc: Raised when the RLM execution exceeds the maximum budget.
- signature: `class BudgetExceededError(Exception):`
- members:
  - `budget` — [`L9`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L9)
  - `spent` — [`L8`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L8)
- protocol/private: `__init__`[`L7`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L7)
- used by: [`_subcall`](../core/rlm.md#RLM._subcall), [`_check_iteration_limits`](../core/rlm.md#RLM._check_iteration_limits)  (1 test-only)

### `CancellationError`  ·  implements/extends Exception
- def: [`rlm/utils/exceptions.py:68`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L68)
- doc: Raised when the RLM execution is cancelled by the user.
- signature: `class CancellationError(Exception):`
- members:
  - `partial_answer` — [`L72`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L72)
- protocol/private: `__init__`[`L71`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L71)
- used by: [`completion`](../core/rlm.md#RLM.completion)

### `ErrorThresholdExceededError`  ·  implements/extends Exception
- def: [`rlm/utils/exceptions.py:47`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L47)
- doc: Raised when the RLM encounters too many consecutive errors.
- signature: `class ErrorThresholdExceededError(Exception):`
- members:
  - `error_count` — [`L58`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L58)
  - `last_error` — [`L60`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L60)
  - `partial_answer` — [`L61`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L61)
  - `threshold` — [`L59`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L59)
- protocol/private: `__init__`[`L50`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L50)
- used by: [`_check_iteration_limits`](../core/rlm.md#RLM._check_iteration_limits)  (1 test-only)

### `TimeoutExceededError`  ·  implements/extends Exception
- def: [`rlm/utils/exceptions.py:13`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L13)
- doc: Raised when the RLM execution exceeds the maximum timeout.
- signature: `class TimeoutExceededError(Exception):`
- members:
  - `elapsed` — [`L23`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L23)
  - `partial_answer` — [`L25`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L25)
  - `timeout` — [`L24`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L24)
- protocol/private: `__init__`[`L16`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L16)
- used by: [`_check_timeout`](../core/rlm.md#RLM._check_timeout)  (1 test-only)

### `TokenLimitExceededError`  ·  implements/extends Exception
- def: [`rlm/utils/exceptions.py:29`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L29)
- doc: Raised when the RLM execution exceeds the maximum token limit.
- signature: `class TokenLimitExceededError(Exception):`
- members:
  - `partial_answer` — [`L41`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L41)
  - `token_limit` — [`L40`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L40)
  - `tokens_used` — [`L39`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L39)
- protocol/private: `__init__`[`L32`](../../../../../../raw/code/rlm/rlm/utils/exceptions.py#L32)
- used by: [`_check_iteration_limits`](../core/rlm.md#RLM._check_iteration_limits)  (1 test-only)

