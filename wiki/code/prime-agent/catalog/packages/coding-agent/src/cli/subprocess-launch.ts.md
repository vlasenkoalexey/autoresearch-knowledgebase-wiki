---
title: 'Module: packages/coding-agent/src/cli/subprocess-launch.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/subprocess-launch.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`subprocess-launch.ts`/
symbols:
  createCliSubprocessLaunchSpec: createCliSubprocessLaunchSpec().
  formatCurrentCliCommand: formatCurrentCliCommand().
  createCliSubprocessEnv: createCliSubprocessEnv().
  CliSubprocessLaunchSpec.args: CliSubprocessLaunchSpec#args.
  CliSubprocessLaunchSpec.command: CliSubprocessLaunchSpec#command.
  CliSubprocessLaunchSpec: CliSubprocessLaunchSpec#
  quoteCommandArgument: quoteCommandArgument().
---
# Module: [`packages/coding-agent/src/cli/subprocess-launch.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts)

## Classes
### `CliSubprocessLaunchSpec`
- def: [`packages/coding-agent/src/cli/subprocess-launch.ts:5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L5)
- signature: `interface CliSubprocessLaunchSpec`
- members:
  - `args` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L7)
  - `command` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L6)
- used by: [`launchWorker`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.launchWorker), [`shutdown`](../modes/daemon/daemon-supervisor.ts.md#DaemonSupervisor.shutdown), [`launchDaemonUpdateRestartCoordinator`](daemon-update-restart.ts.md#launchDaemonUpdateRestartCoordinator), [`owned-session-worker.ts`](owned-session-worker.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-cli-owned-session-worker.ts), [`launchReplacementSupervisor`](../modes/daemon/daemon-mode.ts.md#AgentDaemon.launchReplacementSupervisor), [`runOwnedSessionWorkerFrontend`](owned-session-worker.ts.md#runOwnedSessionWorkerFrontend), [`createCliSubprocessLaunchSpec`](subprocess-launch.ts.md#createCliSubprocessLaunchSpec), [`spawnCatalog`](../modes/daemon/daemon-catalog-process.ts.md#DaemonCatalogClient.spawnCatalog), [`formatCurrentCliCommand`](subprocess-launch.ts.md#formatCurrentCliCommand), [`OwnedWorkerLaunchSpec`](owned-session-worker.ts.md#OwnedWorkerLaunchSpec)  (1 test-only)

## Functions
- `createCliSubprocessEnv(source?: ProcessEnv, entrypoint?: string, execArgs?: readonly string[])` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L10)
- `createCliSubprocessLaunchSpec(args: readonly string[], executable?: string, execArgs?: readonly string[], entrypoint?: string)` — [`L47`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L47)
- `formatCurrentCliCommand(args: readonly string[], environment?: ProcessEnv)` — [`L38`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L38)
- `quoteCommandArgument(value: string)` — [`L34`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/subprocess-launch.ts#L34)

