---
title: 'Module: packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`heartbeat-manager.ts`/
symbols:
  HeartbeatManagerComponent.createActionPanel: HeartbeatManagerComponent#createActionPanel().
  HeartbeatManagerComponent.populateHeartbeatList: HeartbeatManagerComponent#populateHeartbeatList().
  HeartbeatManagerComponent.createHeartbeatListPanel: HeartbeatManagerComponent#createHeartbeatListPanel().
  HeartbeatManagerComponent.getListLayout: HeartbeatManagerComponent#getListLayout().
  HeartbeatManagerComponent.handleInput: HeartbeatManagerComponent#handleInput().
  HeartbeatManagerComponent.setHeartbeats: HeartbeatManagerComponent#setHeartbeats().
  HeartbeatManagerComponent.formatHeartbeatDetails: HeartbeatManagerComponent#formatHeartbeatDetails().
  HeartbeatManagerComponent.confirmSelection: HeartbeatManagerComponent#confirmSelection().
  HeartbeatManagerComponent.heartbeats: HeartbeatManagerComponent#heartbeats.
  HeartbeatManagerComponent.mode: HeartbeatManagerComponent#mode.
  HeartbeatManagerComponent.sessionLabel: HeartbeatManagerComponent#sessionLabel().
  HeartbeatManagerComponent.runAction: HeartbeatManagerComponent#runAction().
  HeartbeatManagerComponent.availableActions.Array.typeLiteral116.action: HeartbeatManagerComponent#availableActions().Array:typeLiteral116:action.
  HeartbeatManagerComponent.moveSelection: HeartbeatManagerComponent#moveSelection().
  HeartbeatManagerComponent.render: HeartbeatManagerComponent#render().
  HeartbeatManagerComponent.findHeartbeat: HeartbeatManagerComponent#findHeartbeat().
  HeartbeatManagerComponent.formatStatus: HeartbeatManagerComponent#formatStatus().
  HeartbeatManagerComponent.-constructor: HeartbeatManagerComponent#`<constructor>`().
  HeartbeatManagerOptions.requestRender: HeartbeatManagerOptions#requestRender.
  HeartbeatManagerOptions.onAction: HeartbeatManagerOptions#onAction.
  HeartbeatManagerComponent.sourceLabel: HeartbeatManagerComponent#sourceLabel().
  HeartbeatManagerComponent.defaultHeartbeatName: HeartbeatManagerComponent#defaultHeartbeatName().
  HeartbeatManagerComponent.selectedIndex: HeartbeatManagerComponent#selectedIndex.
  HeartbeatManagerComponent: HeartbeatManagerComponent#
  HeartbeatManagerComponent.error: HeartbeatManagerComponent#error.
  HeartbeatManagerOptions.onClose: HeartbeatManagerOptions#onClose.
  HeartbeatManagerComponent.availableActions: HeartbeatManagerComponent#availableActions().
  HeartbeatManagerOptions.getRows: HeartbeatManagerOptions#getRows.
  HeartbeatManagerComponent.availableActions.Array.typeLiteral116.label: HeartbeatManagerComponent#availableActions().Array:typeLiteral116:label.
  HeartbeatManagerComponent.singleLine: HeartbeatManagerComponent#singleLine().
  HeartbeatManagerComponent.closeHint: HeartbeatManagerComponent#closeHint().
  HeartbeatManagerComponent.detailHint: HeartbeatManagerComponent#detailHint().
  HeartbeatManagerComponent.actionDescription: HeartbeatManagerComponent#actionDescription().
  HeartbeatManagerComponent.busy: HeartbeatManagerComponent#busy.
  HeartbeatManagerComponent.-get-focused: HeartbeatManagerComponent#`<get>focused`().
  HeartbeatManagerComponent.-set-focused: HeartbeatManagerComponent#`<set>focused`().
  HeartbeatManagerMode: HeartbeatManagerMode#
  HeartbeatManagerComponent._focused: HeartbeatManagerComponent#_focused.
  HEARTBEAT_PANEL_MAX_WIDTH: HEARTBEAT_PANEL_MAX_WIDTH.
  PREFERRED_VISIBLE_HEARTBEATS: PREFERRED_VISIBLE_HEARTBEATS.
  HEARTBEAT_LIST_RESERVED_ROWS: HEARTBEAT_LIST_RESERVED_ROWS.
  HEARTBEAT_SCROLL_INDICATOR_ROWS: HEARTBEAT_SCROLL_INDICATOR_ROWS.
  HeartbeatManagerOptions: HeartbeatManagerOptions#
  HeartbeatManagerComponent.formatTimestamp: HeartbeatManagerComponent#formatTimestamp().
  HeartbeatManagerComponent.invalidate: HeartbeatManagerComponent#invalidate().
  HeartbeatManagerComponent.createActionPanel.mode-Exclude.typeLiteral97.type: HeartbeatManagerComponent#createActionPanel().(mode)Exclude:typeLiteral97:type.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts)

## Classes
### `HeartbeatManagerComponent`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts:23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L23)
- signature: `class HeartbeatManagerComponent`
- members:
  - `<constructor>(heartbeats: readonly AgentConnectionHeartbeat[], options: HeartbeatManagerOptions)` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L31)
  - `<get>focused` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L38) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L42`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L42) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `actionDescription(method)` — [`L303`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L303)
  - `availableActions(method)` — [`L245`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L245)
  - `closeHint(method)` — [`L295`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L295)
  - `confirmSelection(method)` — [`L210`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L210)
  - `createActionPanel(method)` — [`L167`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L167)
  - `createHeartbeatListPanel(method)` — [`L109`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L109)
  - `defaultHeartbeatName(method)` — [`L291`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L291)
  - `detailHint(method)` — [`L299`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L299)
  - `findHeartbeat(method)` — [`L257`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L257)
  - `formatHeartbeatDetails(method)` — [`L281`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L281)
  - `formatStatus(method)` — [`L277`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L277)
  - `formatTimestamp(method)` — [`L318`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L318)
  - `getListLayout(method)` — [`L265`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L265)
  - `handleInput(method)` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L66) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L46) — Invalidate any cached rendering state.
  - `moveSelection(method)` — [`L199`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L199)
  - `populateHeartbeatList(method)` — [`L129`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L129)
  - `render(method)` — [`L100`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L100) — Render the component to lines for the given viewport width
  - `runAction(method)` — [`L230`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L230)
  - `sessionLabel(method)` — [`L261`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L261)
  - `setHeartbeats(method)` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L48)
  - `singleLine(method)` — [`L314`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L314)
  - `sourceLabel(method)` — [`L287`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L287)
  - `action` — [`L247`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L247)
  - `busy` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L27)
  - `error` — [`L28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L28)
  - `heartbeats` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L24)
  - `label` — [`L247`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L247)
  - `mode` — [`L26`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L26)
  - `selectedIndex` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L25)
  - `type` — [`L167`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L167)
- protocol/private: `_focused`[`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L29)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`id`](../../../core/cron-jobs.ts.md#AgentCronJob.id), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`status`](../../../core/cron-jobs.ts.md#AgentCronJob.status), [`AgentConnectionHeartbeat`](../../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`job`](../../agent-connection/types.ts.md#AgentConnectionHeartbeat.job), [`nextRunAt`](../../../core/cron-jobs.ts.md#AgentCronJob.nextRunAt), [`source`](../../../core/cron-jobs.ts.md#AgentCronJob.source), [`getMenuListLayout`](menu-panel.ts.md#getMenuListLayout), [`keyHint`](keybinding-hints.ts.md#keyHint), [`schedule`](../../../core/cron-jobs.ts.md#AgentCronJob.schedule), [`prompt`](../../../core/cron-jobs.ts.md#AgentCronJob.prompt), [`<constructor>`](../../../../../tui/src/components/truncated-text.ts.md#TruncatedText.-constructor), [`render`](menu-panel.ts.md#MenuPanel.render), [`sessionId`](../../../core/cron-jobs.ts.md#AgentCronJob.sessionId), [`AgentHeartbeatManagementAction`](../../../core/cron-jobs.ts.md#AgentHeartbeatManagementAction), [`visibleItems`](menu-panel.ts.md#MenuListLayout.visibleItems), [`runCount`](../../../core/cron-jobs.ts.md#AgentCronJob.runCount), [`expression`](../../../core/cron-jobs.ts.md#AgentCronSchedule.expression), [`deliveryMode`](../../../core/cron-jobs.ts.md#AgentCronJob.deliveryMode), [`createdAt`](../../../core/cron-jobs.ts.md#AgentCronJob.createdAt), [`compact`](menu-panel.ts.md#MenuListLayout.compact), [`<constructor>`](menu-panel.ts.md#MenuPanel.-constructor), [`getRows`](menu-panel.ts.md#MenuViewportProvider.getRows), [`shouldTreatAsBack`](modal-back.ts.md#shouldTreatAsBack), [`reservedRows`](menu-panel.ts.md#MenuListLayoutOptions.reservedRows), [`compactItemRows`](menu-panel.ts.md#MenuListLayoutOptions.compactItemRows), [`preferredVisibleItems`](menu-panel.ts.md#MenuListLayoutOptions.preferredVisibleItems), [`MenuPanel`](menu-panel.ts.md#MenuPanel), [`<constructor>`](menu-panel.ts.md#MenuRow.-constructor), [`MenuList`](menu-panel.ts.md#MenuList), [`comfortableItemRows`](menu-panel.ts.md#MenuListLayoutOptions.comfortableItemRows), [`primary`](menu-panel.ts.md#MenuRowOptions.primary), [`selected`](menu-panel.ts.md#MenuRowOptions.selected)  (+21 more)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showHeartbeatManager`](../interactive-mode.ts.md#InteractiveMode.showHeartbeatManager), [`updateScopedHeartbeats`](../interactive-mode.ts.md#InteractiveMode.updateScopedHeartbeats), [`heartbeatManager`](../interactive-mode.ts.md#InteractiveMode.heartbeatManager)  (1 test-only)

### `HeartbeatManagerMode`
- def: [`packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts:14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L14)
- signature: `type HeartbeatManagerMode`
- used by: [`createActionPanel`](heartbeat-manager.ts.md#HeartbeatManagerComponent.createActionPanel), [`mode`](heartbeat-manager.ts.md#HeartbeatManagerComponent.mode)

### `HeartbeatManagerOptions`
- def: [`packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts:16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L16)
- signature: `interface HeartbeatManagerOptions`
- members:
  - `getRows` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L17)
  - `onAction` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L18)
  - `onClose` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L19)
  - `requestRender` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L20)
- uses (calls/refs, reference-scoped): [`AgentConnectionHeartbeat`](../../agent-connection/types.ts.md#AgentConnectionHeartbeat), [`AgentHeartbeatManagementAction`](../../../core/cron-jobs.ts.md#AgentHeartbeatManagementAction)
- used by: [`showHeartbeatManager`](../interactive-mode.ts.md#InteractiveMode.showHeartbeatManager), [`getListLayout`](heartbeat-manager.ts.md#HeartbeatManagerComponent.getListLayout), [`handleInput`](heartbeat-manager.ts.md#HeartbeatManagerComponent.handleInput), [`setHeartbeats`](heartbeat-manager.ts.md#HeartbeatManagerComponent.setHeartbeats), [`confirmSelection`](heartbeat-manager.ts.md#HeartbeatManagerComponent.confirmSelection), [`runAction`](heartbeat-manager.ts.md#HeartbeatManagerComponent.runAction), [`moveSelection`](heartbeat-manager.ts.md#HeartbeatManagerComponent.moveSelection), [`<constructor>`](heartbeat-manager.ts.md#HeartbeatManagerComponent.-constructor)  (1 test-only)

## Module values
- `HEARTBEAT_LIST_RESERVED_ROWS` — [`L11`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L11)
- `HEARTBEAT_PANEL_MAX_WIDTH` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L9)
- `HEARTBEAT_SCROLL_INDICATOR_ROWS` — [`L12`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L12)
- `PREFERRED_VISIBLE_HEARTBEATS` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/heartbeat-manager.ts#L10)

