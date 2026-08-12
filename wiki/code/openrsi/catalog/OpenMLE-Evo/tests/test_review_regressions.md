---
title: 'Module: OpenMLE-Evo/tests/test_review_regressions.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tests/test_review_regressions.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tests.test_review_regressions`/
symbols:
  test_sandbox_poll_returns_persistent_client_error_immediately: test_sandbox_poll_returns_persistent_client_error_immediately().
  test_load_leaderboard_supports_release_layouts_and_missing_data: test_load_leaderboard_supports_release_layouts_and_missing_data().
  test_summary_skips_corrupt_task_stat_and_continues: test_summary_skips_corrupt_task_stat_and_continues().
  test_linear_sign_preserves_valid_zero_score: test_linear_sign_preserves_valid_zero_score().
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeResponse.json: test_sandbox_poll_returns_persistent_client_error_immediately().FakeResponse#json().
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeClient.post: test_sandbox_poll_returns_persistent_client_error_immediately().FakeClient#post().
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeClient.get: test_sandbox_poll_returns_persistent_client_error_immediately().FakeClient#get().
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeResponse: test_sandbox_poll_returns_persistent_client_error_immediately().FakeResponse#
  FakeResponse._payload: FakeResponse#_payload.
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeClient: test_sandbox_poll_returns_persistent_client_error_immediately().FakeClient#
  test_sandbox_poll_returns_persistent_client_error_immediately.no_sleep: test_sandbox_poll_returns_persistent_client_error_immediately().no_sleep().
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeResponse.__init__: test_sandbox_poll_returns_persistent_client_error_immediately().FakeResponse#__init__().
  FakeResponse.status_code: FakeResponse#status_code.
  FakeResponse.headers: FakeResponse#headers.
  test_sandbox_poll_returns_persistent_client_error_immediately.FakeClient.base_url: test_sandbox_poll_returns_persistent_client_error_immediately().FakeClient#base_url.
  test_corrupt_completed_task_stat_is_not_treated_as_resumable: test_corrupt_completed_task_stat_is_not_treated_as_resumable().
  test_final_submit_is_not_executed_from_a_finally_block: test_final_submit_is_not_executed_from_a_finally_block().
---
# Module: [`OpenMLE-Evo/tests/test_review_regressions.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py)

## Classes
### `FakeClient`
- def: [`OpenMLE-Evo/tests/test_review_regressions.py:83`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L83)
- signature: `class FakeClient:`
- members:
  - `get(self, *args, **kwargs)` — [`L89`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L89)
  - `post(self, *args, **kwargs)` — [`L86`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L86)
  - `base_url` — [`L84`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L84)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `FakeResponse`
- def: [`OpenMLE-Evo/tests/test_review_regressions.py:74`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L74)
- signature: `class FakeResponse:`
- members:
  - `json(self)` — [`L80`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L80)
  - `headers` — [`L78`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L78)
  - `status_code` — [`L76`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L76)
- protocol/private: `__init__`[`L75`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L75), `_payload`[`L77`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L77)
- used by: (2 test-only callers)

## Functions
- `no_sleep(delay)` — [`L92`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L92)
- `test_corrupt_completed_task_stat_is_not_treated_as_resumable(tmp_path)` — [`L112`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L112)
- `test_final_submit_is_not_executed_from_a_finally_block()` — [`L135`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L135)
- `test_linear_sign_preserves_valid_zero_score()` — [`L63`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L63)
- `test_load_leaderboard_supports_release_layouts_and_missing_data(tmp_path)` — [`L14`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L14)
- `test_sandbox_poll_returns_persistent_client_error_immediately(monkeypatch)` — [`L73`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L73)
- `test_summary_skips_corrupt_task_stat_and_continues(tmp_path, caplog)` — [`L42`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_review_regressions.py#L42) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)

