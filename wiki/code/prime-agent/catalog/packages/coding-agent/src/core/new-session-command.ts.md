---
title: 'Module: packages/coding-agent/src/core/new-session-command.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/core/new-session-command.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/core/`new-session-command.ts`/
symbols:
  parseNewSessionCommand: parseNewSessionCommand().
  requireNewPrompt: requireNewPrompt().
  consumeNewSeparator: consumeNewSeparator().
  ParsedNewSessionCommand.prompt: ParsedNewSessionCommand#prompt.
  ParsedNewSessionCommand.name: ParsedNewSessionCommand#name.
  ParsedNewSessionCommand: ParsedNewSessionCommand#
---
# Module: [`packages/coding-agent/src/core/new-session-command.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts)

## Classes
### `ParsedNewSessionCommand`
- def: [`packages/coding-agent/src/core/new-session-command.ts:1`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L1)
- signature: `interface ParsedNewSessionCommand`
- members:
  - `name` — [`L2`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L2)
  - `prompt` — [`L3`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L3)
- used by: [`parseNewSessionCommand`](new-session-command.ts.md#parseNewSessionCommand)

## Functions
- `consumeNewSeparator(value: string, error: string)` — [`L42`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L42)
- `parseNewSessionCommand(rawArgs: string)` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L7) — Parse /new's raw suffix while preserving the initial prompt verbatim.
- `requireNewPrompt(value: string)` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/core/new-session-command.ts#L50)

