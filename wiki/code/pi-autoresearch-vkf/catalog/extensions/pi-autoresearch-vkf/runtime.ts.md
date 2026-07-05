---
title: 'Module: extensions/pi-autoresearch-vkf/runtime.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/runtime.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`runtime.ts`/
symbols:
  resolveRoot: resolveRoot().
  runtimeStore: runtimeStore.
  sessionKey: sessionKey().
  coach: coach().
  Runtime.nudgesSinceProgress: Runtime#nudgesSinceProgress.
  createRuntimeStore: createRuntimeStore().
  Runtime: Runtime#
  Runtime.widgetShown: Runtime#widgetShown.
  Runtime.nudgeSuppressedNotified: Runtime#nudgeSuppressedNotified.
  Runtime.lastFullNoteIteration: Runtime#lastFullNoteIteration.
  Runtime.coachCounts: Runtime#coachCounts.
---
# Module: [`extensions/pi-autoresearch-vkf/runtime.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts)

## Classes
### `Runtime`
- def: [`extensions/pi-autoresearch-vkf/runtime.ts:10`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L10)
- signature: `interface Runtime`
- members:
  - `coachCounts` — [`L20`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L20) — How many times each repeated coaching line has been shown (see {@link coach}).
  - `lastFullNoteIteration` — [`L18`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L18) — Iteration at which the full autonomy paragraph was last emitted.
  - `nudgeSuppressedNotified` — [`L16`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L16) — Whether the user was already told the watchdog gave up (avoid nagging).
  - `nudgesSinceProgress` — [`L14`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L14) — Consecutive watchdog nudges without a new experiment (or plan) since. Reset by vkf_log_experiment / draft_research_plan.
  - `widgetShown` — [`L12`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L12) — Whether the live widget is currently displayed for this session.
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`refreshWidget`](render.ts.md#refreshWidget), [`continuationNote`](index.ts.md#continuationNote), [`coach`](runtime.ts.md#coach), [`createRuntimeStore`](runtime.ts.md#createRuntimeStore)

## Functions
- `coach(rt: Runtime, key: string, line: string, maxTimes?: number)` — [`L61`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L61) — Show a repeated coaching line only the first `maxTimes` a given key is hit
- `createRuntimeStore()` — [`L23`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L23)
- `resolveRoot(ctx: ExtensionContext)` — [`L46`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L46) — Resolve the project root used for `.autoresearch-vkf/session/` and `.autoresearch-vkf/memory/`. Honors — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `sessionKey(ctx: ExtensionContext)` — [`L52`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L52) — Stable per-session key (cwd is sufficient since state is per-project).

## Module values
- `runtimeStore` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/runtime.ts#L40)

