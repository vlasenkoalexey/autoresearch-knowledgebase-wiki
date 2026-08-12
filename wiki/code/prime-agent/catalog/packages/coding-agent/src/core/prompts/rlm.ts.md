---
title: 'Module: packages/coding-agent/src/core/prompts/rlm.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/prompts/rlm.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/prompts/`rlm.ts`/
symbols:
  buildRlmPrompt: buildRlmPrompt().
  buildChildAgentDoctrine: buildChildAgentDoctrine().
  RlmPromptOptions.cwd: RlmPromptOptions#cwd.
  RlmPromptOptions.messagesPath: RlmPromptOptions#messagesPath.
  RlmPromptOptions.activeTools: RlmPromptOptions#activeTools.
  RlmPromptOptions.allowRecursion: RlmPromptOptions#allowRecursion.
  buildSubagentGuidance: buildSubagentGuidance().
  RlmPromptOptions.installedSkills: RlmPromptOptions#installedSkills.
  RlmPromptOptions.depth: RlmPromptOptions#depth.
  ChildAgentDoctrineOptions.activeTools: ChildAgentDoctrineOptions#activeTools.
  RlmPromptOptions: RlmPromptOptions#
  ChildAgentDoctrineOptions: ChildAgentDoctrineOptions#
  ChildAgentDoctrineOptions.depth: ChildAgentDoctrineOptions#depth.
  ChildAgentDoctrineOptions.parentAgent: ChildAgentDoctrineOptions#parentAgent.
  ChildAgentDoctrineOptions.installedSkills: ChildAgentDoctrineOptions#installedSkills.
  RlmPromptOptions.skillsDir: RlmPromptOptions#skillsDir.
  RlmPromptOptions.parentAgent: RlmPromptOptions#parentAgent.
  IPYTHON_CONTROL_PROMPT: IPYTHON_CONTROL_PROMPT.
  buildSubagentGuidance.options-typeLiteral60.includeRefineExamples: buildSubagentGuidance().(options)typeLiteral60:includeRefineExamples.
  buildSubagentGuidance.options-typeLiteral60.hasAgentMessage: buildSubagentGuidance().(options)typeLiteral60:hasAgentMessage.
  buildSubagentGuidance.options-typeLiteral60.hasAgentObserve: buildSubagentGuidance().(options)typeLiteral60:hasAgentObserve.
---
# Module: [`packages/coding-agent/src/core/prompts/rlm.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts)

## Classes
### `ChildAgentDoctrineOptions`
- def: [`packages/coding-agent/src/core/prompts/rlm.ts:36`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L36)
- signature: `interface ChildAgentDoctrineOptions`
- members:
  - `activeTools` — [`L40`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L40)
  - `depth` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L37)
  - `installedSkills` — [`L39`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L39)
  - `parentAgent` — [`L38`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L38)
- used by: [`buildSystemPrompt`](../system-prompt.ts.md#buildSystemPrompt), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-prompts-index.ts), [`buildChildAgentDoctrine`](rlm.ts.md#buildChildAgentDoctrine)

### `RlmPromptOptions`
- def: [`packages/coding-agent/src/core/prompts/rlm.ts:3`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L3)
- signature: `interface RlmPromptOptions`
- members:
  - `activeTools` — [`L11`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L11)
  - `allowRecursion` — [`L8`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L8)
  - `cwd` — [`L4`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L4)
  - `depth` — [`L9`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L9)
  - `installedSkills` — [`L6`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L6)
  - `messagesPath` — [`L7`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L7)
  - `parentAgent` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L10)
  - `skillsDir` — [`L5`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L5)
- used by: [`buildSystemPrompt`](../system-prompt.ts.md#buildSystemPrompt), [`buildRlmPrompt`](rlm.ts.md#buildRlmPrompt), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-prompts-index.ts)  (1 test-only)

## Functions
- `buildChildAgentDoctrine(options: ChildAgentDoctrineOptions)` — [`L43`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L43)
- `buildRlmPrompt(options: RlmPromptOptions)` — [`L60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L60)
- `buildSubagentGuidance(options?: { includeRefineExamples?: boolean | undefined; hasAgentMessage?: boolean | undefined; hasAgentObserve?: boolean | undefined; })` — [`L174`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L174) — Supplemental sub-agent delegation guidance, appended after the base RLM

## Module values
- `IPYTHON_CONTROL_PROMPT` — [`L14`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L14)
- `hasAgentMessage` — [`L175`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L175)
- `hasAgentObserve` — [`L175`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L175)
- `includeRefineExamples` — [`L175`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/prompts/rlm.ts#L175)

