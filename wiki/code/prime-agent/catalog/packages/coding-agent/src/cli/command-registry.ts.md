---
title: 'Module: packages/coding-agent/src/cli/command-registry.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/command-registry.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`command-registry.ts`/
symbols:
  CommandSpec.path: CommandSpec#path.
  CommandSpec.usage: CommandSpec#usage.
  CommandSpec.summary: CommandSpec#summary.
  formatTopLevelHelp: formatTopLevelHelp().
  formatCommandHelp: formatCommandHelp().
  COMMAND_SPECS: COMMAND_SPECS.
  getCommandSpec: getCommandSpec().
  isHelpCommandRequest: isHelpCommandRequest().
  TOP_LEVEL_OPTION_GROUPS.ReadonlyArray.typeLiteral8.options: TOP_LEVEL_OPTION_GROUPS.ReadonlyArray:typeLiteral8:options.
  getChildCommandSpecs: getChildCommandSpecs().
  PUBLIC_COMMAND_NAMES: PUBLIC_COMMAND_NAMES.
  CommandSpec.options: CommandSpec#options.
  findCommandSuggestion: findCommandSuggestion().
  REMOVED_COMMAND_NAMES: REMOVED_COMMAND_NAMES.
  TOP_LEVEL_OPTION_GROUPS.ReadonlyArray.typeLiteral8.heading: TOP_LEVEL_OPTION_GROUPS.ReadonlyArray:typeLiteral8:heading.
  CommandSpec.description: CommandSpec#description.
  CommandSpec.examples: CommandSpec#examples.
  formatOptionGroup: formatOptionGroup().
  CommandSpec: CommandSpec#
  TopLevelOption: TopLevelOption#
  TOP_LEVEL_OPTION_GROUPS: TOP_LEVEL_OPTION_GROUPS.
  editDistance: editDistance().
---
# Module: [`packages/coding-agent/src/cli/command-registry.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts)

## Classes
### `CommandSpec`
- def: [`packages/coding-agent/src/cli/command-registry.ts:3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L3)
- signature: `interface CommandSpec`
- members:
  - `description` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L7)
  - `examples` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L9)
  - `options` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L8)
  - `path` — [`L4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L4)
  - `summary` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L6)
  - `usage` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L5)
- used by: [`runPublicCommand`](public-command.ts.md#runPublicCommand), [`printRequestedHelp`](public-command.ts.md#printRequestedHelp), [`formatTopLevelHelp`](command-registry.ts.md#formatTopLevelHelp), [`formatCommandHelp`](command-registry.ts.md#formatCommandHelp), [`rewriteNestedCommand`](public-command.ts.md#rewriteNestedCommand), [`runNestedAgentCommand`](public-command.ts.md#runNestedAgentCommand), [`runPackage`](public-command.ts.md#runPackage), [`COMMAND_SPECS`](command-registry.ts.md#COMMAND_SPECS), [`getCommandSpec`](command-registry.ts.md#getCommandSpec), [`isHelpCommandRequest`](command-registry.ts.md#isHelpCommandRequest), [`getChildCommandSpecs`](command-registry.ts.md#getChildCommandSpecs), [`PUBLIC_COMMAND_NAMES`](command-registry.ts.md#PUBLIC_COMMAND_NAMES), [`requireOperandCount`](public-command.ts.md#requireOperandCount), [`requireArgumentCount`](public-command.ts.md#requireArgumentCount), [`validateScheduleArgs`](public-command.ts.md#validateScheduleArgs)

### `TopLevelOption`
- def: [`packages/coding-agent/src/cli/command-registry.ts:161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L161)
- signature: `type TopLevelOption`
- used by: [`options`](command-registry.ts.md#TOP_LEVEL_OPTION_GROUPS.ReadonlyArray.typeLiteral8.options), [`formatOptionGroup`](command-registry.ts.md#formatOptionGroup)

## Functions
- `editDistance(left: string, right: string)` — [`L336`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L336)
- `findCommandSuggestion(input: string, candidates: readonly string[])` — [`L271`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L271)
- `formatCommandHelp(path: readonly string[])` — [`L309`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L309)
- `formatOptionGroup(heading: string, options: readonly TopLevelOption[])` — [`L304`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L304)
- `formatTopLevelHelp()` — [`L285`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L285)
- `getChildCommandSpecs(path: readonly string[])` — [`L250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L250)
- `getCommandSpec(path: readonly string[])` — [`L244`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L244)
- `isHelpCommandRequest(path: readonly string[])` — [`L256`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L256)

## Module values
- `COMMAND_SPECS` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L12)
- `PUBLIC_COMMAND_NAMES` — [`L155`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L155)
- `REMOVED_COMMAND_NAMES` — [`L159`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L159)
- `TOP_LEVEL_OPTION_GROUPS` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L163)
- `heading` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L163)
- `options` — [`L163`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/command-registry.ts#L163)

