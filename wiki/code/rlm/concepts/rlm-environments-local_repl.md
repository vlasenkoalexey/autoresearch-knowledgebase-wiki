---
title: LocalREPL — the default, same-process REPL backend
type: concept
provenance: mixed
concept: rlm-environments-local_repl
updated: 2026-08-12
status: fresh
---
# LocalREPL — the default, same-process REPL backend

## Overview

[`LocalREPL`](../catalog/rlm/environments/local_repl.md#LocalREPL) is the default environment
(`RLM.__init__`'s `environment: EnvironmentType = "local"`) — a persistent Python namespace running as a
subprocess on the same machine as the caller, one of the [`NonIsolatedEnv`](rlm-environments-base_env.md)
family. It binds the long input as a plain Python variable in that namespace and executes model-generated
code against it directly, with no container or sandbox boundary — the cheapest and fastest of the seven
backends, at the cost of the least isolation.

## Design rationale

**Every instance gets its own throwaway temp directory** (`tempfile.mkdtemp(prefix="repl_env_...")`) and a
`threading.Lock` guarding execution — so a `LocalREPL`'s working state is isolated from other instances in
the same process even though the *process* itself is shared with the caller. `subcall_fn` is wired directly
in as a constructor argument (see [`rlm-core-rlm`](rlm-core-rlm.md)'s `_spawn_completion_context`), making
recursive calls an ordinary in-namespace function rather than anything crossing a process or network
boundary — the cheapest possible sub-call path in the repo.

## Entry points
- [`LocalREPL.execute_code`](../catalog/rlm/environments/local_repl.md#LocalREPL.execute_code) — implements
  the `BaseEnv` contract; runs code in the persistent namespace and returns a `REPLResult`.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the shared abstraction and custom-tools
  mechanism this backend uses.
- [`rlm-environments-ipython_repl`](rlm-environments-ipython_repl.md) — the richer same-machine alternative
  with real kernel semantics and subprocess isolation option.
