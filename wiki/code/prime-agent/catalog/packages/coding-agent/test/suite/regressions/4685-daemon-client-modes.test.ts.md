---
title: 'Module: packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 test/suite/regressions/`4685-daemon-client-modes.test.ts`/
symbols:
  tempRoots: tempRoots.
  runCli.options-typeLiteral226.environment: runCli().(options)typeLiteral226:environment.
  runRpc: runRpc().
  runRpc.Promise.typeLiteral264.stdout: runRpc().Promise:typeLiteral264:stdout.
  runRpc.Promise.typeLiteral264.stderr: runRpc().Promise:typeLiteral264:stderr.
  children: children.
  harnesses: harnesses.
  daemonSockets: daemonSockets.
  runCli.options-typeLiteral226.agentDir: runCli().(options)typeLiteral226:agentDir.
  CliResult.stdout: CliResult#stdout.
  runCli: runCli().
  fauxExtensionPath: fauxExtensionPath.
  repoTsconfigPath: repoTsconfigPath.
  runCli.options-typeLiteral226.stdin: runCli().(options)typeLiteral226:stdin.
  tsxPath: tsxPath.
  fixturePath: fixturePath.
  rpcEofFauxExtensionPath: rpcEofFauxExtensionPath.
  cliPath: cliPath.
  CliResult: CliResult#
  CliResult.stderr: CliResult#stderr.
  runRpc.options-typeLiteral263.trailingNewline: runRpc().(options)typeLiteral263:trailingNewline.
  CliResult.code: CliResult#code.
  CliResult.signal: CliResult#signal.
---
# Module: [`packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts)

## Classes
### `CliResult`
- def: [`packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts:60`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L60)
- signature: `interface CliResult`
- members:
  - `code` — [`L61`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L61)
  - `signal` — [`L62`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L62)
  - `stderr` — [`L64`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L64)
  - `stdout` — [`L63`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L63)
- used by: (2 test-only callers)

## Functions
- `runCli(args: string[], options: { agentDir: string; stdin?: string | undefined; environment?: ProcessEnv | undefined; })` — [`L67`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L67)
- `runRpc(commands: unknown[], options?: { trailingNewline?: boolean | undefined; })` — [`L113`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L113)

## Module values
- `agentDir` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L69)
- `children` — [`L24`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L24)
- `cliPath` — [`L21`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L21)
- `daemonSockets` — [`L26`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L26)
- `environment` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L69)
- `fauxExtensionPath` — [`L19`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L19)
- `fixturePath` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L18)
- `harnesses` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L25)
- `repoTsconfigPath` — [`L23`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L23)
- `rpcEofFauxExtensionPath` — [`L20`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L20)
- `stderr` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L116)
- `stdin` — [`L69`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L69)
- `stdout` — [`L116`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L116)
- `tempRoots` — [`L27`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L27)
- `trailingNewline` — [`L115`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L115)
- `tsxPath` — [`L22`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/test/suite/regressions/4685-daemon-client-modes.test.ts#L22)

