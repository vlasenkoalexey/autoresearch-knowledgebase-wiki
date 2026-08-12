---
title: 'Module: packages/coding-agent/src/core/slash-commands.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/slash-commands.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`slash-commands.ts`/
symbols:
  BuiltinSlashCommand.name: BuiltinSlashCommand#name.
  parseSessionSlashCommand: parseSessionSlashCommand().
  BuiltinSlashCommand.description: BuiltinSlashCommand#description.
  BUILTIN_SLASH_COMMANDS: BUILTIN_SLASH_COMMANDS.
  parseSlashCommand: parseSlashCommand().
  buildBuiltinSlashCommands: buildBuiltinSlashCommands().
  ParsedSlashCommand.name: ParsedSlashCommand#name.
  resolveSlashCommand: resolveSlashCommand().
  BuiltinSlashCommand.argumentHint: BuiltinSlashCommand#argumentHint.
  parseRefineCommandOptions: parseRefineCommandOptions().
  builtinSlashCommandTakesArgument: builtinSlashCommandTakesArgument().
  BuiltinSlashCommand.takesArgument: BuiltinSlashCommand#takesArgument.
  isBuiltinSlashCommandName: isBuiltinSlashCommandName().
  CANONICAL_BUILTIN_SLASH_COMMANDS: CANONICAL_BUILTIN_SLASH_COMMANDS.
  resolveBuiltinSlashCommandName: resolveBuiltinSlashCommandName().
  isSessionSlashCommandName: isSessionSlashCommandName().
  SlashCommandInfo: SlashCommandInfo#
  SessionSlashCommand: SessionSlashCommand#
  SessionSlashCommand.text: SessionSlashCommand#text.
  SessionSlashCommand.name: SessionSlashCommand#name.
  BUILTIN_SLASH_COMMAND_ALIAS_TO_NAME: BUILTIN_SLASH_COMMAND_ALIAS_TO_NAME.
  SessionSlashCommand.args: SessionSlashCommand#args.
  BuiltinSlashCommandAlias.aliasFor: BuiltinSlashCommandAlias#aliasFor.
  BUILTIN_SLASH_COMMAND_ALIASES: BUILTIN_SLASH_COMMAND_ALIASES.
  BuiltinSlashCommandAlias.name: BuiltinSlashCommandAlias#name.
  BUILTIN_SLASH_COMMAND_BY_NAME: BUILTIN_SLASH_COMMAND_BY_NAME.
  ParsedSlashCommand.args: ParsedSlashCommand#args.
  SlashCommandInfo.sourceInfo: SlashCommandInfo#sourceInfo.
  SESSION_SLASH_COMMAND_NAMES: SESSION_SLASH_COMMAND_NAMES.
  BuiltinSlashCommand.aliases: BuiltinSlashCommand#aliases.
  SlashCommandInfo.source: SlashCommandInfo#source.
  SessionSlashCommandName: SessionSlashCommandName#
  SlashCommandSource: SlashCommandSource#
  SESSION_SLASH_COMMAND_NAME_SET: SESSION_SLASH_COMMAND_NAME_SET.
  ResolvedSlashCommand: ResolvedSlashCommand#
  SlashCommandInfo.name: SlashCommandInfo#name.
  BuiltinSlashCommand: BuiltinSlashCommand#
  BuiltinSlashCommand.execution: BuiltinSlashCommand#execution.
  ParsedSlashCommand: ParsedSlashCommand#
  SlashCommandInfo.description: SlashCommandInfo#description.
  RefineCommandOptions.global: RefineCommandOptions#global.
  RefineCommandOptions: RefineCommandOptions#
  RefineCommandOptions.instructions: RefineCommandOptions#instructions.
  RefineCommandOptions.rollbackId: RefineCommandOptions#rollbackId.
  ResolvedSlashCommand.originalName: ResolvedSlashCommand#originalName.
  ResolvedSlashCommand.isAlias: ResolvedSlashCommand#isAlias.
  BuiltinSlashCommandAlias: BuiltinSlashCommandAlias#
---
# Module: [`packages/coding-agent/src/core/slash-commands.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts)

## Classes
### `BuiltinSlashCommand`
- def: [`packages/coding-agent/src/core/slash-commands.ts:61`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L61)
- signature: `interface BuiltinSlashCommand`
- members:
  - `aliases` — [`L68`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L68) — Hidden names that resolve to this command without being shown as commands.
  - `argumentHint` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L66) — Shown in autocomplete before the description, e.g. "[instructions]"
  - `description` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L63)
  - `execution` — [`L64`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L64)
  - `name` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L62)
  - `takesArgument` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L69)
- used by: [`createBaseAutocompleteProvider`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.createBaseAutocompleteProvider), [`parseSessionSlashCommand`](slash-commands.ts.md#parseSessionSlashCommand), [`BUILTIN_SLASH_COMMANDS`](slash-commands.ts.md#BUILTIN_SLASH_COMMANDS), [`createReplyComposerAutocompleteProvider`](../modes/agents-view/agents-view-mode.ts.md#createReplyComposerAutocompleteProvider), [`agentsViewSlashCommands`](../modes/agents-view/agents-view-mode.ts.md#agentsViewSlashCommands), [`buildBuiltinSlashCommands`](slash-commands.ts.md#buildBuiltinSlashCommands), [`builtinSlashCommandTakesArgument`](slash-commands.ts.md#builtinSlashCommandTakesArgument), [`CANONICAL_BUILTIN_SLASH_COMMANDS`](slash-commands.ts.md#CANONICAL_BUILTIN_SLASH_COMMANDS), [`BUILTIN_SLASH_COMMAND_ALIAS_TO_NAME`](slash-commands.ts.md#BUILTIN_SLASH_COMMAND_ALIAS_TO_NAME), [`BUILTIN_SLASH_COMMAND_BY_NAME`](slash-commands.ts.md#BUILTIN_SLASH_COMMAND_BY_NAME)  (2 test-only)

### `BuiltinSlashCommandAlias`
- def: [`packages/coding-agent/src/core/slash-commands.ts:82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L82)
- signature: `interface BuiltinSlashCommandAlias`
- members:
  - `aliasFor` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L84)
  - `name` — [`L83`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L83)
- used by: [`buildBuiltinSlashCommands`](slash-commands.ts.md#buildBuiltinSlashCommands), [`BUILTIN_SLASH_COMMAND_ALIASES`](slash-commands.ts.md#BUILTIN_SLASH_COMMAND_ALIASES)

### `ParsedSlashCommand`
- def: [`packages/coding-agent/src/core/slash-commands.ts:72`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L72)
- signature: `interface ParsedSlashCommand`
- members:
  - `args` — [`L74`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L74)
  - `name` — [`L73`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L73)
- used by: [`setupEditorSubmitHandler`](../modes/interactive/interactive-mode.ts.md#InteractiveMode.setupEditorSubmitHandler), [`parseSessionSlashCommand`](slash-commands.ts.md#parseSessionSlashCommand), [`_expandSkillCommand`](agent-session.ts.md#AgentSession._expandSkillCommand), [`<constructor>`](../modes/interactive/components/user-message.ts.md#SlashCommandMarkdown.-constructor), [`_executeExtensionCommand`](agent-session.ts.md#AgentSession._executeExtensionCommand), [`parseSlashCommand`](slash-commands.ts.md#parseSlashCommand), [`getReplyComposerCommandRejection`](../modes/agents-view/agents-view-mode.ts.md#getReplyComposerCommandRejection), [`parseAgentsViewCommand`](../modes/agents-view/agents-view-mode.ts.md#parseAgentsViewCommand), [`expandPromptTemplate`](prompt-templates.ts.md#expandPromptTemplate), [`resolveSlashCommand`](slash-commands.ts.md#resolveSlashCommand), [`styleSlashCommandText`](../modes/interactive/components/slash-command-message.ts.md#styleSlashCommandText), [`_throwIfExtensionCommand`](agent-session.ts.md#AgentSession._throwIfExtensionCommand), [`isLeadingSlashCommand`](../modes/interactive/components/slash-command-message.ts.md#isLeadingSlashCommand), [`ResolvedSlashCommand`](slash-commands.ts.md#ResolvedSlashCommand)

### `RefineCommandOptions`
- def: [`packages/coding-agent/src/core/slash-commands.ts:29`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L29)
- signature: `interface RefineCommandOptions`
- members:
  - `global` — [`L32`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L32)
  - `instructions` — [`L30`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L30)
  - `rollbackId` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L31)
- used by: [`parseRefineCommandOptions`](slash-commands.ts.md#parseRefineCommandOptions)

### `ResolvedSlashCommand`
- def: [`packages/coding-agent/src/core/slash-commands.ts:77`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L77)
- signature: `interface ResolvedSlashCommand`
- members:
  - `isAlias` — [`L79`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L79)
  - `originalName` — [`L78`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L78)
- uses (calls/refs, reference-scoped): [`ParsedSlashCommand`](slash-commands.ts.md#ParsedSlashCommand)
- used by: [`resolveSlashCommand`](slash-commands.ts.md#resolveSlashCommand)

### `SessionSlashCommand`
- def: [`packages/coding-agent/src/core/slash-commands.ts:23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L23)
- signature: `interface SessionSlashCommand`
- members:
  - `args` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L25)
  - `name` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L24)
  - `text` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L26)
- uses (calls/refs, reference-scoped): [`SessionSlashCommandName`](slash-commands.ts.md#SessionSlashCommandName)
- used by: [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`messages.ts`](messages.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-messages.ts), [`_executeQueuedSessionCommand`](agent-session.ts.md#AgentSession._executeQueuedSessionCommand), [`parseSessionSlashCommand`](slash-commands.ts.md#parseSessionSlashCommand), [`_appendDurableSessionCommandMessage`](agent-session.ts.md#AgentSession._appendDurableSessionCommandMessage), [`createSessionSlashCommandMessage`](messages.ts.md#createSessionSlashCommandMessage), [`session-action-store.ts`](session-action-store.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-session-action-store.ts), [`isSessionSlashCommandMessage`](messages.ts.md#isSessionSlashCommandMessage), [`_restoreSessionCommand`](agent-session.ts.md#AgentSession._restoreSessionCommand), [`isSessionSlashCommand`](messages.ts.md#isSessionSlashCommand), [`SessionActionRecoveryPayload`](agent-session.ts.md#SessionActionRecoveryPayload), [`_parseGoalSlashCommand`](agent-session.ts.md#AgentSession._parseGoalSlashCommand), [`command`](messages.ts.md#SessionSlashCommandResultDetails.command), [`_parseAutonomousSlashCommand`](agent-session.ts.md#AgentSession._parseAutonomousSlashCommand), [`command`](session-action-store.ts.md#SessionCommandPayload.command), [`_createSessionCommandAction`](agent-session.ts.md#AgentSession._createSessionCommandAction), [`command`](messages.ts.md#SessionSlashCommandDetails.command), [`NormalizedSubmission`](agent-session.ts.md#NormalizedSubmission)  (3 test-only)

### `SessionSlashCommandName`
- def: [`packages/coding-agent/src/core/slash-commands.ts:15`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L15)
- signature: `type SessionSlashCommandName`
- uses (calls/refs, reference-scoped): [`SESSION_SLASH_COMMAND_NAMES`](slash-commands.ts.md#SESSION_SLASH_COMMAND_NAMES)
- used by: [`isSessionSlashCommandName`](slash-commands.ts.md#isSessionSlashCommandName), [`name`](slash-commands.ts.md#SessionSlashCommand.name)

### `SlashCommandInfo`
- def: [`packages/coding-agent/src/core/slash-commands.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L6)
- signature: `interface SlashCommandInfo`
- members:
  - `description` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L8)
  - `name` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L7)
  - `source` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L9)
  - `sourceInfo` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L10)
- uses (calls/refs, reference-scoped): [`SourceInfo`](source-info.ts.md#SourceInfo), [`SlashCommandSource`](slash-commands.ts.md#SlashCommandSource)
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`agent-session.ts`](agent-session.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-agent-session.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`types.ts`](extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`_bindExtensionCore`](agent-session.ts.md#AgentSession._bindExtensionCore), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`GetCommandsHandler`](extensions/types.ts.md#GetCommandsHandler), [`getCommands`](extensions/types.ts.md#ExtensionAPI.getCommands)  (2 test-only)

### `SlashCommandSource`
- def: [`packages/coding-agent/src/core/slash-commands.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L4)
- signature: `type SlashCommandSource`
- used by: [`index.ts`](../index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-index.ts), [`index.ts`](extensions/index.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-index.ts), [`modelFallbackMessage`](sdk.ts.md#CreateAgentSessionResult.modelFallbackMessage), [`source`](slash-commands.ts.md#SlashCommandInfo.source)

## Functions
- `buildBuiltinSlashCommands()` — [`L207`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L207)
- `builtinSlashCommandTakesArgument(name: string)` — [`L251`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L251)
- `isBuiltinSlashCommandName(name: string)` — [`L247`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L247)
- `isSessionSlashCommandName(value: unknown)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L19)
- `parseRefineCommandOptions(args: string)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L35)
- `parseSessionSlashCommand(text: string)` — [`L267`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L267)
- `parseSlashCommand(text: string)` — [`L236`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L236)
- `resolveBuiltinSlashCommandName(name: string)` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L243)
- `resolveSlashCommand(command: ParsedSlashCommand)` — [`L257`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L257)

## Module values
- `BUILTIN_SLASH_COMMANDS` — [`L229`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L229)
- `BUILTIN_SLASH_COMMAND_ALIASES` — [`L199`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L199)
- `BUILTIN_SLASH_COMMAND_ALIAS_TO_NAME` — [`L232`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L232)
- `BUILTIN_SLASH_COMMAND_BY_NAME` — [`L231`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L231)
- `CANONICAL_BUILTIN_SLASH_COMMANDS` — [`L87`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L87)
- `SESSION_SLASH_COMMAND_NAMES` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L13)
- `SESSION_SLASH_COMMAND_NAME_SET` — [`L17`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/slash-commands.ts#L17)

