---
title: tools/bash — the coding agent's one-shot shell-execution tool
type: concept
provenance: mixed
concept: tools-bash
updated: 2026-07-04
status: fresh
---
# tools/bash — the coding agent's one-shot shell-execution tool

## Overview
`tools/bash.py` is one of the two tools (the other is a whole-file edit tool) the frozen coding agent (see
[`../coding_agent.md`](../coding_agent.md)) is wired with — it is how the LLM actually executes shell
commands, whether it is solving a SWE-bench/Polyglot task or, in self-improve mode, editing DGM's own
source. Its core class, [`BashSession`](../catalog/tools/bash.md#BashSession) ("A session of a bash
shell."), is built around a *persistent* interactive shell subprocess driven by a sentinel-echo protocol —
but the way the tool is actually wired up for the agent constructs and abandons a **brand-new session on
every single tool call**. The class is designed for a long-lived shell; the wiring uses it as a one-shot
executor. That gap is the single most important thing to understand about this file, and it is also the
file the self-referential loop is permitted to rewrite (see
[`../../../concepts/self-referential-code-rewriting.md`](../../../concepts/self-referential-code-rewriting.md)),
so its own execution semantics are themselves fair game for a future self-edit.

## Diagram
```mermaid
sequenceDiagram
    participant Agent as coding agent tool loop
    participant TF as tool_function
    participant TFC as tool_function_call
    participant BS as new BashSession()
    participant Sh as "/bin/bash -i" subprocess

    Agent->>TF: command (LLM-issued)
    TF->>TFC: asyncio.run(tool_function_call(command))
    TFC->>BS: BashSession() — fresh instance, _started=False
    TFC->>BS: start()
    BS->>Sh: create_subprocess_shell("/bin/bash -i", setsid)
    TFC->>BS: run(command)
    BS->>Sh: write command + "; echo '<<exit>>'"
    loop every _output_delay (0.2s), up to _timeout (120s)
        BS->>Sh: poll stdout/stderr internal buffers
    end
    Sh-->>BS: sentinel appears in stdout
    BS-->>TFC: (output, error)
    TFC->>TFC: filter_error(error)
    TFC-->>TF: result string ("<output>" / "Error:\n...")
    TF-->>Agent: result string
    Note over BS,Sh: stop() is never invoked on this path —<br/>the subprocess is simply abandoned
```

## Design rationale (why it's built this way)
[`BashSession`](../catalog/tools/bash.md#BashSession) is written like a real terminal session: it spawns
`/bin/bash -i` once, then would let a caller send it command after command via
[`run`](../catalog/tools/bash.md#BashSession.run), keeping cwd/env/shell variables alive between calls the
way a human's terminal does. Because bash never exits on its own after one command, `run` cannot just wait
for EOF — instead it writes the command followed by `; echo '<<exit>>'`
([`_sentinel`](../catalog/tools/bash.md#BashSession._sentinel)) and polls the process's stdout every
[`_output_delay`](../catalog/tools/bash.md#BashSession._output_delay) (0.2s) until that marker shows up,
at which point everything before it is the command's real output. `run` reads directly from
`self._process.stdout._buffer`/`stderr._buffer` — the private internal buffer of the asyncio stream reader
— rather than an ordinary `readline()`/`read()`; that lets it repeatedly peek at partial output without
consuming/blocking on it, but it is a fragile reliance on asyncio internals rather than a public streaming
API. `> [!inferred]` The `-i` flag and `preexec_fn=os.setsid` are not explained in a comment; running bash
interactively is the straightforward way to get a real shell environment (aliases, `$PS1`-style built-ins),
and `setsid` puts the child in its own session so [`stop`](../catalog/tools/bash.md#BashSession.stop) can
`terminate()` exactly that process group without touching the parent.

That interactive shell has a side effect the module has to actively suppress:
[`filter_error`](../catalog/tools/bash.md#filter_error) strips "Inappropriate ioctl for device" lines that
`bash -i` emits on stderr when it tries terminal job-control ioctls against a pipe instead of a real tty —
expected plumbing noise, not a real command error, that would otherwise be reported to the LLM as if the
command itself had failed. The filter is a fixed-offset heuristic (skip 3 lines, optionally one more if the
sentinel lands there, then keep the rest) tuned to this specific warning shape rather than a general ioctl
parser.

Despite all of this persistent-session machinery, the tool as actually exposed to the agent throws it away
every call: [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) constructs a fresh
`bash_session = BashSession()` and, because `_started` is always `False` on a brand-new instance, always
calls [`start`](../catalog/tools/bash.md#BashSession.start) — there is no code path in this subgraph that
reuses one `BashSession` across two different `tool_function` invocations. The test suite's own "state
persistence" cases confirm this by construction rather than by accident: both
[`test_environment_variables`](../catalog/tests/test_bash_tool.md#TestBashTool.test_environment_variables)
(`"TEST_VAR='hello' && echo $TEST_VAR"`) and
[`test_multiple_commands`](../catalog/tests/test_bash_tool.md#TestBashTool.test_multiple_commands)
(`"echo 'first' && echo 'second'"`) join everything into one `&&`-chained string passed to a single
`tool_function` call — because that is the only way this wiring can carry state from one shell statement to
the next.

## Entry points
- [`tool_function`](../catalog/tools/bash.md#tool_function) — the synchronous callable
  `tool_function(command)` the agent's tool-dispatch loop invokes with the LLM-issued command string; it is
  a thin `asyncio.run(...)` wrapper so a synchronous caller can drive the async session underneath.
- [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) — the async implementation
  `tool_function` hands off to immediately; its docstring is simply `"""Execute a command in the bash
  shell."""`, and this is where a session is created, started, run, and turned into the final result string.
- [`result`](../catalog/tools/bash.md#result) — the module's own `if __name__ == "__main__":` entry point
  (`python bash.py '<command>'`), a standalone way to exercise the tool outside the agent loop.

## Mechanism (step-by-step)
1. **Dispatch from the agent loop.** The tool-dispatch layer calls
   [`tool_function`](../catalog/tools/bash.md#tool_function) with the raw command string the LLM produced;
   `tool_function` immediately runs [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) to
   completion via `asyncio.run`, so from the caller's perspective this is an ordinary blocking function call.
2. **A brand-new session is created and started, every time.**
   [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) instantiates
   [`BashSession`](../catalog/tools/bash.md#BashSession), whose constructor sets
   [`_started`](../catalog/tools/bash.md#BashSession._started) to `False` and
   [`_process`](../catalog/tools/bash.md#BashSession._process) to `None`; since a fresh instance is never
   started, `tool_function_call` unconditionally awaits
   [`start`](../catalog/tools/bash.md#BashSession.start), which spawns `/bin/bash -i` as a new subprocess in
   its own session (`preexec_fn=os.setsid`) with the current environment copied in.
3. **The command is sent with a sentinel, and output is polled until it appears.**
   [`run`](../catalog/tools/bash.md#BashSession.run) writes the command plus
   `"; echo '<sentinel>'"` (using [`_sentinel`](../catalog/tools/bash.md#BashSession._sentinel), the literal
   string `"<<exit>>"`) to the subprocess's stdin, then loops — sleeping
   [`_output_delay`](../catalog/tools/bash.md#BashSession._output_delay) (0.2s) between checks — reading the
   process's stdout/stderr buffers directly until the sentinel shows up in stdout, at which point everything
   before it is returned as the command's output. If the sentinel never appears within
   [`_timeout`](../catalog/tools/bash.md#BashSession._timeout) (120s), `run` sets
   [`_timed_out`](../catalog/tools/bash.md#BashSession._timed_out) to `True` and raises a `ValueError`; no
   test in this subgraph drives a command anywhere near that limit —
   [`test_long_running_command`](../catalog/tests/test_bash_tool.md#TestBashTool.test_long_running_command)
   only sleeps 1 second.
4. **Stderr noise from the interactive shell itself is filtered before it reaches the LLM.**
   [`filter_error`](../catalog/tools/bash.md#filter_error) strips the "Inappropriate ioctl for device"
   lines `bash -i` emits when it attempts terminal control against a non-tty pipe, so a clean command that
   merely triggered this shell-plumbing warning is not reported to the model as an error.
5. **Any failure becomes ordinary tool-result text, never a raised exception.**
   [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) wraps the whole session lifecycle
   in a `try`/`except Exception`, returning `f"Error: {str(e)}"` on any failure — a nonexistent command
   (exercised by
   [`test_invalid_commands`](../catalog/tests/test_bash_tool.md#TestBashTool.test_invalid_commands) and
   [`test_command_with_error`](../catalog/tests/test_bash_tool.md#TestBashTool.test_command_with_error)), a
   timeout, or any other `run`/`start` exception all surface identically as plain text in the tool's return
   value, so the agent's outer loop never needs special-case handling for this tool failing.
6. **The subprocess is never explicitly torn down on this path.**
   [`stop`](../catalog/tools/bash.md#BashSession.stop) exists to `terminate()` the process and reset
   [`_started`](../catalog/tools/bash.md#BashSession._started)/[`_process`](../catalog/tools/bash.md#BashSession._process),
   but nothing in this subgraph calls it from
   [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) — the local `bash_session` simply
   goes out of scope at the end of the call, leaving the spawned `/bin/bash -i` process without an explicit
   termination signal from this module.

## Key data structures
- [`BashSession`](../catalog/tools/bash.md#BashSession) — one shell subprocess plus its protocol state:
  [`_started`](../catalog/tools/bash.md#BashSession._started) (has `start()` run yet),
  [`_process`](../catalog/tools/bash.md#BashSession._process) (the `asyncio` subprocess handle),
  [`_timed_out`](../catalog/tools/bash.md#BashSession._timed_out) (latched `True` once a `run` call exceeds
  [`_timeout`](../catalog/tools/bash.md#BashSession._timeout), 120s by default, and never reset back to
  `False` anywhere in this subgraph), [`_sentinel`](../catalog/tools/bash.md#BashSession._sentinel)
  (`"<<exit>>"`, the completion marker), and
  [`_output_delay`](../catalog/tools/bash.md#BashSession._output_delay) (0.2s poll interval).
- The `(output, error)` pair [`run`](../catalog/tools/bash.md#BashSession.run) returns — stdout up to the
  sentinel, and raw stderr — which [`tool_function_call`](../catalog/tools/bash.md#tool_function_call) folds
  into one plain-text result string (`output`, then `"\nError:\n" + filtered_error` if any error remains
  after [`filter_error`](../catalog/tools/bash.md#filter_error)).

## Dynamics (design intent)
Nothing in this subgraph runs the bash tool concurrently with itself — each
[`tool_function`](../catalog/tools/bash.md#tool_function) call is a self-contained
`asyncio.run(...)`, and [`run`](../catalog/tools/bash.md#BashSession.run)'s sentinel-poll loop is a plain
sequential wait, not an event-driven read. The tests all drive exactly one
[`tool_function`](../catalog/tools/bash.md#tool_function) call per case —
[`test_simple_command`](../catalog/tests/test_bash_tool.md#TestBashTool.test_simple_command),
[`test_command_with_special_chars`](../catalog/tests/test_bash_tool.md#TestBashTool.test_command_with_special_chars),
[`test_multiple_line_output`](../catalog/tests/test_bash_tool.md#TestBashTool.test_multiple_line_output), and
[`test_large_output_handling`](../catalog/tests/test_bash_tool.md#TestBashTool.test_large_output_handling)
all confirm the sentinel/poll loop correctly reassembles multi-line and large output up to the marker — none
of them chain two separate `tool_function` calls together to check that shell state (a `cd`, an exported
variable) survives between them.

## Edge cases
- A command that never finishes within 120s latches
  [`_timed_out`](../catalog/tools/bash.md#BashSession._timed_out) permanently `True` on that `BashSession`
  instance (nothing in this subgraph resets it) — but because every
  [`tool_function`](../catalog/tools/bash.md#tool_function) call gets a fresh instance anyway, that
  permanence is currently moot for the wired-in tool; it would only matter if some other, out-of-subgraph
  caller reused one `BashSession` object directly.
- [`filter_error`](../catalog/tools/bash.md#filter_error)'s fixed-offset skip (3 lines, then one more if the
  sentinel is there) is tuned to one specific ioctl-warning shape; a differently formatted warning from a
  different bash build would not be recognized and would leak through to the LLM as a spurious error.
- The command string is written to stdin as-is (`command.encode()`), with no escaping, validation, or
  sandboxing applied by this module —
  [`test_command_with_special_chars`](../catalog/tests/test_bash_tool.md#TestBashTool.test_command_with_special_chars)
  confirms arbitrary special characters pass straight through to the shell unmodified.
- Because [`stop`](../catalog/tools/bash.md#BashSession.stop) is never called from
  [`tool_function_call`](../catalog/tools/bash.md#tool_function_call), every tool call leaves behind a
  `/bin/bash -i` process that this module never explicitly terminates.

## Open questions
- The module also defines a `tool_info()` function (outside this packet's subgraph) whose description text
  tells the calling LLM "State is persistent across command calls" — which the fresh-`BashSession`-per-call
  wiring documented above appears to contradict for anything not chained into a single command string with
  `&&`. Whether that's a known simplification, a stale docstring, or resolved by something outside this
  subgraph isn't settled here.
- Whether the `/bin/bash -i` processes left behind after every call (since
  [`stop`](../catalog/tools/bash.md#BashSession.stop) has no caller in this subgraph) are ever reaped by
  something else — e.g. the disposable-container teardown described in the sibling `self_improve_step`
  concept — isn't visible from this file alone.
- This page does not tag `self-referential-code-rewriting`: nothing in *this* packet's subgraph (which is
  purely "how the bash tool executes one shell command") shows the self-improve mechanism reading, diffing,
  or re-validating `tools/bash.py` itself — that evidence lives in the DGM_outer/self_improve_step machinery
  and the paper, not in this file's own symbols.

## See also
- [`../coding_agent.md`](../coding_agent.md) — the agent this tool is wired into.
- [`../../../concepts/self-referential-code-rewriting.md`](../../../concepts/self-referential-code-rewriting.md) —
  the cross-repo concept naming this file as a legitimate self-edit target.
- [`../../../sources/darwin-godel-machine.md`](../../../sources/darwin-godel-machine.md) — the paper this
  code implements.
