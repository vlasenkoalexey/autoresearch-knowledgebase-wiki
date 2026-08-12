---
title: IPythonREPL — kernel-backed REPL with an explicit in-process/subprocess isolation choice
type: concept
provenance: mixed
concept: rlm-environments-ipython_repl
updated: 2026-08-12
status: fresh
---
# IPythonREPL — kernel-backed REPL with an explicit in-process/subprocess isolation choice

## Overview

[`IPythonREPL`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL) runs model-generated code through a
real IPython kernel rather than a bare `exec`, in one of two modes: `kernel_mode="in_process"` (default,
shares the parent process) or `"subprocess"` (a genuinely separate `ipykernel` process). The choice trades
speed for isolation, and the class's own docstring is unusually candid about exactly where in-process mode
leaks.

## Design rationale

**In-process isolation is explicitly imperfect, by the code's own account.** `sys.stdout`/`sys.stderr`
redirection, `os.chdir`, and `signal.SIGALRM` are process-global in in-process mode — "any other thread in
the parent that touches them while a cell is running will see the shadowed state." Two in-process instances
each get a **unique user module** ([`_setup_in_process`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL._setup_in_process)
names it `_rlm_ipython_main_<uuid>`) specifically so they don't collide on `sys.modules['__main__']`, but
the surrounding process is still shared — the docstring recommends `kernel_mode="subprocess"` when that
matters.

**Subcall attribution has a documented gotcha in subprocess mode**: a background thread or `asyncio.Task`
spawned by one cell that calls `rlm_query` after that cell has already finished gets attributed to
*whichever cell is active when the kernel actually issues the request*, not the cell that spawned it — the
docstring's own advice is to avoid leaving background work running across cells.

**Custom tools are injected differently per mode**: in-process mode writes directly into `shell.user_ns`;
subprocess mode (`_inject_custom_tools_subprocess`) prefers `dill` (which pickles callables by value, including their closures — no import of the defining
module needed inside the kernel) and falls back to a JSON round-trip for plain data if `dill` isn't
installed, raising a clear error if neither path can serialize a given tool.

## Entry points
- [`IPythonREPL.execute_code`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL.execute_code) —
  dispatches to the in-process or subprocess execution path depending on `kernel_mode`.
- [`_restore_scaffold_in_process`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL._restore_scaffold_in_process) —
  re-injects `rlm_query`, `answer`, and custom tools before every cell, defensively recovering from a user
  overwriting a reserved name.

## Edge cases
- `cell_timeout` is a **hard guarantee** in subprocess mode (via kernel interrupt) but only **best-effort**
  in in-process mode (via `SIGALRM` on Unix, from the main thread only) — a runaway cell in in-process mode
  is not guaranteed to actually stop.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the shared contract.
- [`rlm-environments-local_repl`](rlm-environments-local_repl.md) — the simpler same-machine alternative
  this backend supersedes when kernel semantics or subprocess isolation matter.
