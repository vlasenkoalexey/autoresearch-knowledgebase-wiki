---
title: 'Module: packages/coding-agent/src/cli/public-command.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/public-command.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`public-command.ts`/
symbols:
  runPublicCommand: runPublicCommand().
  handlePublicCommand: handlePublicCommand().
  HANDLED: HANDLED.
  printRequestedHelp: printRequestedHelp().
  fail: fail().
  rewriteNestedCommand: rewriteNestedCommand().
  runNestedAgentCommand: runNestedAgentCommand().
  runPackage: runPackage().
  continueWith: continueWith().
  PublicCommandResult: PublicCommandResult#
  runDoctor: runDoctor().
  requireOperandCount: requireOperandCount().
  runInternalAgentCommand: runInternalAgentCommand().
  runStatus: runStatus().
  runShutdown: runShutdown().
  requireArgumentCount: requireArgumentCount().
  validateScheduleArgs: validateScheduleArgs().
  hasPositionalArguments: hasPositionalArguments().
  parseBooleanOptions: parseBooleanOptions().
  rejectRemovedCommand: rejectRemovedCommand().
  PublicCommandResult.attachAgent: PublicCommandResult#attachAgent.
  getCommandPath: getCommandPath().
  splitOperandsAndOptions: splitOperandsAndOptions().
  PublicCommandResult.handled: PublicCommandResult#handled.
  PublicCommandResult.args: PublicCommandResult#args.
  PublicCommandResult.explicitAgentsView: PublicCommandResult#explicitAgentsView.
  normalizeLeadingDaemonSocketOption: normalizeLeadingDaemonSocketOption().
  hasConflictingAttachOption: hasConflictingAttachOption().
---
# Module: [`packages/coding-agent/src/cli/public-command.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts)

## Classes
### `PublicCommandResult`
- def: [`packages/coding-agent/src/cli/public-command.ts:19`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L19)
- signature: `interface PublicCommandResult`
- members:
  - `args` — [`L21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L21)
  - `attachAgent` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L23)
  - `explicitAgentsView` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L22)
  - `handled` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L20)
- used by: [`main`](../main.ts.md#main), [`runPublicCommand`](public-command.ts.md#runPublicCommand), [`handlePublicCommand`](public-command.ts.md#handlePublicCommand), [`HANDLED`](public-command.ts.md#HANDLED), [`printRequestedHelp`](public-command.ts.md#printRequestedHelp), [`fail`](public-command.ts.md#fail), [`rewriteNestedCommand`](public-command.ts.md#rewriteNestedCommand), [`runNestedAgentCommand`](public-command.ts.md#runNestedAgentCommand), [`runPackage`](public-command.ts.md#runPackage), [`continueWith`](public-command.ts.md#continueWith), [`runDoctor`](public-command.ts.md#runDoctor), [`runInternalAgentCommand`](public-command.ts.md#runInternalAgentCommand), [`runShutdown`](public-command.ts.md#runShutdown), [`runStatus`](public-command.ts.md#runStatus), [`rejectRemovedCommand`](public-command.ts.md#rejectRemovedCommand)

## Functions
- `continueWith(args: string[])` — [`L161`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L161)
- `fail(message: string, hint?: string | undefined)` — [`L428`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L428)
- `getCommandPath(args: string[])` — [`L187`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L187)
- `handlePublicCommand(args: string[])` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L28)
- `hasConflictingAttachOption(args: string[])` — [`L354`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L354)
- `hasPositionalArguments(args: string[])` — [`L349`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L349)
- `normalizeLeadingDaemonSocketOption(args: string[])` — [`L148`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L148)
- `parseBooleanOptions(args: string[], allowed: ReadonlySet<string>, command: string)` — [`L329`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L329)
- `printRequestedHelp(path: string[])` — [`L165`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L165)
- `rejectRemovedCommand(args: string[])` — [`L198`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L198)
- `requireArgumentCount(args: string[], count: number, command: string)` — [`L341`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L341)
- `requireOperandCount(args: string[], minimum: number, maximum: number | undefined, command: string)` — [`L378`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L378)
- `rewriteNestedCommand(parent: string, subcommand: string, flag: string, args: string[])` — [`L306`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L306)
- `runDoctor(args: string[])` — [`L250`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L250)
- `runInternalAgentCommand(command: string, args: string[])` — [`L215`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L215)
- `runNestedAgentCommand(parent: string, internalCommand: string, args: string[])` — [`L220`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L220)
- `runPackage(args: string[])` — [`L268`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L268)
- `runPublicCommand(args: string[])` — [`L36`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L36)
- `runShutdown(args: string[])` — [`L261`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L261)
- `runStatus(args: string[])` — [`L243`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L243)
- `splitOperandsAndOptions(args: string[])` — [`L366`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L366)
- `validateScheduleArgs(args: string[])` — [`L402`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L402)

## Module values
- `HANDLED` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/public-command.ts#L26)

