---
title: 'Module: tests/test_runner.py'
type: catalog
provenance: extracted
module: tests/test_runner.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `tests.test_runner`/
symbols:
  make_frame: make_frame().
  reply: reply().
  plan_text: plan_text().
  FakeAgent.calls: FakeAgent#calls.
  FakeEnv: FakeEnv#
  test_resume_replays_the_log_and_continues_with_a_fresh_session: test_resume_replays_the_log_and_continues_with_a_fresh_session().
  make_runner: make_runner().
  FakeAgent: FakeAgent#
  test_expectation_mismatch_truncates_the_queue_and_reinvokes_with_the_diff: test_expectation_mismatch_truncates_the_queue_and_reinvokes_with_the_diff().
  InvokeCall.prompt: InvokeCall#prompt.
  test_queue_drains_with_zero_model_calls_and_win_stops: test_queue_drains_with_zero_model_calls_and_win_stops().
  test_mid_drain_unavailable_action_truncates_queue_and_reinvokes: test_mid_drain_unavailable_action_truncates_queue_and_reinvokes().
  test_level_change_interrupts_the_queue: test_level_change_interrupts_the_queue().
  test_state_change_interrupts_the_queue: test_state_change_interrupts_the_queue().
  test_game_over_reset_counts_toward_action_cap: test_game_over_reset_counts_toward_action_cap().
  test_fresh_session_threshold_drops_the_transcript_and_points_at_the_log: test_fresh_session_threshold_drops_the_transcript_and_points_at_the_log().
  test_expect_levels_mismatch_at_plan_end_reinvokes_with_the_note: test_expect_levels_mismatch_at_plan_end_reinvokes_with_the_note().
  test_parse_retry_limit_stops_the_run: test_parse_retry_limit_stops_the_run().
  test_plan_is_clamped_to_the_remaining_action_budget: test_plan_is_clamped_to_the_remaining_action_budget().
  test_resume_state_round_trips_across_invocations: test_resume_state_round_trips_across_invocations().
  test_large_cumulative_input_with_small_context_stays_in_the_conversation: test_large_cumulative_input_with_small_context_stays_in_the_conversation().
  test_transient_provider_error_is_retried_once: test_transient_provider_error_is_retried_once().
  test_two_self_resets_escalate_the_next_prompt: test_two_self_resets_escalate_the_next_prompt().
  test_game_over_resets_do_not_count_toward_escalation: test_game_over_resets_do_not_count_toward_escalation().
  test_level_completion_stands_down_escalation: test_level_completion_stands_down_escalation().
  test_action_threshold_escalates_then_tier_two: test_action_threshold_escalates_then_tier_two().
  test_deeply_stuck_level_enters_escalation_at_tier_two: test_deeply_stuck_level_enters_escalation_at_tier_two().
  test_runner_logs_settled_board_diff_for_live_actions: test_runner_logs_settled_board_diff_for_live_actions().
  test_runner_omits_diff_for_agent_planned_reset: test_runner_omits_diff_for_agent_planned_reset().
  test_cost_cap_stops_before_the_next_invocation: test_cost_cap_stops_before_the_next_invocation().
  test_matching_expectations_do_not_interrupt_the_drain: test_matching_expectations_do_not_interrupt_the_drain().
  test_resume_from_a_game_over_tail_issues_the_reset: test_resume_from_a_game_over_tail_issues_the_reset().
  test_runner_logs_no_op_diff_when_action_changes_no_cells: test_runner_logs_no_op_diff_when_action_changes_no_cells().
  test_budget_clamped_plans_skip_the_expect_levels_check: test_budget_clamped_plans_skip_the_expect_levels_check().
  test_env_error_is_terminal: test_env_error_is_terminal().
  test_resume_tolerates_cosmetic_intermediate_frame_differences: test_resume_tolerates_cosmetic_intermediate_frame_differences().
  FakeEnv.steps: FakeEnv#steps.
  test_persistent_provider_error_still_writes_metrics: test_persistent_provider_error_still_writes_metrics().
  test_seed_level_signals_recovers_current_level_thrash: test_seed_level_signals_recovers_current_level_thrash().
  FakeEnv.step: FakeEnv#step().
  FakeAgent.invoke: FakeAgent#invoke().
  test_resume_aborts_when_the_replay_diverges_from_the_log: test_resume_aborts_when_the_replay_diverges_from_the_log().
  test_run_game_copies_workspace_template_files: test_run_game_copies_workspace_template_files().
  test_seed_level_signals_recovers_current_level_thrash.rec: test_seed_level_signals_recovers_current_level_thrash().rec().
  FailingAgent.invoke: FailingAgent#invoke().
  StepCall.action: StepCall#action.
  FakeEnv.reset: FakeEnv#reset().
  InvokeCall.resume_from: InvokeCall#resume_from.
  FakeEnv.reset_frames: FakeEnv#reset_frames.
  FakeEnv.step_frames: FakeEnv#step_frames.
  expect_plan: expect_plan().
  write_resume_artifacts: write_resume_artifacts().
  with_cell: with_cell().
  FakeEnv.resets: FakeEnv#resets.
  FakeAgent.replies: FakeAgent#replies.
  test_available_actions_validation_uses_the_current_frame: test_available_actions_validation_uses_the_current_frame().
  StepCall: StepCall#
  InvokeCall: InvokeCall#
  FakeAgent.cycle: FakeAgent#cycle.
  FailingAgent: FailingAgent#
  FailingAgent.failures: FailingAgent#failures.
  FailingAgent.calls: FailingAgent#calls.
  _no_sleep: _no_sleep().
  FakeEnv.cycle: FakeEnv#cycle.
  FailingAgent.then: FailingAgent#then.
  test_run_game_copies_workspace_template_files.DummyClient: test_run_game_copies_workspace_template_files().DummyClient#
  test_run_game_copies_workspace_template_files.FakeArcade: test_run_game_copies_workspace_template_files().FakeArcade#
  StepCall.data: StepCall#data.
  FakeEnv.__init__: FakeEnv#__init__().
  FailingAgent.__init__: FailingAgent#__init__().
  test_run_game_copies_workspace_template_files.DummyClient.__init__: test_run_game_copies_workspace_template_files().DummyClient#__init__().
  DummyClient.workspace: DummyClient#workspace.
  test_run_game_copies_workspace_template_files.DummyClient.aclose: test_run_game_copies_workspace_template_files().DummyClient#aclose().
  test_run_game_copies_workspace_template_files.FakeArcade.get_scorecard: test_run_game_copies_workspace_template_files().FakeArcade#get_scorecard().
---
# Module: [`tests/test_runner.py`](../../../../../raw/code/Retrodict/tests/test_runner.py)

## Classes
### `DummyClient`
- def: [`tests/test_runner.py:528`](../../../../../raw/code/Retrodict/tests/test_runner.py#L528)
- signature: `class DummyClient:`
- members:
  - `aclose(self)` — [`L532`](../../../../../raw/code/Retrodict/tests/test_runner.py#L532)
  - `workspace` — [`L530`](../../../../../raw/code/Retrodict/tests/test_runner.py#L530)
- protocol/private: `__init__`[`L529`](../../../../../raw/code/Retrodict/tests/test_runner.py#L529)
- used by: (1 test-only callers)

### `FailingAgent`
- def: [`tests/test_runner.py:368`](../../../../../raw/code/Retrodict/tests/test_runner.py#L368)
- signature: `class FailingAgent:`
- members:
  - `invoke(self, prompt: str, resume_from: dict[str, Any] | None)` — [`L374`](../../../../../raw/code/Retrodict/tests/test_runner.py#L374)
  - `calls` — [`L372`](../../../../../raw/code/Retrodict/tests/test_runner.py#L372)
  - `failures` — [`L370`](../../../../../raw/code/Retrodict/tests/test_runner.py#L370)
  - `then` — [`L371`](../../../../../raw/code/Retrodict/tests/test_runner.py#L371)
- protocol/private: `__init__`[`L369`](../../../../../raw/code/Retrodict/tests/test_runner.py#L369)
- used by: (2 test-only callers)

### `FakeAgent`
- def: [`tests/test_runner.py:72`](../../../../../raw/code/Retrodict/tests/test_runner.py#L72)
- signature: `class FakeAgent:`
- members:
  - `invoke(self, prompt: str, resume_from: dict[str, Any] | None)` — [`L77`](../../../../../raw/code/Retrodict/tests/test_runner.py#L77)
  - `calls` — [`L75`](../../../../../raw/code/Retrodict/tests/test_runner.py#L75)
  - `cycle` — [`L74`](../../../../../raw/code/Retrodict/tests/test_runner.py#L74)
  - `replies` — [`L73`](../../../../../raw/code/Retrodict/tests/test_runner.py#L73)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (29 test-only callers)

### `FakeArcade`
- def: [`tests/test_runner.py:536`](../../../../../raw/code/Retrodict/tests/test_runner.py#L536)
- signature: `class FakeArcade:`
- members:
  - `get_scorecard(self)` — [`L537`](../../../../../raw/code/Retrodict/tests/test_runner.py#L537)
- used by: (1 test-only callers)

### `FakeEnv`
- def: [`tests/test_runner.py:42`](../../../../../raw/code/Retrodict/tests/test_runner.py#L42)
- signature: `class FakeEnv:`
- members:
  - `reset(self)` — [`L50`](../../../../../raw/code/Retrodict/tests/test_runner.py#L50)
  - `step(self, action, data=None, reasoning=None)` — [`L56`](../../../../../raw/code/Retrodict/tests/test_runner.py#L56)
  - `cycle` — [`L46`](../../../../../raw/code/Retrodict/tests/test_runner.py#L46)
  - `reset_frames` — [`L44`](../../../../../raw/code/Retrodict/tests/test_runner.py#L44)
  - `resets` — [`L47`](../../../../../raw/code/Retrodict/tests/test_runner.py#L47)
  - `step_frames` — [`L45`](../../../../../raw/code/Retrodict/tests/test_runner.py#L45)
  - `steps` — [`L48`](../../../../../raw/code/Retrodict/tests/test_runner.py#L48)
- protocol/private: `__init__`[`L43`](../../../../../raw/code/Retrodict/tests/test_runner.py#L43)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (33 test-only callers)

### `InvokeCall`
- def: [`tests/test_runner.py:66`](../../../../../raw/code/Retrodict/tests/test_runner.py#L66)
- signature: `class InvokeCall:`
- members:
  - `prompt` — [`L67`](../../../../../raw/code/Retrodict/tests/test_runner.py#L67)
  - `resume_from` — [`L68`](../../../../../raw/code/Retrodict/tests/test_runner.py#L68)
- used by: (19 test-only callers)

### `StepCall`
- def: [`tests/test_runner.py:37`](../../../../../raw/code/Retrodict/tests/test_runner.py#L37)
- signature: `class StepCall:`
- members:
  - `action` — [`L38`](../../../../../raw/code/Retrodict/tests/test_runner.py#L38)
  - `data` — [`L39`](../../../../../raw/code/Retrodict/tests/test_runner.py#L39)
- used by: (9 test-only callers)

## Functions
- `_no_sleep(_seconds: float)` — [`L412`](../../../../../raw/code/Retrodict/tests/test_runner.py#L412)
- `expect_plan(json_plan: str)` — [`L301`](../../../../../raw/code/Retrodict/tests/test_runner.py#L301)
- `make_frame(state: GameState = GameState.NOT_FINISHED, levels: int = 0, win: int = 7, available: tuple[int, ...] = (1, 2, 3, 4, 5, 6), boards: int = 1)` — [`L19`](../../../../../raw/code/Retrodict/tests/test_runner.py#L19)
- `make_runner(tmp_path: Path, env: FakeEnv, agent: AgentClient, **cfg_kwargs: Any)` — [`L109`](../../../../../raw/code/Retrodict/tests/test_runner.py#L109)
- `plan_text(*actions: str, reasoning: str = "test")` — [`L84`](../../../../../raw/code/Retrodict/tests/test_runner.py#L84)
- `rec(step: int, action: str, levels: int, state: str = "NOT_FINISHED")` — [`L620`](../../../../../raw/code/Retrodict/tests/test_runner.py#L620)
- `reply(text: str, resume: dict[str, Any] | None = None, input_tokens: int = 100, **kwargs: Any)` — [`L95`](../../../../../raw/code/Retrodict/tests/test_runner.py#L95)
- `test_action_threshold_escalates_then_tier_two(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L596`](../../../../../raw/code/Retrodict/tests/test_runner.py#L596) — Disciplined-but-endless play on one level escalates by action count, then hardens to tier 2.
- `test_available_actions_validation_uses_the_current_frame()` — [`L551`](../../../../../raw/code/Retrodict/tests/test_runner.py#L551) — The parser rejects actions the env is not offering right now.
- `test_budget_clamped_plans_skip_the_expect_levels_check(tmp_path: Path)` — [`L346`](../../../../../raw/code/Retrodict/tests/test_runner.py#L346)
- `test_cost_cap_stops_before_the_next_invocation(tmp_path: Path)` — [`L251`](../../../../../raw/code/Retrodict/tests/test_runner.py#L251)
- `test_deeply_stuck_level_enters_escalation_at_tier_two(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L642`](../../../../../raw/code/Retrodict/tests/test_runner.py#L642) — A level already past double the action threshold (e.g. via resume) skips straight to tier 2.
- `test_env_error_is_terminal(tmp_path: Path)` — [`L358`](../../../../../raw/code/Retrodict/tests/test_runner.py#L358)
- `test_expect_levels_mismatch_at_plan_end_reinvokes_with_the_note(tmp_path: Path)` — [`L333`](../../../../../raw/code/Retrodict/tests/test_runner.py#L333)
- `test_expectation_mismatch_truncates_the_queue_and_reinvokes_with_the_diff(tmp_path: Path)` — [`L318`](../../../../../raw/code/Retrodict/tests/test_runner.py#L318)
- `test_fresh_session_threshold_drops_the_transcript_and_points_at_the_log(tmp_path: Path)` — [`L274`](../../../../../raw/code/Retrodict/tests/test_runner.py#L274)
- `test_game_over_reset_counts_toward_action_cap(tmp_path: Path)` — [`L226`](../../../../../raw/code/Retrodict/tests/test_runner.py#L226) — Every death costs the step plus the RESET, so the cap ends the loop.
- `test_game_over_resets_do_not_count_toward_escalation(tmp_path: Path)` — [`L568`](../../../../../raw/code/Retrodict/tests/test_runner.py#L568) — Engine-forced restarts are failure feedback, not thrash; only self-issued RESETs count.
- `test_large_cumulative_input_with_small_context_stays_in_the_conversation(tmp_path: Path)` — [`L288`](../../../../../raw/code/Retrodict/tests/test_runner.py#L288) — Tool rounds re-count the cached prefix; only real context growth forces a fresh session.
- `test_level_change_interrupts_the_queue(tmp_path: Path)` — [`L187`](../../../../../raw/code/Retrodict/tests/test_runner.py#L187)
- `test_level_completion_stands_down_escalation(tmp_path: Path)` — [`L581`](../../../../../raw/code/Retrodict/tests/test_runner.py#L581)
- `test_matching_expectations_do_not_interrupt_the_drain(tmp_path: Path)` — [`L305`](../../../../../raw/code/Retrodict/tests/test_runner.py#L305)
- `test_mid_drain_unavailable_action_truncates_queue_and_reinvokes(tmp_path: Path)` — [`L175`](../../../../../raw/code/Retrodict/tests/test_runner.py#L175)
- `test_parse_retry_limit_stops_the_run(tmp_path: Path)` — [`L211`](../../../../../raw/code/Retrodict/tests/test_runner.py#L211)
- `test_persistent_provider_error_still_writes_metrics(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L398`](../../../../../raw/code/Retrodict/tests/test_runner.py#L398)
- `test_plan_is_clamped_to_the_remaining_action_budget(tmp_path: Path)` — [`L240`](../../../../../raw/code/Retrodict/tests/test_runner.py#L240)
- `test_queue_drains_with_zero_model_calls_and_win_stops(tmp_path: Path)` — [`L115`](../../../../../raw/code/Retrodict/tests/test_runner.py#L115)
- `test_resume_aborts_when_the_replay_diverges_from_the_log(tmp_path: Path)` — [`L474`](../../../../../raw/code/Retrodict/tests/test_runner.py#L474)
- `test_resume_from_a_game_over_tail_issues_the_reset(tmp_path: Path)` — [`L510`](../../../../../raw/code/Retrodict/tests/test_runner.py#L510)
- `test_resume_replays_the_log_and_continues_with_a_fresh_session(tmp_path: Path)` — [`L446`](../../../../../raw/code/Retrodict/tests/test_runner.py#L446)
- `test_resume_state_round_trips_across_invocations(tmp_path: Path)` — [`L263`](../../../../../raw/code/Retrodict/tests/test_runner.py#L263)
- `test_resume_tolerates_cosmetic_intermediate_frame_differences(tmp_path: Path)` — [`L486`](../../../../../raw/code/Retrodict/tests/test_runner.py#L486) — A resume must not abort when only throwaway animation frames differ (settled board matches).
- `test_run_game_copies_workspace_template_files(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L525`](../../../../../raw/code/Retrodict/tests/test_runner.py#L525)
- `test_runner_logs_no_op_diff_when_action_changes_no_cells(tmp_path: Path)` — [`L151`](../../../../../raw/code/Retrodict/tests/test_runner.py#L151)
- `test_runner_logs_settled_board_diff_for_live_actions(tmp_path: Path)` — [`L138`](../../../../../raw/code/Retrodict/tests/test_runner.py#L138)
- `test_runner_omits_diff_for_agent_planned_reset(tmp_path: Path)` — [`L162`](../../../../../raw/code/Retrodict/tests/test_runner.py#L162)
- `test_seed_level_signals_recovers_current_level_thrash(tmp_path: Path)` — [`L616`](../../../../../raw/code/Retrodict/tests/test_runner.py#L616) — Resume must rebuild the stuck signals for the level in progress from the log alone.
- `test_state_change_interrupts_the_queue(tmp_path: Path)` — [`L199`](../../../../../raw/code/Retrodict/tests/test_runner.py#L199)
- `test_transient_provider_error_is_retried_once(tmp_path: Path, monkeypatch: pytest.MonkeyPatch)` — [`L384`](../../../../../raw/code/Retrodict/tests/test_runner.py#L384)
- `test_two_self_resets_escalate_the_next_prompt(tmp_path: Path)` — [`L557`](../../../../../raw/code/Retrodict/tests/test_runner.py#L557) — Voluntary reset-thrash on one level must trigger the binding stuck directive.
- `with_cell(frame: FrameDataRaw, x: int, y: int, color: int)` — [`L31`](../../../../../raw/code/Retrodict/tests/test_runner.py#L31)
- `write_resume_artifacts(run_dir: Path, frames: list, prior_metrics: dict[str, Any] | None = None)` — [`L416`](../../../../../raw/code/Retrodict/tests/test_runner.py#L416) — Write a log (RESET + ACTION1 steps from the given frames) and optional prior metrics.

