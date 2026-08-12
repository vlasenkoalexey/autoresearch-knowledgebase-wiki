---
title: 'Module: src/arc3/prompts.py'
type: catalog
provenance: extracted
module: src/arc3/prompts.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.prompts`/
symbols:
  SYSTEM_PROMPT: SYSTEM_PROMPT.
  initial_prompt: initial_prompt().
  reinvoke_prompt: reinvoke_prompt().
  fresh_session_prompt: fresh_session_prompt().
  escalation_directive: escalation_directive().
  parse_retry_prompt: parse_retry_prompt().
  REINVOKE_REASONS: REINVOKE_REASONS.
---
# Module: [`src/arc3/prompts.py`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py)

## Functions
- `escalation_directive(tier: int, actions_this_level: int, self_resets: int)` — [`L212`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L212) — Appended by the runner when the current level looks stuck; absent otherwise.
- `fresh_session_prompt(game_id: str, last_step: int, reason: str)` — [`L195`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L195) — First invocation of a fresh conversation mid-run; the log is the only memory.
- `initial_prompt(game_id: str, prime_note: str | None = None)` — [`L166`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L166) — First invocation of a run; prime_note is an optional vision-model read of the opening frame.
- `parse_retry_prompt(error: str)` — [`L236`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L236) — Ask the model to re-emit a valid [ACTIONS] block after a parse failure.
- `reinvoke_prompt(reason: str, first_new_step: int, last_step: int)` — [`L185`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L185) — Continuation within the same conversation after the queue stopped.

## Module values
- `REINVOKE_REASONS` — [`L244`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L244)
- `SYSTEM_PROMPT` — [`L11`](../../../../../../raw/code/Retrodict/src/arc3/prompts.py#L11)

