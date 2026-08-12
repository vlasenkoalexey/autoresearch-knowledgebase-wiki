---
title: 'Module: packages/coding-agent/src/modes/interactive/components/tree-selector.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/tree-selector.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`tree-selector.ts`/
symbols:
  TreeList.getEntryDisplayText: TreeList#getEntryDisplayText().
  TreeList.applyFilter: TreeList#applyFilter().
  TreeList.flattenTree: TreeList#flattenTree().
  TreeList.getSearchableText: TreeList#getSearchableText().
  TreeSelectorComponent.-constructor: TreeSelectorComponent#`<constructor>`().
  TreeList.render: TreeList#render().
  TreeSelectorComponent.handleInput: TreeSelectorComponent#handleInput().
  TreeList.getSelectedNode: TreeList#getSelectedNode().
  TreeList.handleInput: TreeList#handleInput().
  TreeList.recalculateVisualStructure: TreeList#recalculateVisualStructure().
  TreeList.-constructor: TreeList#`<constructor>`().
  FlatNode.node: FlatNode#node.
  TreeSelectorComponent.showLabelInput: TreeSelectorComponent#showLabelInput().
  TreeList.filteredNodes: TreeList#filteredNodes.
  TreeList.selectedIndex: TreeList#selectedIndex.
  TreeSelectorComponent.getTreeList: TreeSelectorComponent#getTreeList().
  TreeList.buildActivePath: TreeList#buildActivePath().
  LabelInput.handleInput: LabelInput#handleInput().
  TreeList.findNearestVisibleIndex: TreeList#findNearestVisibleIndex().
  TreeList.findBranchSegmentStart: TreeList#findBranchSegmentStart().
  TreeList.filterMode: TreeList#filterMode.
  TreeList.foldedNodes: TreeList#foldedNodes.
  TreeSelectorComponent.hideLabelInput: TreeSelectorComponent#hideLabelInput().
  TreeList.updateNodeLabel: TreeList#updateNodeLabel().
  LabelInput.render: LabelInput#render().
  TreeSelectorComponent.treeList: TreeSelectorComponent#treeList.
  TreeSelectorComponent.labelInput: TreeSelectorComponent#labelInput.
  LabelInput.-constructor: LabelInput#`<constructor>`().
  SearchLine.render: SearchLine#render().
  TreeSelectorComponent.-set-focused: TreeSelectorComponent#`<set>focused`().
  TreeList.flatNodes: TreeList#flatNodes.
  LabelInput.-set-focused: LabelInput#`<set>focused`().
  TreeList.multipleRoots: TreeList#multipleRoots.
  TreeSelectorComponent: TreeSelectorComponent#
  LabelInput.input: LabelInput#input.
  TreeSelectorComponent.treeContainer: TreeSelectorComponent#treeContainer.
  FlatNode: FlatNode#
  TreeList.searchQuery: TreeList#searchQuery.
  TreeSelectorComponent.labelInputContainer: TreeSelectorComponent#labelInputContainer.
  TreeList.lastSelectedId: TreeList#lastSelectedId.
  TreeList.getStatusLabels: TreeList#getStatusLabels().
  TreeList.isFoldable: TreeList#isFoldable().
  TreeList.maxVisibleLines: TreeList#maxVisibleLines.
  LabelInput: LabelInput#
  FlatNode.gutters: FlatNode#gutters.
  TreeList: TreeList#
  TreeList.toolCallMap: TreeList#toolCallMap.
  GutterInfo: GutterInfo#
  FilterMode: FilterMode#
  TreeList.currentLeafId: TreeList#currentLeafId.
  TreeList.visibleChildrenMap: TreeList#visibleChildrenMap.
  LabelInput.-get-focused: LabelInput#`<get>focused`().
  FlatNode.indent: FlatNode#indent.
  FlatNode.showConnector: FlatNode#showConnector.
  FlatNode.isLast: FlatNode#isLast.
  FlatNode.isVirtualRootChild: FlatNode#isVirtualRootChild.
  TreeList.showLabelTimestamps: TreeList#showLabelTimestamps.
  TreeList.extractContent: TreeList#extractContent().
  TreeList.getSearchQuery: TreeList#getSearchQuery().
  SearchLine.-constructor: SearchLine#`<constructor>`().
  GutterInfo.position: GutterInfo#position.
  GutterInfo.show: GutterInfo#show.
  TreeList.activePathIds: TreeList#activePathIds.
  TreeList.visibleParentMap: TreeList#visibleParentMap.
  TreeList.onSelect: TreeList#onSelect.
  TreeList.onLabelEdit: TreeList#onLabelEdit.
  TreeSelectorComponent._focused: TreeSelectorComponent#_focused.
  SearchLine: SearchLine#
  TreeSelectorComponent.-get-focused: TreeSelectorComponent#`<get>focused`().
  ToolCallInfo.name: ToolCallInfo#name.
  ToolCallInfo.arguments: ToolCallInfo#arguments.
  TreeList.onCancel: TreeList#onCancel.
  LabelInput.entryId: LabelInput#entryId.
  LabelInput.onSubmit: LabelInput#onSubmit.
  LabelInput.onCancel: LabelInput#onCancel.
  LabelInput._focused: LabelInput#_focused.
  TreeSelectorComponent.onLabelChangeCallback: TreeSelectorComponent#onLabelChangeCallback.
  ToolCallInfo: ToolCallInfo#
  TreeList.formatLabelTimestamp: TreeList#formatLabelTimestamp().
  TreeList.hasTextContent: TreeList#hasTextContent().
  TreeList.formatToolCall: TreeList#formatToolCall().
  TreeList.invalidate: TreeList#invalidate().
  SearchLine.invalidate: SearchLine#invalidate().
  SearchLine.handleInput: SearchLine#handleInput().
  LabelInput.invalidate: LabelInput#invalidate().
---
# Module: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts)

## Classes
### `FilterMode`
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L39)
- doc: Filter mode for tree display
- signature: `type FilterMode`
- used by: [`<constructor>`](tree-selector.ts.md#TreeSelectorComponent.-constructor), [`handleInput`](tree-selector.ts.md#TreeList.handleInput), [`<constructor>`](tree-selector.ts.md#TreeList.-constructor), [`filterMode`](tree-selector.ts.md#TreeList.filterMode)

### `FlatNode`
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L24)
- doc: Flattened tree node for navigation
- signature: `interface FlatNode`
- members:
  - `gutters` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L33) — Gutter info for each ancestor branch point
  - `indent` — [`L27`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L27) — Indentation level (each level = 3 chars)
  - `isLast` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L31) — If showConnector, true = last sibling (└─), false = not last (├─)
  - `isVirtualRootChild` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L35) — True if this node is a root under a virtual branching root (multiple roots)
  - `node` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L25)
  - `showConnector` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L29) — Whether to show connector (├─ or └─) - true if parent has multiple children
- uses (calls/refs, reference-scoped): [`AgentConnectionSessionTreeNode`](../../agent-connection/types.ts.md#AgentConnectionSessionTreeNode), [`GutterInfo`](tree-selector.ts.md#GutterInfo)
- used by: [`applyFilter`](tree-selector.ts.md#TreeList.applyFilter), [`flattenTree`](tree-selector.ts.md#TreeList.flattenTree), [`render`](tree-selector.ts.md#TreeList.render), [`getSelectedNode`](tree-selector.ts.md#TreeList.getSelectedNode), [`handleInput`](tree-selector.ts.md#TreeList.handleInput), [`recalculateVisualStructure`](tree-selector.ts.md#TreeList.recalculateVisualStructure), [`<constructor>`](tree-selector.ts.md#TreeList.-constructor), [`filteredNodes`](tree-selector.ts.md#TreeList.filteredNodes), [`buildActivePath`](tree-selector.ts.md#TreeList.buildActivePath), [`findBranchSegmentStart`](tree-selector.ts.md#TreeList.findBranchSegmentStart), [`findNearestVisibleIndex`](tree-selector.ts.md#TreeList.findNearestVisibleIndex), [`updateNodeLabel`](tree-selector.ts.md#TreeList.updateNodeLabel), [`flatNodes`](tree-selector.ts.md#TreeList.flatNodes)

### `GutterInfo`
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L18)
- doc: Gutter info: position (displayIndent where connector was) and whether to show │
- signature: `interface GutterInfo`
- members:
  - `position` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L19)
  - `show` — [`L20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L20)
- used by: [`flattenTree`](tree-selector.ts.md#TreeList.flattenTree), [`render`](tree-selector.ts.md#TreeList.render), [`recalculateVisualStructure`](tree-selector.ts.md#TreeList.recalculateVisualStructure), [`gutters`](tree-selector.ts.md#FlatNode.gutters)

### `LabelInput`  ·  implements/extends Component, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:1071`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1071)
- doc: Label input component shown when editing a label
- signature: `class LabelInput`
- members:
  - `<constructor>(entryId: string, currentLabel: string | undefined)` — [`L1087`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1087) — Label input component shown when editing a label
  - `<get>focused` — [`L1079`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1079) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L1082`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1082) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `handleInput(method)` — [`L1112`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1112) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L1095`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1095) — Invalidate any cached rendering state.
  - `render(method)` — [`L1097`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1097) — Render the component to lines for the given viewport width
  - `entryId` — [`L1073`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1073)
  - `input` — [`L1072`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1072)
  - `onCancel` — [`L1075`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1075)
  - `onSubmit` — [`L1074`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1074)
- protocol/private: `_focused`[`L1078`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1078)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`handleInput`](../../../../../tui/src/components/input.ts.md#Input.handleInput), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`getValue`](../../../../../tui/src/components/input.ts.md#Input.getValue), [`Input`](../../../../../tui/src/components/input.ts.md#Input), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`keyHint`](keybinding-hints.ts.md#keyHint), [`setValue`](../../../../../tui/src/components/input.ts.md#Input.setValue), [`render`](../../../../../tui/src/components/input.ts.md#Input.render), [`focused`](../../../../../tui/src/components/input.ts.md#Input.focused)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`handleInput`](tree-selector.ts.md#TreeSelectorComponent.handleInput), [`showLabelInput`](tree-selector.ts.md#TreeSelectorComponent.showLabelInput), [`labelInput`](tree-selector.ts.md#TreeSelectorComponent.labelInput), [`<set>focused`](tree-selector.ts.md#TreeSelectorComponent.-set-focused)

### `SearchLine`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:1054`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1054)
- doc: Component that displays the current search query
- signature: `class SearchLine`
- members:
  - `<constructor>(treeList: TreeList)` — [`L1055`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1055) — Component that displays the current search query
  - `handleInput(method)` — [`L1067`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1067) — Optional handler for keyboard input when component has focus
  - `invalidate(method)` — [`L1057`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1057) — Invalidate any cached rendering state.
  - `render(method)` — [`L1059`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1059) — Render the component to lines for the given viewport width
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`TreeList`](tree-selector.ts.md#TreeList), [`getSearchQuery`](tree-selector.ts.md#TreeList.getSearchQuery)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`<constructor>`](tree-selector.ts.md#TreeSelectorComponent.-constructor)

### `ToolCallInfo`
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L45)
- doc: Tool call info for lookup
- signature: `interface ToolCallInfo`
- members:
  - `arguments` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L47)
  - `name` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L46)
- used by: [`getEntryDisplayText`](tree-selector.ts.md#TreeList.getEntryDisplayText), [`flattenTree`](tree-selector.ts.md#TreeList.flattenTree), [`toolCallMap`](tree-selector.ts.md#TreeList.toolCallMap)

### `TreeList`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L50)
- signature: `class TreeList`
- members:
  - `<constructor>(tree: AgentConnectionSessionTreeNode[], currentLeafId: string | null, maxVisibleLines: number, initialSelectedId?: string | undefined, initialFilterMode?: FilterMode | undefined)` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L71)
  - `applyFilter(method)` — [`L273`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L273)
  - `buildActivePath(method)` — [`L123`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L123) — Build the set of entry IDs on the path from root to current leaf
  - `extractContent(method)` — [`L830`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L830)
  - `findBranchSegmentStart(method)` — [`L1022`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1022) — Find the index of the next branch segment start in the given direction.
  - `findNearestVisibleIndex(method)` — [`L96`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L96) — Find the index of the nearest visible entry, walking up the parent chain if needed.
  - `flattenTree(method)` — [`L143`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L143)
  - `formatLabelTimestamp(method)` — [`L805`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L805)
  - `formatToolCall(method)` — [`L859`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L859)
  - `getEntryDisplayText(method)` — [`L710`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L710)
  - `getSearchQuery(method)` — [`L571`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L571)
  - `getSearchableText(method)` — [`L505`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L505) — Get searchable text content from a node
  - `getSelectedNode(method)` — [`L575`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L575)
  - `getStatusLabels(method)` — [`L589`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L589)
  - `handleInput(method)` — [`L895`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L895) — Optional handler for keyboard input when component has focus
  - `hasTextContent(method)` — [`L846`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L846)
  - `invalidate(method)` — [`L569`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L569) — Invalidate any cached rendering state.
  - `isFoldable(method)` — [`L1006`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1006) — Whether a node can be folded. A node is foldable if it has visible children
  - `recalculateVisualStructure(method)` — [`L379`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L379) — Recompute indentation/connectors for the filtered view
  - `render(method)` — [`L611`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L611) — Render the component to lines for the given viewport width
  - `updateNodeLabel(method)` — [`L579`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L579)
  - `activePathIds` — [`L61`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L61)
  - `currentLeafId` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L54)
  - `filterMode` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L56)
  - `filteredNodes` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L52)
  - `flatNodes` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L51)
  - `foldedNodes` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L65)
  - `lastSelectedId` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L64)
  - `maxVisibleLines` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L55)
  - `multipleRoots` — [`L59`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L59)
  - `onCancel` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L68)
  - `onLabelEdit` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L69)
  - `onSelect` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L67)
  - `searchQuery` — [`L57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L57)
  - `selectedIndex` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L53)
  - `showLabelTimestamps` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L60)
  - `toolCallMap` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L58)
  - `visibleChildrenMap` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L63)
  - `visibleParentMap` — [`L62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L62)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`role`](../../../../../ai/src/types.ts.md#AssistantMessage.role), [`role`](../../../../../ai/src/types.ts.md#ToolResultMessage.role), [`role`](../../../../../ai/src/types.ts.md#UserMessage.role), [`theme`](../theme/theme.ts.md#theme), [`type`](../../../../../ai/src/types.ts.md#TextContent.type), [`content`](../../../../../ai/src/types.ts.md#AssistantMessage.content), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`role`](../../../core/messages.ts.md#CustomMessage.role), [`role`](../../../core/messages.ts.md#BashExecutionMessage.role), [`role`](../../../core/messages.ts.md#BranchSummaryMessage.role), [`role`](../../../core/messages.ts.md#CompactionSummaryMessage.role), [`content`](../../../../../ai/src/types.ts.md#UserMessage.content), [`content`](../../../../../ai/src/types.ts.md#ToolResultMessage.content), [`type`](../../../../../ai/src/types.ts.md#ImageContent.type), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`input`](../../../../../ai/src/types.ts.md#Usage.input), [`matches`](../../../../../tui/src/keybindings.ts.md#KeybindingsManager.matches), [`output`](../../../../../ai/src/types.ts.md#Usage.output), [`cacheRead`](../../../../../ai/src/types.ts.md#Usage.cacheRead), [`cacheWrite`](../../../../../ai/src/types.ts.md#Usage.cacheWrite), [`content`](../../../core/messages.ts.md#CustomMessage.content), [`entry`](../../agent-connection/types.ts.md#AgentConnectionSessionTreeFlatNode.entry), [`id`](../../agent-connection/types.ts.md#AgentConnectionSessionEntryBase.id), [`bold`](../theme/theme.ts.md#Theme.bold), [`getKeybindings`](../../../../../tui/src/keybindings.ts.md#getKeybindings), [`getSelectionBackgroundColor`](../theme/theme.ts.md#Theme.getSelectionBackgroundColor), [`node`](tree-selector.ts.md#FlatNode.node), [`AgentConnectionSessionTreeNode`](../../agent-connection/types.ts.md#AgentConnectionSessionTreeNode), [`type`](../../agent-connection/types.ts.md#AgentConnectionSessionMessageEntry.type), [`parentId`](../../agent-connection/types.ts.md#AgentConnectionSessionEntryBase.parentId), [`type`](../../agent-connection/types.ts.md#AgentConnectionAgentStatusEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionBranchSummaryEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionCompactionEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionCustomMessageEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionGitStateEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionSessionStateEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionChildUsageAttributionEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionServiceTierChangeEntry.type), [`type`](../../agent-connection/types.ts.md#AgentConnectionSessionInfoEntry.type)  (+34 more)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`<constructor>`](tree-selector.ts.md#TreeSelectorComponent.-constructor), [`handleInput`](tree-selector.ts.md#TreeSelectorComponent.handleInput), [`showLabelInput`](tree-selector.ts.md#TreeSelectorComponent.showLabelInput), [`getTreeList`](tree-selector.ts.md#TreeSelectorComponent.getTreeList), [`treeList`](tree-selector.ts.md#TreeSelectorComponent.treeList), [`render`](tree-selector.ts.md#SearchLine.render), [`<constructor>`](tree-selector.ts.md#SearchLine.-constructor)  (1 test-only)

### `TreeSelectorComponent`  ·  implements/extends Component, Container, Focusable
- def: [`packages/coding-agent/src/modes/interactive/components/tree-selector.ts:1128`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1128)
- doc: Component that renders a session tree selector for navigation
- signature: `class TreeSelectorComponent`
- members:
  - `<constructor>(tree: AgentConnectionSessionTreeNode[], currentLeafId: string | null, terminalHeight: number, onSelect: (entryId: string) => void, onCancel: () => void, onLabelChange?: ((entryId: string, label: string | undefined) => void) | undefined, initialSelectedId?: string | undefined, initialFilterMode?: FilterMode | undefined)` — [`L1148`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1148) — Component that renders a session tree selector for navigation
  - `<get>focused` — [`L1137`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1137) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `<set>focused` — [`L1140`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1140) — Set by TUI when focus changes. Component should emit CURSOR_MARKER when true.
  - `getTreeList(method)` — [`L1239`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1239)
  - `handleInput(method)` — [`L1231`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1231)
  - `hideLabelInput(method)` — [`L1224`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1224)
  - `showLabelInput(method)` — [`L1207`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1207)
  - `labelInput` — [`L1130`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1130)
  - `labelInputContainer` — [`L1131`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1131)
  - `onLabelChangeCallback` — [`L1133`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1133)
  - `treeContainer` — [`L1132`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1132)
  - `treeList` — [`L1129`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1129)
- protocol/private: `_focused`[`L1136`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/tree-selector.ts#L1136)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`addChild`](../../../../../tui/src/tui.ts.md#Container.addChild), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`<constructor>`](../../../../../tui/src/components/spacer.ts.md#Spacer.-constructor), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`keyText`](keybinding-hints.ts.md#keyText), [`bold`](../theme/theme.ts.md#Theme.bold), [`clear`](../../../../../tui/src/tui.ts.md#Container.clear), [`handleInput`](tree-selector.ts.md#TreeList.handleInput), [`<constructor>`](tree-selector.ts.md#TreeList.-constructor), [`<constructor>`](dynamic-border.ts.md#DynamicBorder.-constructor), [`AgentConnectionSessionTreeNode`](../../agent-connection/types.ts.md#AgentConnectionSessionTreeNode), [`<constructor>`](../../../../../tui/src/components/truncated-text.ts.md#TruncatedText.-constructor), [`handleInput`](tree-selector.ts.md#LabelInput.handleInput), [`updateNodeLabel`](tree-selector.ts.md#TreeList.updateNodeLabel), [`<constructor>`](tree-selector.ts.md#LabelInput.-constructor), [`<set>focused`](tree-selector.ts.md#LabelInput.-set-focused), [`LabelInput`](tree-selector.ts.md#LabelInput), [`TreeList`](tree-selector.ts.md#TreeList), [`FilterMode`](tree-selector.ts.md#FilterMode), [`<get>focused`](tree-selector.ts.md#LabelInput.-get-focused), [`<constructor>`](tree-selector.ts.md#SearchLine.-constructor), [`onLabelEdit`](tree-selector.ts.md#TreeList.onLabelEdit), [`onSelect`](tree-selector.ts.md#TreeList.onSelect), [`onCancel`](tree-selector.ts.md#LabelInput.onCancel), [`onCancel`](tree-selector.ts.md#TreeList.onCancel), [`onSubmit`](tree-selector.ts.md#LabelInput.onSubmit)
- used by: [`index.ts`](../../../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`Container`](../../../../../tui/src/tui.ts.md#Container), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`handleInput`](../../../../../tui/src/tui.ts.md#Component.handleInput), [`Focusable`](../../../../../tui/src/tui.ts.md#Focusable), [`showTreeSelector`](../interactive-mode.ts.md#InteractiveMode.showTreeSelector)  (1 test-only)

