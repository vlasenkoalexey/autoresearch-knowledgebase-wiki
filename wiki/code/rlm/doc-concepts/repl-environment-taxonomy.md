---
title: REPL environment taxonomy — non-isolated vs. isolated
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-12
status: fresh
---
# REPL environment taxonomy — non-isolated vs. isolated

## Definition
The README frames the seven supported environments (`local`, `ipython`, `docker`, `modal`, `prime`,
`daytona`, `e2b`) as two families with different threat models: **non-isolated** environments run on the
same machine as the RLM (fine for "simple benchmarking," explicitly not recommended for production or
untrusted input), and **isolated** environments run on separate, cloud-based sandbox machines, "ensuring
complete isolation from the host process."

## In rlm (grounded)
The taxonomy is a real class hierarchy, not just README prose: [`BaseEnv`](../catalog/rlm/environments/base_env.md#BaseEnv)
splits into [`NonIsolatedEnv`](../catalog/rlm/environments/base_env.md#NonIsolatedEnv) (backing
[`LocalREPL`](../catalog/rlm/environments/local_repl.md#LocalREPL),
[`IPythonREPL`](../catalog/rlm/environments/ipython_repl.md#IPythonREPL),
[`DockerREPL`](../catalog/rlm/environments/docker_repl.md#DockerREPL)) and
[`IsolatedEnv`](../catalog/rlm/environments/base_env.md#IsolatedEnv) (backing
[`ModalREPL`](../catalog/rlm/environments/modal_repl.md#ModalREPL),
[`PrimeREPL`](../catalog/rlm/environments/prime_repl.md#PrimeREPL),
[`DaytonaREPL`](../catalog/rlm/environments/daytona_repl.md#DaytonaREPL),
[`E2BREPL`](../catalog/rlm/environments/e2b_repl.md#E2BREPL)). The README's specific claim about isolated
backends — "whenever a recursive sub-call is made in these instances, it is requested from the host
process" — is exactly the broker-and-poll bridge documented in
[`rlm-environments-base_env`](../concepts/rlm-environments-base_env.md).

## Why it matters / when it applies
This is the security-relevant axis a caller must choose deliberately: `local`/`ipython` share the host's
Python environment and dependencies (convenient, unsafe for untrusted prompts), while the isolated backends
cost more setup (cloud auth, sandbox provisioning) in exchange for a genuine process/machine boundary. The
README's own guidance for `DockerREPL` — "custom tools should be passed as Python code strings or
JSON-serializable values (host callables cannot cross the process boundary)" — is the concrete practical
consequence of choosing isolation: you lose the ability to hand the REPL a live Python closure.

## Connections
- Code concepts: [`rlm-environments-base_env`](../concepts/rlm-environments-base_env.md) — the full grounded
  mechanism; [`rlm-environments-local_repl`](../concepts/rlm-environments-local_repl.md),
  [`rlm-environments-ipython_repl`](../concepts/rlm-environments-ipython_repl.md),
  [`rlm-environments-docker_repl`](../concepts/rlm-environments-docker_repl.md),
  [`rlm-environments-modal_repl`](../concepts/rlm-environments-modal_repl.md),
  [`rlm-environments-prime_repl`](../concepts/rlm-environments-prime_repl.md),
  [`rlm-environments-daytona_repl`](../concepts/rlm-environments-daytona_repl.md),
  [`rlm-environments-e2b_repl`](../concepts/rlm-environments-e2b_repl.md) — the seven concrete backends.
- Module catalogs: [`environments/base_env`](../catalog/rlm/environments/base_env.md)
- Related doc-concepts: [trajectory-logging-and-visualization](trajectory-logging-and-visualization.md)

## Source
Extracted from `README.md` (kept in place).
