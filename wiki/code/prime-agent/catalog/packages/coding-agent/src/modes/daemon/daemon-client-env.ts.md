---
title: 'Module: packages/coding-agent/src/modes/daemon/daemon-client-env.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/daemon/daemon-client-env.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/daemon/`daemon-client-env.ts`/
symbols:
  withClientEnv: withClientEnv().
  execEnvForSession: execEnvForSession().
  filterClientEnv: filterClientEnv().
  baseClientEnv: baseClientEnv.
  lastExclusive: lastExclusive.
  activeShared: activeShared.
---
# Module: [`packages/coding-agent/src/modes/daemon/daemon-client-env.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts)

## Functions
- `execEnvForSession(clientEnv?: Record<string, string> | undefined)` — [`L30`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L30) — Exec env for a session's subprocesses: pins every allowlisted key to the
- `filterClientEnv(env?: Record<string, string> | undefined)` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L4) — Re-filter client-sent env to the allowlist; the socket peer is untrusted.
- `withClientEnv(env: Record<string, string> | undefined, fn: () => Promise<T>)` — [`L51`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L51) — Run fn with the client's env applied to process.env, restoring afterwards.

## Module values
- `activeShared` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L43)
- `baseClientEnv` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L19)
- `lastExclusive` — [`L42`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/daemon/daemon-client-env.ts#L42)

