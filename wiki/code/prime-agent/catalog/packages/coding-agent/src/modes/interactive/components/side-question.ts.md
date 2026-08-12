---
title: 'Module: packages/coding-agent/src/modes/interactive/components/side-question.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/components/side-question.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/components/`side-question.ts`/SideQuestion
symbols:
  SideQuestionComponent.render: Component#render().
  SideQuestionComponent.addTurn: Component#addTurn().
  SideQuestionComponent.renderAnswer: Component#renderAnswer().
  SideQuestionComponent.renderHint: Component#renderHint().
  SideQuestionComponent.update: Component#update().
  SideQuestionComponent.invalidate: Component#invalidate().
  SideQuestionComponent.-constructor: Component#`<constructor>`().
  SideQuestionComponent.entries: Component#entries.
  SideQuestionComponent.finishBash: Component#finishBash().
  SideQuestionComponent.addBash: Component#addBash().
  SideQuestionTurnState.event: TurnState#event.
  SideQuestionComponent.applySurface: Component#applySurface().
  SideQuestionComponent.paddingX: Component#paddingX.
  SideQuestionTurnState.kind: TurnState#kind.
  SideQuestionBashState.kind: BashState#kind.
  SideQuestionTurnState.questionBubble: TurnState#questionBubble.
  SideQuestionTurnState.answer: TurnState#answer.
  SideQuestionComponent: Component#
  SideQuestionBashState.component: BashState#component.
  SideQuestionTurnState: TurnState#
  SideQuestionBashState.running: BashState#running.
  SideQuestionBashState: BashState#
---
# Module: [`packages/coding-agent/src/modes/interactive/components/side-question.ts`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts)

## Classes
### `SideQuestionBashState`
- def: [`packages/coding-agent/src/modes/interactive/components/side-question.ts:14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L14)
- doc: A ! / !! run inside the pane, rendered by the same component the main thread uses.
- signature: `interface SideQuestionBashState`
- members:
  - `component` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L16)
  - `kind` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L15)
  - `running` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L17)
- uses (calls/refs, reference-scoped): [`Component`](../../../../../tui/src/tui.ts.md#Component)
- used by: [`render`](side-question.ts.md#SideQuestionComponent.render), [`addTurn`](side-question.ts.md#SideQuestionComponent.addTurn), [`renderHint`](side-question.ts.md#SideQuestionComponent.renderHint), [`update`](side-question.ts.md#SideQuestionComponent.update), [`invalidate`](side-question.ts.md#SideQuestionComponent.invalidate), [`entries`](side-question.ts.md#SideQuestionComponent.entries), [`finishBash`](side-question.ts.md#SideQuestionComponent.finishBash), [`addBash`](side-question.ts.md#SideQuestionComponent.addBash)

### `SideQuestionComponent`  ·  implements/extends Component
- def: [`packages/coding-agent/src/modes/interactive/components/side-question.ts:20`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L20)
- signature: `class SideQuestionComponent`
- members:
  - `<constructor>(event: AgentConnectionSideQuestionEvent, paddingX?: number)` — [`L24`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L24)
  - `addBash(method)` — [`L48`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L48)
  - `addTurn(method)` — [`L29`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L29)
  - `applySurface(method)` — [`L144`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L144)
  - `finishBash(method)` — [`L52`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L52)
  - `invalidate(method)` — [`L72`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L72) — Invalidate any cached rendering state.
  - `render(method)` — [`L83`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L83) — Render the component to lines for the given viewport width
  - `renderAnswer(method)` — [`L115`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L115)
  - `renderHint(method)` — [`L134`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L134)
  - `update(method)` — [`L60`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L60)
  - `entries` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L22)
  - `paddingX` — [`L21`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L21)
- uses (calls/refs, reference-scoped): [`fg`](../theme/theme.ts.md#Theme.fg), [`theme`](../theme/theme.ts.md#theme), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`visibleWidth`](../../../../../tui/src/utils.ts.md#visibleWidth), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`<constructor>`](../../../../../tui/src/components/text.ts.md#Text.-constructor), [`render`](../../../../../tui/src/components/markdown.ts.md#Markdown.render), [`<constructor>`](../../../../../tui/src/components/markdown.ts.md#Markdown.-constructor), [`getMarkdownTheme`](../theme/theme.ts.md#getMarkdownTheme), [`bold`](../theme/theme.ts.md#Theme.bold), [`render`](../../../../../tui/src/components/box.ts.md#Box.render), [`render`](../../../../../tui/src/components/text.ts.md#Text.render), [`addChild`](../../../../../tui/src/components/box.ts.md#Box.addChild), [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`id`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent.id), [`status`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent.status), [`answer`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent.answer), [`setText`](../../../../../tui/src/components/markdown.ts.md#Markdown.setText), [`question`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent.question), [`invalidate`](../../../../../tui/src/components/box.ts.md#Box.invalidate), [`<constructor>`](../../../../../tui/src/components/box.ts.md#Box.-constructor), [`invalidate`](../../../../../tui/src/components/markdown.ts.md#Markdown.invalidate), [`AgentConnectionSideQuestionEvent`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent), [`event`](side-question.ts.md#SideQuestionTurnState.event), [`getUserMessageBackgroundColor`](../theme/theme.ts.md#Theme.getUserMessageBackgroundColor), [`kind`](side-question.ts.md#SideQuestionBashState.kind), [`kind`](side-question.ts.md#SideQuestionTurnState.kind), [`answer`](side-question.ts.md#SideQuestionTurnState.answer), [`getPopupBackgroundColor`](../theme/theme.ts.md#Theme.getPopupBackgroundColor), [`questionBubble`](side-question.ts.md#SideQuestionTurnState.questionBubble), [`component`](side-question.ts.md#SideQuestionBashState.component), [`errorMessage`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent.errorMessage), [`SideQuestionTurnState`](side-question.ts.md#SideQuestionTurnState), [`running`](side-question.ts.md#SideQuestionBashState.running), [`SideQuestionBashState`](side-question.ts.md#SideQuestionBashState)
- used by: [`interactive-mode.ts`](../interactive-mode.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-interactive-mode.ts), [`Component`](../../../../../tui/src/tui.ts.md#Component), [`handleEvent`](../interactive-mode.ts.md#InteractiveMode.handleEvent), [`setupEditorSubmitHandler`](../interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`render`](../../../../../tui/src/tui.ts.md#Component.render), [`invalidate`](../../../../../tui/src/tui.ts.md#Component.invalidate), [`renderResyncedSession`](../interactive-mode.ts.md#InteractiveMode.renderResyncedSession), [`handleSideQuestion`](../interactive-mode.ts.md#InteractiveMode.handleSideQuestion), [`finishSideQuestionBash`](../interactive-mode.ts.md#InteractiveMode.finishSideQuestionBash), [`handleSideQuestionEvent`](../interactive-mode.ts.md#InteractiveMode.handleSideQuestionEvent), [`sideQuestionComponent`](../interactive-mode.ts.md#InteractiveMode.sideQuestionComponent)  (1 test-only)

### `SideQuestionTurnState`
- def: [`packages/coding-agent/src/modes/interactive/components/side-question.ts:5`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L5)
- signature: `interface SideQuestionTurnState`
- members:
  - `answer` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L10)
  - `event` — [`L7`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L7)
  - `kind` — [`L6`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L6)
  - `questionBubble` — [`L9`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/components/side-question.ts#L9) — Follow-up questions render as a standard user-message bubble; the first turn keeps the /btw header.
- uses (calls/refs, reference-scoped): [`Box`](../../../../../tui/src/components/box.ts.md#Box), [`Markdown`](../../../../../tui/src/components/markdown.ts.md#Markdown), [`AgentConnectionSideQuestionEvent`](../../agent-connection/types.ts.md#AgentConnectionSideQuestionEvent)
- used by: [`render`](side-question.ts.md#SideQuestionComponent.render), [`addTurn`](side-question.ts.md#SideQuestionComponent.addTurn), [`renderAnswer`](side-question.ts.md#SideQuestionComponent.renderAnswer), [`renderHint`](side-question.ts.md#SideQuestionComponent.renderHint), [`update`](side-question.ts.md#SideQuestionComponent.update), [`invalidate`](side-question.ts.md#SideQuestionComponent.invalidate), [`entries`](side-question.ts.md#SideQuestionComponent.entries), [`finishBash`](side-question.ts.md#SideQuestionComponent.finishBash), [`addBash`](side-question.ts.md#SideQuestionComponent.addBash)

