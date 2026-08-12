---
title: 'Module: packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/`daemon-serialized-refine-process.test.ts`/
symbols:
  runCli.Promise.typeLiteral227.stderr: runCli().Promise:typeLiteral227:stderr.
  tempRoots: tempRoots.
  children: children.
  readEventLog: readEventLog().
  daemonSockets: daemonSockets.
  EventLogEntry.type: EventLogEntry#type.
  runCli.options-typeLiteral226.agentDir: runCli().(options)typeLiteral226:agentDir.
  runCli.options-typeLiteral226.environment: runCli().(options)typeLiteral226:environment.
  EventLogEntry: EventLogEntry#
  EventLogEntry.seq: EventLogEntry#seq.
  cliPath: cliPath.
  tsxPath: tsxPath.
  repoTsconfigPath: repoTsconfigPath.
  fauxRefineExtensionPath: fauxRefineExtensionPath.
  eventOrderExtensionPath: eventOrderExtensionPath.
  runCli: runCli().
  runCli.options-typeLiteral226.stdin: runCli().(options)typeLiteral226:stdin.
  writeAutoRefineSettings: writeAutoRefineSettings().
  runCli.Promise.typeLiteral227.code: runCli().Promise:typeLiteral227:code.
  runCli.Promise.typeLiteral227.signal: runCli().Promise:typeLiteral227:signal.
  runCli.Promise.typeLiteral227.stdout: runCli().Promise:typeLiteral227:stdout.
---
# Module: [`packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts)

## Classes
### `EventLogEntry`
- def: [`packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts:135`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L135)
- signature: `interface EventLogEntry`
- members:
  - `seq` — [`L136`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L136)
  - `type` — [`L137`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L137)
- used by: (2 test-only callers)

## Functions
- `readEventLog(path: string)` — [`L141`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L141)
- `runCli(args: string[], options: { agentDir: string; stdin?: string | undefined; environment?: ProcessEnv | undefined; })` — [`L82`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L82)
- `writeAutoRefineSettings(agentDir: string)` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L151)

## Module values
- `agentDir` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L84)
- `children` — [`L50`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L50)
- `cliPath` — [`L45`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L45)
- `code` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L85)
- `daemonSockets` — [`L51`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L51)
- `environment` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L84)
- `eventOrderExtensionPath` — [`L49`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L49)
- `fauxRefineExtensionPath` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L48)
- `repoTsconfigPath` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L47)
- `signal` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L85)
- `stderr` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L85)
- `stdin` — [`L84`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L84)
- `stdout` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L85)
- `tempRoots` — [`L52`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L52)
- `tsxPath` — [`L46`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/daemon-serialized-refine-process.test.ts#L46)

