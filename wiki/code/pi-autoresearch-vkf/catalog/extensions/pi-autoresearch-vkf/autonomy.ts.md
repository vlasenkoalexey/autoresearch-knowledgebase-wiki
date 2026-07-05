---
title: 'Module: extensions/pi-autoresearch-vkf/autonomy.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/autonomy.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`autonomy.ts`/
symbols:
  shouldContinue: shouldContinue().
  nudgeMessage: nudgeMessage().
  AutonomySnapshot.sessionMode: AutonomySnapshot#sessionMode.
  AutonomySnapshot.maxIterations: AutonomySnapshot#maxIterations.
  AutonomySnapshot.autonomy: AutonomySnapshot#autonomy.
  wantFullNote: wantFullNote().
  AutonomySnapshot: AutonomySnapshot#
  AutonomySnapshot.iterations: AutonomySnapshot#iterations.
  AutonomySnapshot.loopEngaged: AutonomySnapshot#loopEngaged.
  AutonomySnapshot.stopFileExists: AutonomySnapshot#stopFileExists.
  AutonomySnapshot.planWritten: AutonomySnapshot#planWritten.
  AutonomySnapshot.nudgesSinceProgress: AutonomySnapshot#nudgesSinceProgress.
  MAX_NUDGES_WITHOUT_PROGRESS: MAX_NUDGES_WITHOUT_PROGRESS.
  FULL_NOTE_EVERY: FULL_NOTE_EVERY.
  ContinueDecision: ContinueDecision#
---
# Module: [`extensions/pi-autoresearch-vkf/autonomy.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts)

## Classes
### `AutonomySnapshot`
- def: [`extensions/pi-autoresearch-vkf/autonomy.ts:20`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L20) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- signature: `interface AutonomySnapshot`
- members:
  - `autonomy` — [`L21`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L21) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `iterations` — [`L28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L28) — Experiments logged so far (the iteration counter). — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `loopEngaged` — [`L25`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L25) — Whether the just-ended agent run actually used the research tools. An — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `maxIterations` — [`L29`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L29) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `nudgesSinceProgress` — [`L33`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L33) — Consecutive nudges since the last new experiment / plan. — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `planWritten` — [`L31`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L31) — Ideation sessions: whether research_plan.md (the deliverable) exists. — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `sessionMode` — [`L22`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L22) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
  - `stopFileExists` — [`L26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L26) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- uses (calls/refs, reference-scoped): [`AutonomyMode`](config.ts.md#AutonomyMode), [`SessionMode`](config.ts.md#SessionMode)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`shouldContinue`](autonomy.ts.md#shouldContinue), [`nudgeMessage`](autonomy.ts.md#nudgeMessage)

### `ContinueDecision`
- def: [`extensions/pi-autoresearch-vkf/autonomy.ts:36`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L36) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- signature: `type ContinueDecision`
- used by: [`shouldContinue`](autonomy.ts.md#shouldContinue)

## Functions
- `nudgeMessage(s: AutonomySnapshot, sessionName: string)` — [`L60`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L60) — The short follow-up prompt the watchdog injects. Deliberately ~40 tokens. — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- `shouldContinue(s: AutonomySnapshot, sessionName: string)` — [`L44`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L44) — Decide whether the watchdog should re-prompt the agent after it ended its — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- `wantFullNote(lastFullAtIteration: number | undefined, iteration: number)` — [`L78`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L78) — Whether the long autonomy paragraph is due, vs the one-line brief. Full text

## Module values
- `FULL_NOTE_EVERY` — [`L18`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L18) — Re-emit the full autonomy paragraph every this many iterations (else one line).
- `MAX_NUDGES_WITHOUT_PROGRESS` — [`L15`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/autonomy.ts#L15) — Stop nudging after this many auto-continues that produced no new experiment. — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)

