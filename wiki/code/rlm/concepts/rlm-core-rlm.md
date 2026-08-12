---
title: RLM — the completion loop, sub-calls, and context offloading
type: concept
provenance: mixed
concept: rlm-core-rlm
updated: 2026-08-12
status: fresh
---
# RLM — the completion loop, sub-calls, and context offloading

## Overview

[`RLM`](../catalog/rlm/core/rlm.md#RLM) is the class a caller instantiates in place of an ordinary model
client. Its [`completion`](../catalog/rlm/core/rlm.md#RLM.completion) method is a drop-in replacement for a
plain chat-completion call, but internally it never puts the caller's full prompt into any model's context
directly: it spins up a REPL environment, hands the model only metadata about the prompt, and lets the
model *write code* to inspect and process it. The root idea — the mechanism behind
[Recursive Language Models](../../../sources/recursive-language-models.md)'s core claim — is that
`completion()` and `_subcall()` both bottom out in the same recursive structure: an RLM at depth `d` can
spawn a child RLM at depth `d+1`, and only stops recursing (falls back to a plain model call) once `depth
>= max_depth`.

## Diagram

```mermaid
flowchart TD
    A["completion(prompt)"] -->|depth >= max_depth?| B["_fallback_answer(prompt)"]
    A -->|else| C["_spawn_completion_context(prompt)"]
    C --> D["get_client(backend) → LMHandler.start()"]
    C --> E["get_environment(...) — REPL with prompt bound as a variable"]
    D & E --> F["_setup_prompt: model sees length + prefix, not the full prompt"]
    F --> G["loop: _completion_turn(prompt, lm_handler, environment)"]
    G -->|model writes code| H["environment.execute_code(code) → REPLResult"]
    H -->|code calls rlm(...)| I["_subcall(prompt, model)"]
    I -->|next_depth < max_depth| J["spawn child RLM.completion(...)"]
    I -->|next_depth >= max_depth| K["plain client.completion(prompt)"]
    J & K --> L["RLMChatCompletion returned to REPL as a bound value"]
    L --> G
    G -->|model sets Final variable| M["return RLMChatCompletion"]
    G -->|_check_iteration_limits raises| N["error/budget/token limit exceeded"]
```

## Design rationale (why it's built this way)

**The prompt never enters the model's own context window.** [`_spawn_completion_context`](../catalog/rlm/core/rlm.md#RLM._spawn_completion_context)
constructs the REPL with `context_payload=prompt` and passes only the environment's *handle* forward;
[`_setup_prompt`](../catalog/rlm/core/rlm.md#RLM._setup_prompt) builds the system message the root model
actually sees, which describes the variable's shape (length, a short prefix) rather than its content. This
is the literal implementation of "context as a variable" — the REPL, not the model's token buffer, is where
the long input lives.

**Sub-calls are just another kind of code execution.** [`_subcall`](../catalog/rlm/core/rlm.md#RLM._subcall)
is registered as a callback into the REPL (`LocalREPL`'s `subcall_fn`), so when the model's generated code
invokes the sub-call primitive, it's an ordinary function call from the REPL's point of view — not a special
tool-calling protocol. This is the paper's stated bet against JSON tool schemas: recursion is *code*, not a
structured message type.

**Depth is a hard ceiling with a graceful floor.** `_subcall` computes `next_depth = self.depth + 1` and,
the moment that would reach `max_depth`, routes to a **plain** model completion instead of spawning another
RLM — with an explicit *model-override* path (`model` argument) so a parent can hand a cheaper model to its
children even if it defaults to a stronger one for itself. This is the mechanical anchor for the
[RLM paper](../../../sources/recursive-language-models.md)'s `RLM(model, depth=N)` notation and its finding
that recursion depth has diminishing (and sometimes negative) returns — the code makes the ceiling explicit
rather than emergent.

**Limits are checked after every iteration, not just at the end.** [`_check_iteration_limits`](../catalog/rlm/core/rlm.md#RLM._check_iteration_limits)
inspects each iteration's `stderr` for errors, tracks a consecutive-error counter (reset on any clean
iteration), and separately tracks cumulative cost against `max_budget` and usage against `max_tokens` —
three independent circuit breakers a single long-running recursive session can trip.

## Entry points
- [`RLM.completion`](../catalog/rlm/core/rlm.md#RLM.completion) — the top-level call a caller makes; spawns
  a fresh environment + [`LMHandler`](../catalog/rlm/core/lm_handler.md#LMHandler) per call unless
  `persistent=True`.
- [`RLM._subcall`](../catalog/rlm/core/rlm.md#RLM._subcall) — reached only from inside model-generated code
  running in the REPL, via the `subcall_fn` callback wired into
  [`LocalREPL`](../catalog/rlm/environments/local_repl.md#LocalREPL) or
  [`IPythonREPL`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL).
- [`RLM.close`](../catalog/rlm/core/rlm.md#RLM.close) — required cleanup for a `persistent=True` RLM holding
  a long-lived [`_persistent_env`](../catalog/rlm/core/rlm.md#RLM._persistent_env) across multiple
  `completion()` calls (multi-turn use).

## Mechanism (step-by-step)

1. **[`RLM.completion`](../catalog/rlm/core/rlm.md#RLM.completion) checks the depth ceiling first.** If
   `self.depth >= self.max_depth`, there is no REPL at all — the call falls straight through to a plain
   model completion, because at the leaf of the recursion tree an RLM degenerates into an ordinary LM.
2. **`_spawn_completion_context` wires up the client, the sub-call handler, and the environment together**,
   registering `other_backends` (if configured) as additional callable model names inside
   [`LMHandler`](../catalog/rlm/core/lm_handler.md#LMHandler) — this is how a parent RLM lets its generated
   code address more than one downstream model by name.
3. **The iteration loop (`_completion_turn`) alternates a model turn and a code-execution turn**: the model
   sees the running message history (built by [`format_iteration`](../catalog/rlm/utils/parsing.md#format_iteration),
   which truncates long results before they re-enter history — a second, smaller instance of the same
   "don't let content flood context" discipline the whole system is built around) and returns a response
   containing code; the environment executes it and returns a [`REPLResult`](../catalog/rlm/core/types.md#REPLResult)
   with `stdout`/`stderr`/`final_answer`/any `rlm_calls` made.
4. **A sub-call inside that code becomes `_subcall`**, which either spawns a genuine child RLM (propagating
   a logger if the parent has one — see the test coverage on logger propagation) or, at the depth ceiling,
   degrades to a plain [`BaseLM.completion`](../catalog/rlm/clients/base_lm.md#BaseLM.completion) call and
   wraps the result in the same [`RLMChatCompletion`](../catalog/rlm/core/types.md#RLMChatCompletion) shape
   either way — callers never see a different return type depending on whether recursion actually happened.
5. **[`_check_iteration_limits`](../catalog/rlm/core/rlm.md#RLM._check_iteration_limits) runs after every
   iteration**, and any of the three limits it enforces (consecutive errors, budget, tokens) aborts the loop
   with the best partial answer preserved.
6. **The loop ends when the model sets the `Final` variable** (surfaced through `REPLResult.final_answer`)
   or exhausts `max_iterations`, in which case [`_default_answer`](../catalog/rlm/core/rlm.md#RLM._default_answer)
   produces a best-effort response from whatever history exists.

## Key data structures
- [`RLMChatCompletion`](../catalog/rlm/core/types.md#RLMChatCompletion) — the uniform return type for both a
  root call and a sub-call: `root_model`, `prompt`, `response`, `usage_summary`, `execution_time`, and an
  optional `metadata` field carrying the full child trajectory when a logger captured it.
- [`UsageSummary`](../catalog/rlm/core/types.md#UsageSummary) — aggregates
  [`ModelUsageSummary`](../catalog/rlm/core/types.md#ModelUsageSummary) per model name, so a multi-model
  recursive tree's cost is attributable back to which model did what.
- [`RLMIteration`](../catalog/rlm/core/types.md#RLMIteration) / [`REPLResult`](../catalog/rlm/core/types.md#REPLResult) —
  one iteration's model response plus the code blocks it triggered and their stdout/stderr/final-answer.

## Dynamics (design intent)
`max_concurrent_subcalls` (default 4, threaded through `RLM.__init__` into the environment) caps how many
sub-RLM calls a single iteration's code can have in flight at once — recursion is concurrent by default, not
serial, which is why a single REPL turn can dispatch several sub-tasks and wait on all of them. The test
suite's dedicated coverage of logger propagation across `_subcall` boundaries
([`test_child_gets_logger_when_parent_has_logger`](../catalog/tests/test_depth_metadata.md#TestSubcallLoggerPropagation.test_child_gets_logger_when_parent_has_logger),
[`test_leaf_subcall_returns_no_metadata`](../catalog/tests/test_depth_metadata.md#TestSubcallLoggerPropagation.test_leaf_subcall_returns_no_metadata))
indicates this was a real bug surface: a child RLM only gets its own trajectory logger if the parent had
one, and a leaf-depth sub-call (one that degrades to a plain LM call) legitimately carries no `metadata` at
all, which downstream code must not assume is present.

## Edge cases
- A `persistent=True` RLM reuses `_persistent_env` across calls; the code defensively checks the environment
  actually supports the required persistence methods (`update_handler_address`, `add_context`,
  `get_context_count`) before trusting it, rather than assuming every environment backend implements them.
- `_subcall`'s `model` override only changes *which model* answers; it does not change `max_depth` or any
  other structural setting — a child spawned with a different model still counts against the same depth
  budget as its siblings.
- On an exception during a sub-call, `_subcall` catches it and returns an `RLMChatCompletion` carrying the
  error as the response rather than raising — a sub-call failure is data the parent's REPL code can react
  to, not a hard stop of the whole completion.

## Open questions
- The exact compaction trigger threshold interaction with `_check_iteration_limits`'s token check (whether
  compaction is guaranteed to fire before the token limit trips, or can race it) is not settled by anything
  in this packet's subgraph.

## See also
- [`rlm-environments-local_repl`](rlm-environments-local_repl.md) — the concrete REPL implementation
  `_spawn_completion_context` wires the sub-call callback into.
- [`rlm-core-lm_handler`](rlm-core-lm_handler.md) — the socket-server side of how the REPL actually reaches
  a model without the model's own weights being in-process.
- [`rlm-core-types`](rlm-core-types.md) — the full data-model reference for `RLMChatCompletion`,
  `UsageSummary`, `RLMIteration`, `REPLResult`.
