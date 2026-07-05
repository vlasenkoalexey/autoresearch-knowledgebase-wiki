---
title: 'Module: extensions/pi-autoresearch-vkf/dashboard.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/dashboard.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`dashboard.ts`/
symbols:
  buildFullscreenLines: buildFullscreenLines().
  buildWidgetLines: buildWidgetLines().
  experimentLine: experimentLine().
  loopLine: loopLine().
  runsTable: runsTable().
  coverageLine: coverageLine().
  memoryCounts: memoryCounts().
  readUpdates: readUpdates().
  statusLabel: statusLabel().
  renderTable: renderTable().
  shortcutHint: shortcutHint().
  memoryLine: memoryLine().
  updateLine: updateLine().
  trimNum: trimNum.
  TableStyle.header: TableStyle#header.
  TableStyle.rule: TableStyle#rule.
  TableStyle.cell: TableStyle#cell.
  WIDGET_ROWS: WIDGET_ROWS.
  ALT_ABBR: ALT_ABBR.
  TableStyle: TableStyle#
---
# Module: [`extensions/pi-autoresearch-vkf/dashboard.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts)

## Classes
### `TableStyle`
- def: [`extensions/pi-autoresearch-vkf/dashboard.ts:172`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L172)
- doc: Optional per-element styling for {@link renderTable}.
- signature: `interface TableStyle`
- members:
  - `cell` — [`L178`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L178) — Wraps a body cell. `text` is already padded; `col`/`row` are 0-based.
  - `header` — [`L174`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L174) — Wraps each header cell (after padding).
  - `rule` — [`L176`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L176) — Wraps the whole rule line.
- used by: [`renderTable`](dashboard.ts.md#renderTable)

## Functions
- `buildFullscreenLines(root: string)` — [`L311`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L311) — Full status for the fullscreen overlay. — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `buildWidgetLines(root: string)` — [`L277`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L277) — Compact widget shown above the editor. Returns `[]` when there is no session. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `coverageLine(root: string)` — [`L136`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L136) — The rut-detector: how the experiments we've actually run spread across — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `experimentLine(root: string)` — [`L56`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L56) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `loopLine(root: string, config: ResearchConfig)` — [`L86`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L86) — The loop-state line: session mode, autonomy, budget burn, and the user's — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `memoryCounts(root: string)` — [`L46`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L46) — documented in [extensions-pi-autoresearch-vkf-cards.ts](../../../concepts/extensions-pi-autoresearch-vkf-cards.ts.md)
- `memoryLine(root: string)` — [`L70`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L70) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `readUpdates(root: string)` — [`L105`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L105) — Agent research updates (research_update tool), oldest first. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `renderTable(headers: string[], rows: string[][], align: ("l" | "r")[], ts?: TableStyle)` — [`L189`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L189) — Render a fixed-width text table: header row, a rule, then the body rows. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `runsTable(root: string, metricName: string)` — [`L228`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L228) — The recent-runs table: # · commit · each metric · status · description. — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `shortcutHint()` — [`L35`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L35) — A one-line footer advertising the configured shortcuts (the "buttons"). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `statusLabel(e: Experiment)` — [`L166`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L166) — keep / discard if decided, otherwise the raw outcome (win/loss/…). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
- `updateLine(root: string)` — [`L115`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L115) — The latest agent update as a one-liner — the in-terminal mirror of the — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)

## Module values
- `ALT_ABBR` — [`L123`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L123)
- `WIDGET_ROWS` — [`L32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L32) — How many recent runs the live widget table shows.
- `trimNum` — [`L43`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/dashboard.ts#L43) — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)

