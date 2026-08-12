---
title: 'Module: packages/coding-agent/src/modes/interactive/components/ipython-cell.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/ipython-cell.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`ipython-cell.ts`/
symbols:
  IPythonCellComponent.render: IPythonCellComponent#render().
  IPythonCellComponent.renderOutput: IPythonCellComponent#renderOutput().
  IPythonCellComponent.collapsedLine: IPythonCellComponent#collapsedLine().
  IPythonCellComponent.renderFileDiff: IPythonCellComponent#renderFileDiff().
  IPythonCellState.expanded: IPythonCellState#expanded.
  IPythonCellComponent.renderSentAgentMessages: IPythonCellComponent#renderSentAgentMessages().
  IPythonCellState.code: IPythonCellState#code.
  IPythonCellState.executionStarted: IPythonCellState#executionStarted.
  readDetails: readDetails().
  IPythonCellComponent.-constructor: IPythonCellComponent#`<constructor>`().
  IPythonCellComponent.state: IPythonCellComponent#state.
  IPythonCellComponent.lineCounts: IPythonCellComponent#lineCounts().
  IPythonCellState.details: IPythonCellState#details.
  IPythonCellState.argsComplete: IPythonCellState#argsComplete.
  readSentAgentMessages: readSentAgentMessages().
  IPythonCellComponent.hasResult: IPythonCellComponent#hasResult().
  IPythonCellComponent.renderCode: IPythonCellComponent#renderCode().
  IPythonCellComponent.statusKind: IPythonCellComponent#statusKind().
  IPythonCellComponent.addWrapped: IPythonCellComponent#addWrapped().
  IPythonCellComponent.marker: IPythonCellComponent#marker().
  formatIpythonErrorSummary: formatIpythonErrorSummary().
  IPythonCellState.content: IPythonCellState#content.
  IPythonCellComponent.renderOutputText: IPythonCellComponent#renderOutputText().
  IPythonCellComponent: IPythonCellComponent#
  IPythonCellComponent.highlightInputLine: IPythonCellComponent#highlightInputLine().
  readDiffDisplays: readDiffDisplays().
  IPythonCellComponent.update: IPythonCellComponent#update().
  IPythonCellContentBlock.type: IPythonCellContentBlock#type.
  IPythonCellContentBlock.text: IPythonCellContentBlock#text.
  IPythonCellState: IPythonCellState#
  IPythonCellComponent.renderTraceback: IPythonCellComponent#renderTraceback().
  isAgentMessageReceipt: isAgentMessageReceipt().
  isImageBlock: isImageBlock().
  IPythonCellComponent.renderDiffs: IPythonCellComponent#renderDiffs().
  IpythonDetails.error: IpythonDetails#error.
  IpythonDetails.sentAgentMessages: IpythonDetails#sentAgentMessages.
  isEditConfirmation: isEditConfirmation().
  textFromBlocks: textFromBlocks().
  IpythonDetails.result: IpythonDetails#result.
  IpythonDetails.diffs: IpythonDetails#diffs.
  splitTraceback: splitTraceback().
  IPythonCellState.isError: IPythonCellState#isError.
  DiffDisplay: DiffDisplay#
  IpythonDetails: IpythonDetails#
  IpythonDetails.stdout: IpythonDetails#stdout.
  OUTPUT_INDENT: OUTPUT_INDENT.
  IPythonCellComponent.invalidate: IPythonCellComponent#invalidate().
  IPythonCellComponent.renderCache: IPythonCellComponent#renderCache.
  IPythonCellState.isPartial: IPythonCellState#isPartial.
  IpythonDetails.stderr: IpythonDetails#stderr.
  IpythonErrorDetails.ename: IpythonErrorDetails#ename.
  SentAgentMessageDisplay: SentAgentMessageDisplay#
  IPythonCellContentBlock: IPythonCellContentBlock#
  DiffDisplay.path: DiffDisplay#path.
  IPythonCellComponent.addBlank: IPythonCellComponent#addBlank().
  IPythonCellComponent.addPlain: IPythonCellComponent#addPlain().
  closeOpenSgr: closeOpenSgr().
  readErrorDetails: readErrorDetails().
  displayEditPath: displayEditPath().
  IPythonCellState.cwd: IPythonCellState#cwd.
  SentAgentMessageDisplay.id: SentAgentMessageDisplay#id.
  SentAgentMessageDisplay.message: SentAgentMessageDisplay#message.
  IpythonDetails.status: IpythonDetails#status.
  IpythonDetails.errorEname: IpythonDetails#errorEname.
  IpythonErrorDetails: IpythonErrorDetails#
  getIpythonCodeFromArgs: getIpythonCodeFromArgs().
  IPythonCellComponent.stateVersion: IPythonCellComponent#stateVersion.
  IPythonCellState.showImages: IPythonCellState#showImages.
  DiffDisplay.oldStr: DiffDisplay#oldStr.
  DiffDisplay.newStr: DiffDisplay#newStr.
  DiffDisplay.startLine: DiffDisplay#startLine.
  SentAgentMessageDisplay.deliveryStatus: SentAgentMessageDisplay#deliveryStatus.
  SentAgentMessageDisplay.receiverRole: SentAgentMessageDisplay#receiverRole.
  SentAgentMessageDisplay.target: SentAgentMessageDisplay#target.
  IpythonDetails.durationMs: IpythonDetails#durationMs.
  TracebackParts.output: TracebackParts#output.
  stripReprQuotes: stripReprQuotes().
  IPythonCellContentBlock.data: IPythonCellContentBlock#data.
  IPythonCellContentBlock.mimeType: IPythonCellContentBlock#mimeType.
  IPythonCellState.showExpandHint: IPythonCellState#showExpandHint.
  SentAgentMessageDisplay.target.typeLiteral0.activeSessionId: SentAgentMessageDisplay#target.typeLiteral0:activeSessionId.
  SentAgentMessageDisplay.target.typeLiteral0.sessionId: SentAgentMessageDisplay#target.typeLiteral0:sessionId.
  SentAgentMessageDisplay.target.typeLiteral0.sessionName: SentAgentMessageDisplay#target.typeLiteral0:sessionName.
  IpythonErrorDetails.evalue: IpythonErrorDetails#evalue.
  IpythonErrorDetails.traceback: IpythonErrorDetails#traceback.
  TracebackParts: TracebackParts#
  TracebackParts.traceback: TracebackParts#traceback.
  MAGIC_LINE_PATTERN: MAGIC_LINE_PATTERN.
  SGR_PATTERN: SGR_PATTERN.
  formatDuration: formatDuration().
  TracebackParts.preview: TracebackParts#preview.
---
# Module: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts)

## Classes
### `DiffDisplay`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:43`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L43)
- signature: `interface DiffDisplay`
- members:
  - `newStr` — [`L46`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L46)
  - `oldStr` — [`L45`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L45)
  - `path` — [`L44`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L44)
  - `startLine` — [`L47`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L47)
- used by: [`renderFileDiff`](ipython-cell.ts.md#IPythonCellComponent.renderFileDiff), [`readDiffDisplays`](ipython-cell.ts.md#readDiffDisplays), [`renderDiffs`](ipython-cell.ts.md#IPythonCellComponent.renderDiffs), [`isEditConfirmation`](ipython-cell.ts.md#isEditConfirmation), [`diffs`](ipython-cell.ts.md#IpythonDetails.diffs)

### `IPythonCellComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:345`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L345)
- signature: `class IPythonCellComponent`
- members:
  - `<constructor>(state: IPythonCellState)` — [`L350`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L350)
  - `addBlank(method)` — [`L741`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L741)
  - `addPlain(method)` — [`L746`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L746)
  - `addWrapped(method)` — [`L731`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L731)
  - `collapsedLine(method)` — [`L400`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L400)
  - `hasResult(method)` — [`L497`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L497)
  - `highlightInputLine(method)` — [`L530`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L530)
  - `invalidate(method)` — [`L359`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L359) — Invalidate any cached rendering state.
  - `lineCounts(method)` — [`L452`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L452)
  - `marker(method)` — [`L435`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L435) — Status marker — color carries running/done/error; ✓/✗ once finished.
  - `render(method)` — [`L363`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L363) — Render the component to lines for the given viewport width
  - `renderCode(method)` — [`L510`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L510)
  - `renderDiffs(method)` — [`L666`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L666)
  - `renderFileDiff(method)` — [`L679`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L679)
  - `renderOutput(method)` — [`L539`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L539)
  - `renderOutputText(method)` — [`L717`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L717)
  - `renderSentAgentMessages(method)` — [`L642`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L642)
  - `renderTraceback(method)` — [`L724`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L724)
  - `statusKind(method)` — [`L478`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L478)
  - `update(method)` — [`L354`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L354)
  - `renderCache` — [`L346`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L346)
  - `state` — [`L347`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L347)
  - `stateVersion` — [`L348`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L348)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`truncateToWidth`](../../../../../tui/src/utils.ts.md#truncateToWidth), [`wrapTextWithAnsi`](../../../../../tui/src/utils.ts.md#wrapTextWithAnsi), [`renderRichDiff`](diff.ts.md#renderRichDiff), [`expanded`](ipython-cell.ts.md#IPythonCellState.expanded), [`code`](ipython-cell.ts.md#IPythonCellState.code), [`executionStarted`](ipython-cell.ts.md#IPythonCellState.executionStarted), [`expandCollapseHint`](keybinding-hints.ts.md#expandCollapseHint), [`readDetails`](ipython-cell.ts.md#readDetails), [`details`](ipython-cell.ts.md#IPythonCellState.details), [`argsComplete`](ipython-cell.ts.md#IPythonCellState.argsComplete), [`formatAgentMessageParticipant`](../../../core/agent-messages.ts.md#formatAgentMessageParticipant), [`parseIpythonBashCell`](../../../core/tools/ipython-cell-code.ts.md#parseIpythonBashCell), [`previewIpythonCode`](../../../core/tools/code-preview.ts.md#previewIpythonCode), [`workingIconFrame`](../theme/working-icon.ts.md#workingIconFrame), [`formatIpythonErrorSummary`](ipython-cell.ts.md#formatIpythonErrorSummary), [`content`](ipython-cell.ts.md#IPythonCellState.content), [`highlightCode`](../theme/theme.ts.md#highlightCode), [`language`](../../../core/tools/code-preview.ts.md#CodePreview.language), [`agentMessageBodyLines`](agent-message.ts.md#agentMessageBodyLines), [`normalizeErrorDetails`](collapsible-error.ts.md#normalizeErrorDetails), [`IPythonCellState`](ipython-cell.ts.md#IPythonCellState), [`renderDiffSeparator`](diff.ts.md#renderDiffSeparator), [`text`](../../../core/tools/code-preview.ts.md#CodePreview.text), [`isAgentMessageReceipt`](ipython-cell.ts.md#isAgentMessageReceipt), [`isImageBlock`](ipython-cell.ts.md#isImageBlock), [`error`](ipython-cell.ts.md#IpythonDetails.error), [`WORKING_ICON_FRAMES`](../theme/working-icon.ts.md#WORKING_ICON_FRAMES), [`agentMessageSummaryLine`](agent-message.ts.md#agentMessageSummaryLine), [`getWorkingPulseFrame`](../theme/working-icon.ts.md#getWorkingPulseFrame), [`isEditConfirmation`](ipython-cell.ts.md#isEditConfirmation), [`sentAgentMessages`](ipython-cell.ts.md#IpythonDetails.sentAgentMessages), [`set`](../../../../../tui/src/render-cache.ts.md#VersionedRenderCache.set), [`textFromBlocks`](ipython-cell.ts.md#textFromBlocks), [`result`](ipython-cell.ts.md#IpythonDetails.result), [`diffs`](ipython-cell.ts.md#IpythonDetails.diffs), [`get`](../../../../../tui/src/render-cache.ts.md#VersionedRenderCache.get)  (+38 more)
- used by: [`Component`](../../../../../tui/src/tui.ts.md#Component), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`updateDisplay`](tool-execution.ts.md#ToolExecutionComponent.updateDisplay), [`tool-execution.ts`](tool-execution.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-tool-execution.ts), [`conversation-components.ts`](conversation-components.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-conversation-components.ts), [`isCompactAgentMessageNeighbor`](conversation-components.ts.md#isCompactAgentMessageNeighbor), [`ipythonCellComponent`](tool-execution.ts.md#ToolExecutionComponent.ipythonCellComponent)  (7 test-only)

### `IPythonCellContentBlock`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L21)
- signature: `interface IPythonCellContentBlock`
- members:
  - `data` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L24)
  - `mimeType` — [`L25`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L25)
  - `text` — [`L23`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L23)
  - `type` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L22)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`content`](ipython-cell.ts.md#IPythonCellState.content), [`isImageBlock`](ipython-cell.ts.md#isImageBlock), [`textFromBlocks`](ipython-cell.ts.md#textFromBlocks)  (3 test-only)

### `IPythonCellState`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:28`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L28)
- signature: `interface IPythonCellState`
- members:
  - `argsComplete` — [`L37`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L37)
  - `code` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L29)
  - `content` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L30)
  - `cwd` — [`L40`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L40) — Session cwd — edit paths nested under it render relative, else absolute.
  - `details` — [`L31`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L31)
  - `executionStarted` — [`L36`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L36)
  - `expanded` — [`L34`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L34)
  - `isError` — [`L33`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L33)
  - `isPartial` — [`L32`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L32)
  - `showExpandHint` — [`L35`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L35)
  - `showImages` — [`L38`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L38)
- uses (calls/refs, reference-scoped): [`IPythonCellContentBlock`](ipython-cell.ts.md#IPythonCellContentBlock)
- used by: [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-index.ts), [`render`](ipython-cell.ts.md#IPythonCellComponent.render), [`renderOutput`](ipython-cell.ts.md#IPythonCellComponent.renderOutput), [`collapsedLine`](ipython-cell.ts.md#IPythonCellComponent.collapsedLine), [`renderFileDiff`](ipython-cell.ts.md#IPythonCellComponent.renderFileDiff), [`renderSentAgentMessages`](ipython-cell.ts.md#IPythonCellComponent.renderSentAgentMessages), [`<constructor>`](ipython-cell.ts.md#IPythonCellComponent.-constructor), [`lineCounts`](ipython-cell.ts.md#IPythonCellComponent.lineCounts), [`state`](ipython-cell.ts.md#IPythonCellComponent.state), [`hasResult`](ipython-cell.ts.md#IPythonCellComponent.hasResult), [`renderCode`](ipython-cell.ts.md#IPythonCellComponent.renderCode), [`statusKind`](ipython-cell.ts.md#IPythonCellComponent.statusKind), [`update`](ipython-cell.ts.md#IPythonCellComponent.update)  (5 test-only)

### `IpythonDetails`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:62`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L62)
- signature: `interface IpythonDetails`
- members:
  - `diffs` — [`L69`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L69)
  - `durationMs` — [`L63`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L63)
  - `error` — [`L71`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L71)
  - `errorEname` — [`L65`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L65)
  - `result` — [`L68`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L68)
  - `sentAgentMessages` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L70)
  - `status` — [`L64`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L64)
  - `stderr` — [`L67`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L67)
  - `stdout` — [`L66`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L66)
- uses (calls/refs, reference-scoped): [`DiffDisplay`](ipython-cell.ts.md#DiffDisplay), [`SentAgentMessageDisplay`](ipython-cell.ts.md#SentAgentMessageDisplay), [`IpythonErrorDetails`](ipython-cell.ts.md#IpythonErrorDetails)
- used by: [`render`](ipython-cell.ts.md#IPythonCellComponent.render), [`renderOutput`](ipython-cell.ts.md#IPythonCellComponent.renderOutput), [`collapsedLine`](ipython-cell.ts.md#IPythonCellComponent.collapsedLine), [`readDetails`](ipython-cell.ts.md#readDetails), [`lineCounts`](ipython-cell.ts.md#IPythonCellComponent.lineCounts), [`hasResult`](ipython-cell.ts.md#IPythonCellComponent.hasResult), [`statusKind`](ipython-cell.ts.md#IPythonCellComponent.statusKind), [`marker`](ipython-cell.ts.md#IPythonCellComponent.marker)

### `IpythonErrorDetails`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:74`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L74)
- signature: `interface IpythonErrorDetails`
- members:
  - `ename` — [`L75`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L75)
  - `evalue` — [`L76`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L76)
  - `traceback` — [`L77`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L77)
- used by: [`renderOutput`](ipython-cell.ts.md#IPythonCellComponent.renderOutput), [`collapsedLine`](ipython-cell.ts.md#IPythonCellComponent.collapsedLine), [`readDetails`](ipython-cell.ts.md#readDetails), [`formatIpythonErrorSummary`](ipython-cell.ts.md#formatIpythonErrorSummary), [`error`](ipython-cell.ts.md#IpythonDetails.error), [`readErrorDetails`](ipython-cell.ts.md#readErrorDetails)

### `SentAgentMessageDisplay`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:50`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L50)
- signature: `interface SentAgentMessageDisplay`
- members:
  - `activeSessionId` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L56)
  - `deliveryStatus` — [`L53`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L53)
  - `id` — [`L51`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L51)
  - `message` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L52)
  - `receiverRole` — [`L54`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L54)
  - `sessionId` — [`L57`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L57)
  - `sessionName` — [`L58`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L58)
  - `target` — [`L55`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L55)
- used by: [`renderSentAgentMessages`](ipython-cell.ts.md#IPythonCellComponent.renderSentAgentMessages), [`readSentAgentMessages`](ipython-cell.ts.md#readSentAgentMessages), [`isAgentMessageReceipt`](ipython-cell.ts.md#isAgentMessageReceipt), [`sentAgentMessages`](ipython-cell.ts.md#IpythonDetails.sentAgentMessages)

### `TracebackParts`
- def: [`packages/coding-agent/src/modes/interactive/components/ipython-cell.ts:80`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L80)
- signature: `interface TracebackParts`
- members:
  - `output` — [`L81`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L81)
  - `preview` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L83)
  - `traceback` — [`L82`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L82)
- used by: [`renderOutput`](ipython-cell.ts.md#IPythonCellComponent.renderOutput), [`splitTraceback`](ipython-cell.ts.md#splitTraceback)

## Functions
- `closeOpenSgr(line: string)` — [`L98`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L98) — Append `ESC[0m` when `line` ends with a foreground or background color still
- `displayEditPath(path: string, cwd: string | undefined)` — [`L287`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L287)
- `formatDuration(durationMs: number | undefined)` — [`L276`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L276)
- `formatIpythonErrorSummary(error: IpythonErrorDetails)` — [`L333`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L333)
- `getIpythonCodeFromArgs(args: unknown)` — [`L128`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L128)
- `isAgentMessageReceipt(text: string | undefined, messages: readonly SentAgentMessageDisplay[])` — [`L249`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L249) — True when `text` is the `agent_message.send` receipt dict for one of the sent
- `isEditConfirmation(text: string | undefined, diffs: readonly DiffDisplay[])` — [`L234`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L234) — True when `text` is just the edit skill's "Edited <path>" confirmation for one of `diffs`.
- `isImageBlock(block: IPythonCellContentBlock)` — [`L298`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L298)
- `readDetails(details: unknown)` — [`L136`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L136)
- `readDiffDisplays(value: unknown)` — [`L197`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L197)
- `readErrorDetails(value: unknown)` — [`L259`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L259)
- `readSentAgentMessages(value: unknown)` — [`L155`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L155)
- `splitTraceback(text: string, errorName: string | undefined)` — [`L312`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L312)
- `stripReprQuotes(text: string)` — [`L222`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L222) — Strip one layer of repr quotes so an `execute_result` string compares cleanly.
- `textFromBlocks(blocks: readonly IPythonCellContentBlock[] | undefined)` — [`L302`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L302)

## Module values
- `MAGIC_LINE_PATTERN` — [`L86`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L86)
- `OUTPUT_INDENT` — [`L89`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L89)
- `SGR_PATTERN` — [`L91`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/ipython-cell.ts#L91)

