---
title: 'Module: packages/coding-agent/src/core/skill-blocks.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/skill-blocks.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`skill-blocks.ts`/
symbols:
  parseSkillBlock: parseSkillBlock().
  ParsedSkillBlock: ParsedSkillBlock#
  ParsedSkillBlock.name: ParsedSkillBlock#name.
  ParsedSkillBlock.userMessage: ParsedSkillBlock#userMessage.
  ParsedSkillBlock.content: ParsedSkillBlock#content.
  ParsedSkillBlock.location: ParsedSkillBlock#location.
---
# Module: [`packages/coding-agent/src/core/skill-blocks.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts)

## Classes
### `ParsedSkillBlock`
- def: [`packages/coding-agent/src/core/skill-blocks.ts:2`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L2)
- doc: Parsed skill block from a user message.
- signature: `interface ParsedSkillBlock`
- members:
  - `content` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L5)
  - `location` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L4)
  - `name` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L3)
  - `userMessage` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L6)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`addMessageToChat`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.addMessageToChat), [`skill-invocation-message.ts`](../modes/interactive/components/skill-invocation-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-modes-interactive-components-skill-invocation-message.ts), [`updateDisplay`](../modes/interactive/components/skill-invocation-message.ts.md#SkillInvocationMessageComponent.updateDisplay), [`<constructor>`](../modes/interactive/components/skill-invocation-message.ts.md#SkillInvocationMessageComponent.-constructor), [`parseSkillBlock`](skill-blocks.ts.md#parseSkillBlock), [`skillBlock`](../modes/interactive/components/skill-invocation-message.ts.md#SkillInvocationMessageComponent.skillBlock)

## Functions
- `parseSkillBlock(text: string)` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/skill-blocks.ts#L13) — Parse a skill block from message text.

