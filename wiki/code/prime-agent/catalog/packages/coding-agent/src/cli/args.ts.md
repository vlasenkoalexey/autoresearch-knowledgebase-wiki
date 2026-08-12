---
title: 'Module: packages/coding-agent/src/cli/args.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/args.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`args.ts`/
symbols:
  parseArgs: parseArgs().
  Args.messages: Args#messages.
  Args.diagnostics: Args#diagnostics.
  Args.resume: Args#resume.
  hasRequiredOptionValue: hasRequiredOptionValue().
  Args: Args#
  parsePositiveInt: parsePositiveInt().
  Args.autonomous: Args#autonomous.
  Args.unknownFlags: Args#unknownFlags.
  Args.diagnostics.Array.typeLiteral0.type: Args#diagnostics.Array:typeLiteral0:type.
  Args.diagnostics.Array.typeLiteral0.message: Args#diagnostics.Array:typeLiteral0:message.
  Args.noSession: Args#noSession.
  Args.mode: Args#mode.
  Args.autonomousGates: Args#autonomousGates.
  Args.fileArgs: Args#fileArgs.
  INTERNAL_RUNTIME_COMMAND_MARKER: INTERNAL_RUNTIME_COMMAND_MARKER.
  isValidThinkingLevel: isValidThinkingLevel().
  Args.goal: Args#goal.
  Args.continue: Args#continue.
  Args.tools: Args#tools.
  Args.print: Args#print.
  Args.listModels: Args#listModels.
  Args.fork: Args#fork.
  Args.extensions: Args#extensions.
  Args.provider: Args#provider.
  Args.autonomousMaxTurns: Args#autonomousMaxTurns.
  Args.goalTokenBudget: Args#goalTokenBudget.
  Args.verbose: Args#verbose.
  Args.thinking: Args#thinking.
  Args.cwd: Args#cwd.
  Args.appendSystemPrompt: Args#appendSystemPrompt.
  Args.skills: Args#skills.
  Args.promptTemplates: Args#promptTemplates.
  Args.themes: Args#themes.
  Args.help: Args#help.
  Args.version: Args#version.
  Args.noTools: Args#noTools.
  Args.noBuiltinTools: Args#noBuiltinTools.
  Args.export: Args#export.
  Args.autonomousGateRetries: Args#autonomousGateRetries.
  Args.autonomousGateTimeoutMs: Args#autonomousGateTimeoutMs.
  Args.model: Args#model.
  Args.daemonSocket: Args#daemonSocket.
  Args.noExtensions: Args#noExtensions.
  Args.noContextFiles: Args#noContextFiles.
  Args.autonomousMaxContinuations: Args#autonomousMaxContinuations.
  Args.autonomousMaxTokens: Args#autonomousMaxTokens.
  Args.autonomousTimeoutMs: Args#autonomousTimeoutMs.
  Mode: Mode#
  Args.apiKey: Args#apiKey.
  Args.systemPrompt: Args#systemPrompt.
  Args.sessionDir: Args#sessionDir.
  Args.models: Args#models.
  Args.noSkills: Args#noSkills.
  Args.noPromptTemplates: Args#noPromptTemplates.
  Args.noThemes: Args#noThemes.
  Args.offline: Args#offline.
  VALID_THINKING_LEVELS: VALID_THINKING_LEVELS.
  REMOVED_BUILTIN_TOOL_NAMES: REMOVED_BUILTIN_TOOL_NAMES.
  BUILTIN_TOOL_NAMES: BUILTIN_TOOL_NAMES.
---
# Module: [`packages/coding-agent/src/cli/args.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts)

## Classes
### `Args`
- def: [`packages/coding-agent/src/cli/args.ts:10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L10)
- signature: `interface Args`
- members:
  - `apiKey` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L13)
  - `appendSystemPrompt` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L16)
  - `autonomous` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L42)
  - `autonomousGateRetries` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L44)
  - `autonomousGateTimeoutMs` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L45)
  - `autonomousGates` — [`L43`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L43)
  - `autonomousMaxContinuations` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L46)
  - `autonomousMaxTokens` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L48)
  - `autonomousMaxTurns` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L47)
  - `autonomousTimeoutMs` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L49)
  - `continue` — [`L18`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L18)
  - `cwd` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L14)
  - `daemonSocket` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L23)
  - `diagnostics` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L59)
  - `export` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L34)
  - `extensions` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L31)
  - `fileArgs` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L56)
  - `fork` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L25)
  - `goal` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L50)
  - `goalTokenBudget` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L51)
  - `help` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L20)
  - `listModels` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L52)
  - `message` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L59)
  - `messages` — [`L55`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L55)
  - `mode` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L22)
  - `model` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L12)
  - `models` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L27)
  - `noBuiltinTools` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L30)
  - `noContextFiles` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L41)
  - `noExtensions` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L32)
  - `noPromptTemplates` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L38)
  - `noSession` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L24)
  - `noSkills` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L35)
  - `noThemes` — [`L40`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L40)
  - `noTools` — [`L29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L29)
  - `offline` — [`L53`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L53)
  - `print` — [`L33`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L33)
  - `promptTemplates` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L37)
  - `provider` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L11)
  - `resume` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L19)
  - `sessionDir` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L26)
  - `skills` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L36)
  - `systemPrompt` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L15)
  - `themes` — [`L39`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L39)
  - `thinking` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L17)
  - `tools` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L28)
  - `type` — [`L59`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L59)
  - `unknownFlags` — [`L58`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L58) — Unknown flags (potentially extension flags) - map of flag name to value
  - `verbose` — [`L54`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L54)
  - `version` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L21)
- uses (calls/refs, reference-scoped): [`ThinkingLevel`](../../../agent/src/types.ts.md#ThinkingLevel), [`Mode`](args.ts.md#Mode)
- used by: [`main`](../main.ts.md#main), [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`parseArgs`](args.ts.md#parseArgs), [`runtimeConfigFromArgs`](../main.ts.md#runtimeConfigFromArgs), [`createSessionManager`](../main.ts.md#createSessionManager), [`buildInitialMessage`](initial-message.ts.md#buildInitialMessage), [`runtimeAutonomousConfigFromArgs`](../main.ts.md#runtimeAutonomousConfigFromArgs), [`initialImages`](../main.ts.md#prepareInitialMessage.Promise.typeLiteral38.initialImages), [`hasRequiredOptionValue`](args.ts.md#hasRequiredOptionValue), [`getInteractiveDaemonSessionPath`](../main.ts.md#getInteractiveDaemonSessionPath), [`parsePositiveInt`](args.ts.md#parsePositiveInt), [`validateForkFlags`](../main.ts.md#validateForkFlags), [`initial-message.ts`](initial-message.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-initial-message.ts), [`resolveAppMode`](../main.ts.md#resolveAppMode), [`hasPositionalArguments`](public-command.ts.md#hasPositionalArguments), [`parsed`](initial-message.ts.md#InitialMessageInput.parsed), [`getResumeSelector`](../main.ts.md#getResumeSelector), [`prepareInitialMessage`](../main.ts.md#prepareInitialMessage)  (6 test-only)

### `Mode`
- def: [`packages/coding-agent/src/cli/args.ts:8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L8)
- signature: `type Mode`
- used by: [`main.ts`](../main.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-main.ts), [`mode`](args.ts.md#Args.mode), [`toPrintOutputMode`](../main.ts.md#toPrintOutputMode)

## Functions
- `hasRequiredOptionValue(args: string[], index: number, flag: string, result: Args)` — [`L330`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L330)
- `isValidThinkingLevel(level: string)` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L68)
- `parseArgs(args: string[])` — [`L72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L72)
- `parsePositiveInt(value: string, flag: string, result: Args)` — [`L339`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L339)

## Module values
- `BUILTIN_TOOL_NAMES` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L64)
- `INTERNAL_RUNTIME_COMMAND_MARKER` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L66)
- `REMOVED_BUILTIN_TOOL_NAMES` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L63)
- `VALID_THINKING_LEVELS` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/args.ts#L62)

