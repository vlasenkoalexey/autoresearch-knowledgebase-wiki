---
title: 'Module: packages/coding-agent/src/cli/daemon-stop-confirm.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-stop-confirm.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-stop-confirm.ts`/
symbols:
  confirmDaemonSessionLoss: confirmDaemonSessionLoss().
  pluralizeSessions: pluralizeSessions().
  confirmDaemonSessionLoss.options-typeLiteral15.force: confirmDaemonSessionLoss().(options)typeLiteral15:force.
  confirmDaemonSessionLoss.options-typeLiteral15.copy: confirmDaemonSessionLoss().(options)typeLiteral15:copy.
  DaemonSessionLossCopy: DaemonSessionLossCopy#
  pluralizeSessions.typeLiteral14.noun: pluralizeSessions().typeLiteral14:noun.
  pluralizeSessions.typeLiteral14.pronoun: pluralizeSessions().typeLiteral14:pronoun.
  DaemonSessionLossCopy.busyDetail: DaemonSessionLossCopy#busyDetail().
  DaemonSessionLossCopy.unlistableDetail: DaemonSessionLossCopy#unlistableDetail.
  DaemonSessionLossCopy.question: DaemonSessionLossCopy#question.
  DaemonSessionLossCopy.nonTtyHint: DaemonSessionLossCopy#nonTtyHint.
  promptYesNo: promptYesNo().
---
# Module: [`packages/coding-agent/src/cli/daemon-stop-confirm.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts)

## Classes
### `DaemonSessionLossCopy`
- def: [`packages/coding-agent/src/cli/daemon-stop-confirm.ts:33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L33)
- signature: `interface DaemonSessionLossCopy`
- members:
  - `busyDetail(method)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L35) — Full sentence describing the busy sessions and what stopping the daemon does.
  - `nonTtyHint` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L41) — Remediation appended after the detail when not at a TTY.
  - `question` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L39) — Question appended after the detail when prompting at a TTY (before " [y/N]").
  - `unlistableDetail` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L37) — Full sentence for the reachable-but-unlistable case (work may be lost).
- used by: [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`package-manager-cli.ts`](../package-manager-cli.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-package-manager-cli.ts), [`confirmDaemonSessionLoss`](daemon-stop-confirm.ts.md#confirmDaemonSessionLoss), [`STARTUP_SESSION_LOSS_COPY`](../main.ts.md#STARTUP_SESSION_LOSS_COPY), [`UPDATE_SESSION_LOSS_COPY`](../package-manager-cli.ts.md#UPDATE_SESSION_LOSS_COPY)  (2 test-only)

## Functions
- `confirmDaemonSessionLoss(probe: RunningDaemonProbe, options: { force: boolean; copy: DaemonSessionLossCopy; })` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L51) — Returns true when it is safe to proceed with stopping the daemon: it is not
- `pluralizeSessions(count: number)` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L29)
- `promptYesNo(message: string)` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L18) — Prompt for a yes/no answer at a TTY. Empty/anything-but-yes resolves false (default No).

## Module values
- `copy` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L53)
- `force` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L53)
- `noun` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L29)
- `pronoun` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-stop-confirm.ts#L29)

