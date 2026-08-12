---
title: 'Module: packages/coding-agent/src/core/system-prompt.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/system-prompt.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`system-prompt.ts`/
symbols:
  buildSystemPrompt: buildSystemPrompt().
  BuildSystemPromptOptions.skills: BuildSystemPromptOptions#skills.
  BuildSystemPromptOptions: BuildSystemPromptOptions#
  BuildSystemPromptOptions.selectedTools: BuildSystemPromptOptions#selectedTools.
  BuildSystemPromptOptions.cwd: BuildSystemPromptOptions#cwd.
  BuildSystemPromptOptions.contextFiles: BuildSystemPromptOptions#contextFiles.
  BuildSystemPromptOptions.harnessState: BuildSystemPromptOptions#harnessState.
  BuildSystemPromptOptions.messagesPath: BuildSystemPromptOptions#messagesPath.
  BuildSystemPromptOptions.customPrompt: BuildSystemPromptOptions#customPrompt.
  BuildSystemPromptOptions.appendSystemPrompt: BuildSystemPromptOptions#appendSystemPrompt.
  BuildSystemPromptOptions.rlmDepth: BuildSystemPromptOptions#rlmDepth.
  BuildSystemPromptOptions.rlmParentAgent: BuildSystemPromptOptions#rlmParentAgent.
  BuildSystemPromptOptions.promptGuidelines: BuildSystemPromptOptions#promptGuidelines.
  BuildSystemPromptOptions.contextFiles.Array.typeLiteral0.path: BuildSystemPromptOptions#contextFiles.Array:typeLiteral0:path.
  BuildSystemPromptOptions.contextFiles.Array.typeLiteral0.content: BuildSystemPromptOptions#contextFiles.Array:typeLiteral0:content.
  BuildSystemPromptOptions.allowRecursion: BuildSystemPromptOptions#allowRecursion.
  BuildSystemPromptOptions.toolSnippets: BuildSystemPromptOptions#toolSnippets.
  formatPromptGuidelines: formatPromptGuidelines().
---
# Module: [`packages/coding-agent/src/core/system-prompt.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts)

## Classes
### `BuildSystemPromptOptions`
- def: [`packages/coding-agent/src/core/system-prompt.ts:9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L9)
- signature: `interface BuildSystemPromptOptions`
- members:
  - `allowRecursion` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L29) — Whether to include the model-facing rlm recursion guidance.
  - `appendSystemPrompt` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L19) — Text to append to system prompt.
  - `content` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L25)
  - `contextFiles` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L25) — Pre-loaded context files.
  - `customPrompt` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L11) — Custom system prompt (replaces default).
  - `cwd` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L21) — Working directory.
  - `harnessState` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L35) — Global harness state to inject as compact persistent context.
  - `messagesPath` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L23) — Conversation log path.
  - `path` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L25)
  - `promptGuidelines` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L17) — Additional guideline bullets appended to the system prompt.
  - `rlmDepth` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L31) — Fixed recursive-agent depth for this session.
  - `rlmParentAgent` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L33) — Human-readable parent name or id for child communication doctrine.
  - `selectedTools` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L13) — Active tools. Tool schemas carry tool descriptions outside the prompt body.
  - `skills` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L27) — Pre-loaded skills.
  - `toolSnippets` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L15) — Optional one-line tool snippets keyed by tool name. Used only for custom prompts.
- uses (calls/refs, reference-scoped): [`Skill`](skills.ts.md#Skill), [`HarnessState`](refinement/refinement.ts.md#HarnessState)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`index.ts`](index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`runner.ts`](extensions/runner.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-runner.ts), [`buildSystemPrompt`](system-prompt.ts.md#buildSystemPrompt), [`_rebuildSystemPrompt`](agent-session.ts.md#AgentSession._rebuildSystemPrompt), [`emitBeforeAgentStart`](extensions/runner.ts.md#ExtensionRunner.emitBeforeAgentStart), [`_baseSystemPromptOptions`](agent-session.ts.md#AgentSession._baseSystemPromptOptions), [`systemPromptOptions`](extensions/types.ts.md#BeforeAgentStartEvent.systemPromptOptions)  (6 test-only)

## Functions
- `buildSystemPrompt(options: BuildSystemPromptOptions)` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L39) — Build the system prompt with tools, guidelines, and context
- `formatPromptGuidelines(promptGuidelines: string[] | undefined)` — [`L171`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/system-prompt.ts#L171)

