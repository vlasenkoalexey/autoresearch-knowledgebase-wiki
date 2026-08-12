---
title: 'Module: packages/coding-agent/src/core/event-bus.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/event-bus.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`event-bus.ts`/
symbols:
  createEventBus: createEventBus().
  EventBus: EventBus#
  EventBusController: EventBusController#
  EventBus.emit: EventBus#emit().
  EventBus.on: EventBus#on().
  EventBusController.clear: EventBusController#clear().
---
# Module: [`packages/coding-agent/src/core/event-bus.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts)

## Classes
### `EventBus`
- def: [`packages/coding-agent/src/core/event-bus.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L3)
- signature: `interface EventBus`
- members:
  - `emit(method)` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L4)
  - `on(method)` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L5)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`createExtensionAPI`](extensions/loader.ts.md#createExtensionAPI), [`resource-loader.ts`](resource-loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-resource-loader.ts), [`discoverAndLoadExtensions`](extensions/loader.ts.md#discoverAndLoadExtensions), [`loader.ts`](extensions/loader.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-loader.ts), [`herdrAgentStateExtensionImpl`](extensions/builtin/herdr-agent-state.ts.md#herdrAgentStateExtensionImpl), [`loadExtensions`](extensions/loader.ts.md#loadExtensions), [`loadExtensionFromFactory`](extensions/loader.ts.md#loadExtensionFromFactory), [`createEventBus`](event-bus.ts.md#createEventBus), [`events`](extensions/types.ts.md#ExtensionAPI.events), [`loadExtension`](extensions/loader.ts.md#loadExtension), [`EventBusController`](event-bus.ts.md#EventBusController), [`eventBus`](resource-loader.ts.md#DefaultResourceLoader.eventBus), [`eventBus`](resource-loader.ts.md#DefaultResourceLoaderOptions.eventBus)  (1 test-only)

### `EventBusController`
- def: [`packages/coding-agent/src/core/event-bus.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L8)
- signature: `interface EventBusController`
- members:
  - `clear(method)` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L9)
- uses (calls/refs, reference-scoped): [`EventBus`](event-bus.ts.md#EventBus)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`createEventBus`](event-bus.ts.md#createEventBus)

## Functions
- `createEventBus()` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/event-bus.ts#L12)

