---
title: 'Module: extensions/pi-autoresearch-vkf/metrics.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/metrics.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`metrics.ts`/
symbols:
  parseMetrics: parseMetrics().
  readMetric: readMetric().
  METRIC_RE: METRIC_RE.
---
# Module: [`extensions/pi-autoresearch-vkf/metrics.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/metrics.ts)

## Functions
- `parseMetrics(output: string)` — [`L13`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/metrics.ts#L13) — Extract all `METRIC name=value` pairs from text, last-wins on duplicates.
- `readMetric(output: string, name: string)` — [`L23`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/metrics.ts#L23) — Pick a specific metric by name from command output, if present.

## Module values
- `METRIC_RE` — [`L10`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/metrics.ts#L10) — Parse `METRIC name=number` lines from experiment command output.

