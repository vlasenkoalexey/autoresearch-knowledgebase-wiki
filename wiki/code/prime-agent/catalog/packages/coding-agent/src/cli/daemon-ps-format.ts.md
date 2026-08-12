---
title: 'Module: packages/coding-agent/src/cli/daemon-ps-format.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-ps-format.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-ps-format.ts`/
symbols:
  formatDaemonListTable: formatDaemonListTable().
  formatUptime: formatUptime().
  formatDaemonCell: formatDaemonCell().
  colorStatus: colorStatus().
  DaemonRow: DaemonRow#
  formatTable: formatTable().
  DaemonRow.typeLiteral0.socket: DaemonRow#typeLiteral0:socket.
  DaemonRow.typeLiteral0.pid: DaemonRow#typeLiteral0:pid.
  DaemonRow.typeLiteral0.version: DaemonRow#typeLiteral0:version.
  DaemonRow.typeLiteral0.status: DaemonRow#typeLiteral0:status.
  DaemonRow.typeLiteral0.sessions: DaemonRow#typeLiteral0:sessions.
  DaemonRow.typeLiteral0.uptime: DaemonRow#typeLiteral0:uptime.
---
# Module: [`packages/coding-agent/src/cli/daemon-ps-format.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts)

## Classes
### `DaemonRow`
- def: [`packages/coding-agent/src/cli/daemon-ps-format.ts:4`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L4)
- signature: `type DaemonRow`
- members:
  - `pid` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L6)
  - `sessions` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L9)
  - `socket` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L5)
  - `status` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L8)
  - `uptime` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L10)
  - `version` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L7)
- used by: [`formatDaemonCell`](daemon-ps-format.ts.md#formatDaemonCell)

## Functions
- `colorStatus(status: DaemonStatus, value: string)` — [`L35`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L35)
- `formatDaemonCell(_row: DaemonRow, column: keyof DaemonRow, value: string)` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L28)
- `formatDaemonListTable(daemons: readonly DaemonInfo[])` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L13)
- `formatTable(columns: (keyof T)[], rows: T[], formatCell?: ((row: T, column: keyof T, value: string) => string) | undefined)` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L71)
- `formatUptime(uptimeSeconds: number | undefined)` — [`L48`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-ps-format.ts#L48)

