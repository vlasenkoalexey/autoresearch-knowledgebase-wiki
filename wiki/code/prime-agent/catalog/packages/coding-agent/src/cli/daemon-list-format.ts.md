---
title: 'Module: packages/coding-agent/src/cli/daemon-list-format.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/cli/daemon-list-format.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/cli/`daemon-list-format.ts`/
symbols:
  formatSessionListTable: formatSessionListTable().
  listStatusForSummary: listStatusForSummary().
  formatSessionModel: formatSessionModel().
  sortSessionsForList: sortSessionsForList().
  formatListCell: formatListCell().
  LIST_STATUS_ORDER: LIST_STATUS_ORDER.
  ListRow.typeLiteral0.status: ListRow#typeLiteral0:status.
  ListStatus: ListStatus#
  ListRow: ListRow#
  formatSessionAge: formatSessionAge().
  formatTable: formatTable().
  ListRow.typeLiteral0.name: ListRow#typeLiteral0:name.
  ListRow.typeLiteral0.id: ListRow#typeLiteral0:id.
  ListRow.typeLiteral0.age: ListRow#typeLiteral0:age.
  ListRow.typeLiteral0.model: ListRow#typeLiteral0:model.
  ListRow.typeLiteral0.messages: ListRow#typeLiteral0:messages.
  ListRow.typeLiteral0.clients: ListRow#typeLiteral0:clients.
---
# Module: [`packages/coding-agent/src/cli/daemon-list-format.ts`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts)

## Classes
### `ListRow`
- def: [`packages/coding-agent/src/cli/daemon-list-format.ts:21`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L21)
- signature: `type ListRow`
- members:
  - `age` — [`L25`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L25)
  - `clients` — [`L28`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L28)
  - `id` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L23)
  - `messages` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L27)
  - `model` — [`L26`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L26)
  - `name` — [`L22`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L22)
  - `status` — [`L24`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L24)
- uses (calls/refs, reference-scoped): [`ListStatus`](daemon-list-format.ts.md#ListStatus)
- used by: [`formatListCell`](daemon-list-format.ts.md#formatListCell)

### `ListStatus`
- def: [`packages/coding-agent/src/cli/daemon-list-format.ts:6`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L6)
- signature: `type ListStatus`
- used by: [`listStatusForSummary`](daemon-list-format.ts.md#listStatusForSummary), [`LIST_STATUS_ORDER`](daemon-list-format.ts.md#LIST_STATUS_ORDER), [`status`](daemon-list-format.ts.md#ListRow.typeLiteral0.status)

## Functions
- `formatListCell(row: ListRow, column: keyof ListRow, value: string)` — [`L56`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L56)
- `formatSessionAge(modified: string | undefined, nowMs: number)` — [`L71`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L71)
- `formatSessionListTable(sessions: readonly SessionSummary[], nowMs?: number)` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L31)
- `formatSessionModel(model: Model<Api> | undefined)` — [`L102`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L102)
- `formatTable(columns: (keyof T)[], rows: T[], formatCell?: ((row: T, column: keyof T, value: string) => string) | undefined)` — [`L106`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L106)
- `listStatusForSummary(summary: SessionSummary)` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L14)
- `sortSessionsForList(sessions: readonly SessionSummary[])` — [`L44`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L44)

## Module values
- `LIST_STATUS_ORDER` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/cli/daemon-list-format.ts#L8)

