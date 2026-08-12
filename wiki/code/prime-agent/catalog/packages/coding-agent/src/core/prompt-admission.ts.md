---
title: 'Module: packages/coding-agent/src/core/prompt-admission.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/prompt-admission.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`prompt-admission.ts`/
symbols:
  waitForPromptAdmission: waitForPromptAdmission().
  throwIfPromptAdmissionCancelled: throwIfPromptAdmissionCancelled().
  PromptAdmissionCancelledError: PromptAdmissionCancelledError#
  PromptAdmissionCancelledError.-constructor: PromptAdmissionCancelledError#`<constructor>`().
---
# Module: [`packages/coding-agent/src/core/prompt-admission.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-admission.ts)

## Classes
### `PromptAdmissionCancelledError`  ·  implements/extends Error
- def: [`packages/coding-agent/src/core/prompt-admission.ts:1`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-admission.ts#L1)
- signature: `class PromptAdmissionCancelledError`
- members:
  - `<constructor>()` — [`L2`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-admission.ts#L2)
- used by: [`handleCommand`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleCommand), [`daemon-mode.ts`](../modes/daemon/daemon-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-mode.ts), [`daemon-supervisor.ts`](../modes/daemon/daemon-supervisor.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-daemon-daemon-supervisor.ts), [`handleLine`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.handleLine), [`waitForPromptAdmission`](prompt-admission.ts.md#waitForPromptAdmission), [`throwIfAdmissionCancelled`](../modes/daemon/daemon-supervisor.ts.md#throwIfAdmissionCancelled), [`throwIfPromptAdmissionCancelled`](prompt-admission.ts.md#throwIfPromptAdmissionCancelled)  (1 test-only)

## Functions
- `throwIfPromptAdmissionCancelled(signal: AbortSignal | undefined)` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-admission.ts#L8)
- `waitForPromptAdmission(promise: Promise<T>, signal: AbortSignal | undefined)` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompt-admission.ts#L16) — Await `promise` unless `signal` aborts first. Always observes the supplied

