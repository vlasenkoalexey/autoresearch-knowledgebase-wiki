---
title: 'Module: src/arc3/runner.py'
type: catalog
provenance: extracted
module: src/arc3/runner.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.runner`/
symbols:
  GameRunner._call: GameRunner#_call().
  GameRunner._restore: GameRunner#_restore().
  GameRunner.state: GameRunner#state.
  GameRunner._metrics: GameRunner#_metrics().
  GameRunner._accept: GameRunner#_accept().
  GameRunner._log_frame: GameRunner#_log_frame().
  GameRunner._build_prompt: GameRunner#_build_prompt().
  GameRunner._step: GameRunner#_step().
  GameRunner._drain: GameRunner#_drain().
  ThinAgentClient.invoke: ThinAgentClient#invoke().
  GameRunner.run: GameRunner#run().
  GameRunner._cost: GameRunner#_cost().
  GameRunner._image_prime: GameRunner#_image_prime().
  GameRunner._invoke: GameRunner#_invoke().
  GameRunner._escalation_directive: GameRunner#_escalation_directive().
  run_game: run_game().
  main: main().
  GameRunner._reset_after_game_over: GameRunner#_reset_after_game_over().
  GameRunner.frame: GameRunner#frame.
  GameRunner._loop: GameRunner#_loop().
  ThinAgentClient.__init__: ThinAgentClient#__init__().
  GameRunner._start_fresh: GameRunner#_start_fresh().
  GameRunner._seed_level_signals: GameRunner#_seed_level_signals().
  GameRunner._check_expectations: GameRunner#_check_expectations().
  GameRunner._record_escalation: GameRunner#_record_escalation().
  GameRunner._start_level: GameRunner#_start_level().
  GameRunner.cfg: GameRunner#cfg.
  GameRunner._seed_prior_usage: GameRunner#_seed_prior_usage().
  ModelPricing: ModelPricing#
  RunnerConfig.resolve_pricing: RunnerConfig#resolve_pricing().
  RunState.actions_taken: RunState#actions_taken.
  _render_action: _render_action().
  containment_check: containment_check().
  RunState.escalation_tier: RunState#escalation_tier.
  RunState.level_self_resets: RunState#level_self_resets.
  GameRunner.workspace: GameRunner#workspace.
  GameRunner.__init__: GameRunner#__init__().
  ThinAgentClient.harness: ThinAgentClient#harness.
  RunState.step_no: RunState#step_no.
  GameRunner.log: GameRunner#log.
  GameRunner._available_names: GameRunner#_available_names().
  RunnerConfig.game_id: RunnerConfig#game_id.
  RunnerConfig.model: RunnerConfig#model.
  GameRunner.run_dir: GameRunner#run_dir.
  GameRunner.pricing: GameRunner#pricing.
  RunnerConfig.action_cap: RunnerConfig#action_cap.
  AgentReply: AgentReply#
  RunState.invocations: RunState#invocations.
  RunState.surprise_note: RunState#surprise_note.
  RunState.input_tokens: RunState#input_tokens.
  RunState.cached_tokens: RunState#cached_tokens.
  RunState.invocation_log: RunState#invocation_log.
  GameRunner.env: GameRunner#env.
  ANALYSIS_PYTHON: ANALYSIS_PYTHON.
  WORKSPACE_TEMPLATE: WORKSPACE_TEMPLATE.
  AgentClient.invoke: AgentClient#invoke().
  GameRunner.transcript_path: GameRunner#transcript_path.
  REPO_ROOT: REPO_ROOT.
  RunnerConfig: RunnerConfig#
  RunState.output_tokens: RunState#output_tokens.
  RunState.level_start_actions: RunState#level_start_actions.
  _board_lists: _board_lists().
  ENVIRONMENTS_DIR: ENVIRONMENTS_DIR.
  PRICING: PRICING.
  RunnerConfig.pricing: RunnerConfig#pricing.
  ThinAgentClient.aclose: ThinAgentClient#aclose().
  open_environment: open_environment().
  _ESCALATE_ACTIONS: _ESCALATE_ACTIONS.
  RunnerConfig.reasoning_effort: RunnerConfig#reasoning_effort.
  RunnerConfig.image_prime: RunnerConfig#image_prime.
  RunnerConfig.vision_model: RunnerConfig#vision_model.
  AgentReply.text: AgentReply#text.
  AgentReply.resume_state: AgentReply#resume_state.
  AgentReply.input_tokens: AgentReply#input_tokens.
  AgentReply.cached_tokens: AgentReply#cached_tokens.
  AgentReply.output_tokens: AgentReply#output_tokens.
  AgentReply.model_requests: AgentReply#model_requests.
  AgentReply.truncated: AgentReply#truncated.
  AgentReply.last_context_tokens: AgentReply#last_context_tokens.
  GameEnv.reset: GameEnv#reset().
  RunState.surprises: RunState#surprises.
  RunState.resume_state: RunState#resume_state.
  RunState.escalated_at_actions: RunState#escalated_at_actions.
  GameRunner.resume_requested: GameRunner#resume_requested.
  _PARSE_RETRY_LIMIT: _PARSE_RETRY_LIMIT.
  RunnerConfig.cost_cap_usd: RunnerConfig#cost_cap_usd.
  AgentReply.stop_reason: AgentReply#stop_reason.
  GameEnv.step: GameEnv#step().
  RunState.fresh_sessions: RunState#fresh_sessions.
  RunState.parse_retries: RunState#parse_retries.
  RunState.model_requests: RunState#model_requests.
  RunState.context_tokens: RunState#context_tokens.
  RunState.last_planned_step: RunState#last_planned_step.
  GameRunner.agent: GameRunner#agent.
  GameRunner.resumed_at_actions: GameRunner#resumed_at_actions.
  GameRunner.prime_note: GameRunner#prime_note.
  _ESCALATE_RESETS: _ESCALATE_RESETS.
  ModelPricing.input_per_mtok: ModelPricing#input_per_mtok.
  ModelPricing.cached_per_mtok: ModelPricing#cached_per_mtok.
  ModelPricing.output_per_mtok: ModelPricing#output_per_mtok.
  RunnerConfig.max_output_tokens: RunnerConfig#max_output_tokens.
  RunnerConfig.fresh_session_input_tokens: RunnerConfig#fresh_session_input_tokens.
  RunnerConfig.max_model_requests: RunnerConfig#max_model_requests.
  RunnerConfig.request_timeout: RunnerConfig#request_timeout.
  AgentClient: AgentClient#
  GameEnv: GameEnv#
  ThinAgentClient: ThinAgentClient#
  _hit_output_token_limit: _hit_output_token_limit().
  _last_input_tokens: _last_input_tokens().
  RunState: RunState#
  GameRunner: GameRunner#
  write_scorecard: write_scorecard().
---
# Module: [`src/arc3/runner.py`](../../../../../../raw/code/Retrodict/src/arc3/runner.py)

## Classes
### `AgentClient`  ·  implements/extends Protocol
- def: [`src/arc3/runner.py:115`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L115)
- signature: `class AgentClient(Protocol):`
- members:
  - `invoke(self, prompt: str, resume_from: dict[str, Any] | None)` — [`L116`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L116)
- uses (calls/refs, reference-scoped): [`AgentReply`](runner.md#AgentReply)
- used by: [`_call`](runner.md#GameRunner._call), [`__init__`](runner.md#GameRunner.__init__)

### `AgentReply`
- def: [`src/arc3/runner.py:98`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L98)
- doc: One agent invocation's model-facing outcome.
- signature: `class AgentReply:`
- members:
  - `cached_tokens` — [`L104`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L104)
  - `input_tokens` — [`L103`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L103)
  - `last_context_tokens` — [`L112`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L112)
  - `model_requests` — [`L106`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L106)
  - `output_tokens` — [`L105`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L105)
  - `resume_state` — [`L102`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L102)
  - `stop_reason` — [`L107`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L107)
  - `text` — [`L101`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L101)
  - `truncated` — [`L108`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L108)
- used by: [`_call`](runner.md#GameRunner._call), [`_accept`](runner.md#GameRunner._accept), [`invoke`](runner.md#ThinAgentClient.invoke), [`_invoke`](runner.md#GameRunner._invoke), [`invoke`](runner.md#AgentClient.invoke)

### `GameEnv`  ·  implements/extends Protocol
- def: [`src/arc3/runner.py:119`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L119)
- signature: `class GameEnv(Protocol):`
- members:
  - `reset(self)` — [`L120`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L120)
  - `step(self, action: Any, data: dict[str, Any] | None = None, reasoning: dict[str, Any] | None = None)` — [`L122`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L122)
- used by: [`_restore`](runner.md#GameRunner._restore), [`_step`](runner.md#GameRunner._step), [`_reset_after_game_over`](runner.md#GameRunner._reset_after_game_over), [`_start_fresh`](runner.md#GameRunner._start_fresh), [`__init__`](runner.md#GameRunner.__init__)

### `GameRunner`
- def: [`src/arc3/runner.py:209`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L209)
- doc: Run one game to a terminal condition.
- signature: `class GameRunner:`
- members:
  - `_escalation_directive(self)` — [`L400`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L400) — Escalate a stuck level (par-free signals only) and render the binding directive, or ''. — documented in [arc3-runner](../../../concepts/arc3-runner.md)
  - `_image_prime(self)` — [`L256`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L256) — Ask a vision model to read the opening frame; store its answer for the first prompt. — documented in [arc3-runner](../../../concepts/arc3-runner.md)
  - `_restore(self)` — [`L277`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L277) — Rebuild env state by replaying the logged actions; continue accounting. — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `_seed_level_signals(self, records: list[StepRecord])` — [`L325`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L325) — Recover the current level's stuck signals from the replayed log. — documented in [arc3-logwriter](../../../concepts/arc3-logwriter.md)
  - `_start_level(self)` — [`L541`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L541) — A new level began: reset the per-level stuck signals and stand down any escalation.
  - `run(self)` — [`L228`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L228) — Play until WIN, a cap, or a failure; return (and write) metrics. — documented in [arc3-runner](../../../concepts/arc3-runner.md)
  - `agent` — [`L214`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L214)
  - `cfg` — [`L215`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L215)
  - `env` — [`L213`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L213)
  - `frame` — [`L223`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L223)
  - `log` — [`L219`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L219)
  - `pricing` — [`L221`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L221)
  - `prime_note` — [`L226`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L226)
  - `resume_requested` — [`L224`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L224)
  - `resumed_at_actions` — [`L225`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L225)
  - `run_dir` — [`L216`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L216)
  - `state` — [`L222`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L222) — documented in [arc3-runner](../../../concepts/arc3-runner.md)
  - `transcript_path` — [`L220`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L220)
  - `workspace` — [`L217`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L217)
- protocol/private: `__init__`[`L212`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L212), `_accept`[`L462`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L462), `_available_names`[`L474`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L474), `_build_prompt`[`L386`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L386), `_call`[`L427`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L427), `_check_expectations`[`L526`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L526), `_cost`[`L589`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L589), `_drain`[`L479`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L479), `_invoke`[`L373`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L373), `_log_frame`[`L561`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L561), `_loop`[`L358`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L358), `_metrics`[`L603`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L603), `_record_escalation`[`L416`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L416), `_reset_after_game_over`[`L549`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L549), `_seed_prior_usage`[`L346`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L346), `_start_fresh`[`L247`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L247), `_step`[`L498`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L498)
- uses (calls/refs, reference-scoped): [`append_step`](logwriter.md#LogWriter.append_step), [`parse_log`](logwriter.md#parse_log), [`parse_actions`](plan_parser.md#parse_actions), [`PlanParseError`](plan_parser.md#PlanParseError), [`name`](plan_parser.md#PlannedAction.name), [`_render_action`](runner.md#_render_action), [`actions_taken`](runner.md#RunState.actions_taken), [`resolve_pricing`](runner.md#RunnerConfig.resolve_pricing), [`escalation_tier`](runner.md#RunState.escalation_tier), [`PlannedAction`](plan_parser.md#PlannedAction), [`StepRecord`](logwriter.md#StepRecord), [`level_self_resets`](runner.md#RunState.level_self_resets), [`action`](logwriter.md#StepRecord.action), [`step_no`](runner.md#RunState.step_no), [`ParsedPlan`](plan_parser.md#ParsedPlan), [`describe_opening`](vision.md#describe_opening), [`game_id`](runner.md#RunnerConfig.game_id), [`levels_completed`](logwriter.md#StepRecord.levels_completed), [`model`](runner.md#RunnerConfig.model), [`action_name`](logwriter.md#action_name), [`actions`](plan_parser.md#ParsedPlan.actions), [`AgentReply`](runner.md#AgentReply), [`action_cap`](runner.md#RunnerConfig.action_cap), [`cached_tokens`](runner.md#RunState.cached_tokens), [`frames`](logwriter.md#StepRecord.frames), [`input_tokens`](runner.md#RunState.input_tokens), [`invocation_log`](runner.md#RunState.invocation_log), [`invocations`](runner.md#RunState.invocations), [`state`](logwriter.md#StepRecord.state), [`step`](logwriter.md#StepRecord.step), [`surprise_note`](runner.md#RunState.surprise_note), [`x`](logwriter.md#StepRecord.x), [`x`](plan_parser.md#PlannedAction.x), [`y`](logwriter.md#StepRecord.y), [`diff_boards`](logwriter.md#diff_boards), [`invoke`](runner.md#AgentClient.invoke), [`RunnerConfig`](runner.md#RunnerConfig), [`_board_lists`](runner.md#_board_lists), [`expect`](plan_parser.md#PlannedAction.expect), [`expect_levels`](plan_parser.md#ParsedPlan.expect_levels)  (+49 more)
- used by: [`run_game`](runner.md#run_game)

### `ModelPricing`
- def: [`src/arc3/runner.py:36`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L36)
- doc: USD per million tokens.
- signature: `class ModelPricing:`
- members:
  - `cached_per_mtok` — [`L40`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L40)
  - `input_per_mtok` — [`L39`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L39)
  - `output_per_mtok` — [`L41`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L41)
- used by: [`_cost`](runner.md#GameRunner._cost), [`resolve_pricing`](runner.md#RunnerConfig.resolve_pricing), [`PRICING`](runner.md#PRICING), [`pricing`](runner.md#RunnerConfig.pricing)

### `RunState`
- def: [`src/arc3/runner.py:185`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L185)
- doc: Mutable per-run accounting.
- signature: `class RunState:`
- members:
  - `actions_taken` — [`L189`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L189)
  - `cached_tokens` — [`L196`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L196)
  - `context_tokens` — [`L200`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L200)
  - `escalated_at_actions` — [`L205`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L205)
  - `escalation_tier` — [`L204`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L204)
  - `fresh_sessions` — [`L191`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L191)
  - `input_tokens` — [`L195`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L195)
  - `invocation_log` — [`L206`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L206)
  - `invocations` — [`L190`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L190)
  - `last_planned_step` — [`L201`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L201)
  - `level_self_resets` — [`L203`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L203)
  - `level_start_actions` — [`L202`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L202)
  - `model_requests` — [`L198`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L198)
  - `output_tokens` — [`L197`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L197)
  - `parse_retries` — [`L192`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L192)
  - `resume_state` — [`L199`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L199)
  - `step_no` — [`L188`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L188)
  - `surprise_note` — [`L194`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L194)
  - `surprises` — [`L193`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L193)
- used by: [`_call`](runner.md#GameRunner._call), [`_restore`](runner.md#GameRunner._restore), [`state`](runner.md#GameRunner.state), [`_metrics`](runner.md#GameRunner._metrics), [`_accept`](runner.md#GameRunner._accept), [`_log_frame`](runner.md#GameRunner._log_frame), [`_build_prompt`](runner.md#GameRunner._build_prompt), [`_step`](runner.md#GameRunner._step), [`_drain`](runner.md#GameRunner._drain), [`run`](runner.md#GameRunner.run), [`_cost`](runner.md#GameRunner._cost), [`_escalation_directive`](runner.md#GameRunner._escalation_directive), [`_image_prime`](runner.md#GameRunner._image_prime), [`_invoke`](runner.md#GameRunner._invoke), [`_reset_after_game_over`](runner.md#GameRunner._reset_after_game_over), [`_loop`](runner.md#GameRunner._loop), [`_start_fresh`](runner.md#GameRunner._start_fresh), [`_check_expectations`](runner.md#GameRunner._check_expectations), [`_seed_level_signals`](runner.md#GameRunner._seed_level_signals), [`_record_escalation`](runner.md#GameRunner._record_escalation), [`_start_level`](runner.md#GameRunner._start_level), [`_seed_prior_usage`](runner.md#GameRunner._seed_prior_usage)

### `RunnerConfig`
- def: [`src/arc3/runner.py:70`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L70)
- doc: Per-run knobs; defaults are the pilot protocol (gpt-5.5 at high effort, $80 cost cap, 2k action cap).
- signature: `class RunnerConfig:`
- members:
  - `resolve_pricing(self)` — [`L90`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L90)
  - `action_cap` — [`L77`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L77)
  - `cost_cap_usd` — [`L78`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L78)
  - `fresh_session_input_tokens` — [`L79`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L79)
  - `game_id` — [`L73`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L73)
  - `image_prime` — [`L87`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L87)
  - `max_model_requests` — [`L82`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L82)
  - `max_output_tokens` — [`L76`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L76)
  - `model` — [`L74`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L74)
  - `pricing` — [`L84`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L84)
  - `reasoning_effort` — [`L75`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L75)
  - `request_timeout` — [`L83`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L83)
  - `vision_model` — [`L88`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L88)
- uses (calls/refs, reference-scoped): [`ModelPricing`](runner.md#ModelPricing), [`PRICING`](runner.md#PRICING)
- used by: [`_metrics`](runner.md#GameRunner._metrics), [`_accept`](runner.md#GameRunner._accept), [`_build_prompt`](runner.md#GameRunner._build_prompt), [`_drain`](runner.md#GameRunner._drain), [`run`](runner.md#GameRunner.run), [`_cost`](runner.md#GameRunner._cost), [`_image_prime`](runner.md#GameRunner._image_prime), [`main`](runner.md#main), [`run_game`](runner.md#run_game), [`_reset_after_game_over`](runner.md#GameRunner._reset_after_game_over), [`_loop`](runner.md#GameRunner._loop), [`__init__`](runner.md#ThinAgentClient.__init__), [`__init__`](runner.md#GameRunner.__init__), [`pricing`](runner.md#GameRunner.pricing)

### `ThinAgentClient`
- def: [`src/arc3/runner.py:125`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L125)
- doc: AgentClient backed by a thinharness Harness over the run workspace.
- signature: `class ThinAgentClient:`
- members:
  - `aclose(self)` — [`L162`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L162)
  - `invoke(self, prompt: str, resume_from: dict[str, Any] | None)` — [`L147`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L147)
  - `harness` — [`L145`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L145)
- protocol/private: `__init__`[`L128`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L128)
- uses (calls/refs, reference-scoped): [`spec`](tools.md#PythonTool.spec), [`model`](runner.md#RunnerConfig.model), [`AgentReply`](runner.md#AgentReply), [`ANALYSIS_PYTHON`](runner.md#ANALYSIS_PYTHON), [`RunnerConfig`](runner.md#RunnerConfig), [`PythonTool`](tools.md#PythonTool), [`cached_tokens`](runner.md#AgentReply.cached_tokens), [`input_tokens`](runner.md#AgentReply.input_tokens), [`last_context_tokens`](runner.md#AgentReply.last_context_tokens), [`model_requests`](runner.md#AgentReply.model_requests), [`output_tokens`](runner.md#AgentReply.output_tokens), [`reasoning_effort`](runner.md#RunnerConfig.reasoning_effort), [`resume_state`](runner.md#AgentReply.resume_state), [`text`](runner.md#AgentReply.text), [`truncated`](runner.md#AgentReply.truncated), [`stop_reason`](runner.md#AgentReply.stop_reason), [`SYSTEM_PROMPT`](prompts.md#SYSTEM_PROMPT), [`_hit_output_token_limit`](runner.md#_hit_output_token_limit), [`_last_input_tokens`](runner.md#_last_input_tokens), [`max_model_requests`](runner.md#RunnerConfig.max_model_requests), [`max_output_tokens`](runner.md#RunnerConfig.max_output_tokens), [`request_timeout`](runner.md#RunnerConfig.request_timeout)
- used by: [`run_game`](runner.md#run_game)

## Functions
- `_board_lists(board: Any)` — [`L637`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L637)
- `_hit_output_token_limit(responses: list[dict[str, Any]])` — [`L166`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L166) — Best-effort check that the final provider turn was cut off at max_output_tokens.
- `_last_input_tokens(responses: list[dict[str, Any]])` — [`L175`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L175) — Input tokens of the final provider request, i.e. the conversation size.
- `_render_action(action: PlannedAction)` — [`L631`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L631)
- `containment_check(workspace: Path, analysis_python: Path = ANALYSIS_PYTHON)` — [`L644`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L644) — Prove the agent interpreter cannot import the game engine; abort the run if it can.
- `main(argv: list[str] | None = None)` — [`L712`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L712)
- `open_environment(game_id: str, run_dir: Path, mode: str)` — [`L655`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L655) — Open the game via arc-agi; NORMAL downloads and runs locally, ONLINE plays the API.
- `run_game(cfg: RunnerConfig, runs_root: Path, mode: str = "normal", resume_dir: Path | None = None)` — [`L682`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L682) — Materialize a run directory, gate on containment, and play one game.
- `write_scorecard(arcade, run_dir: Path)` — [`L670`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L670) — Persist the engine's official scorecard (per-level actions and scores) beside metrics.json.

## Module values
- `ANALYSIS_PYTHON` — [`L27`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L27)
- `ENVIRONMENTS_DIR` — [`L28`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L28)
- `PRICING` — [`L45`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L45)
- `REPO_ROOT` — [`L26`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L26)
- `WORKSPACE_TEMPLATE` — [`L29`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L29)
- `_ESCALATE_ACTIONS` — [`L32`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L32)
- `_ESCALATE_RESETS` — [`L31`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L31)
- `_PARSE_RETRY_LIMIT` — [`L30`](../../../../../../raw/code/Retrodict/src/arc3/runner.py#L30)

