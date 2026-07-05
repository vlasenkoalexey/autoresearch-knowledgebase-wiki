---
title: 'Module: extensions/pi-autoresearch-vkf/vkf.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/vkf.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`vkf.ts`/
symbols:
  validate: validate().
  run: run().
  check: check().
  graph: graph().
  html: html().
  freshness: freshness().
  VkfResult.stdout: VkfResult#stdout.
  VkfResult.stderr: VkfResult#stderr.
  cached: cached.
  VkfResult.unavailable: VkfResult#unavailable.
  freshness.typeLiteral74.report: freshness().typeLiteral74:report.
  resolveVkf: resolveVkf().
  GraphResult.edges: GraphResult#edges.
  VkfResult.ok: VkfResult#ok.
  GraphResult.nodes: GraphResult#nodes.
  isAvailable: isAvailable().
  GraphResult.available: GraphResult#available.
  freshness.typeLiteral74.available: freshness().typeLiteral74:available.
  VkfResult.code: VkfResult#code.
  ValidateReport.available: ValidateReport#available.
  ValidateReport.passed: ValidateReport#passed.
  html.typeLiteral67.ok: html().typeLiteral67:ok.
  ValidateReport.raw: ValidateReport#raw.
  GraphResult.raw: GraphResult#raw.
  html.typeLiteral67.available: html().typeLiteral67:available.
  html.typeLiteral67.raw: html().typeLiteral67:raw.
  freshness.typeLiteral74.raw: freshness().typeLiteral74:raw.
  CheckResult.available: CheckResult#available.
  CheckResult.allowed: CheckResult#allowed.
  CheckResult.requiresReview: CheckResult#requiresReview.
  CheckResult.reason: CheckResult#reason.
  CheckResult.raw: CheckResult#raw.
  resetVkfCache: resetVkfCache().
  VkfInvocation: VkfInvocation#
  ValidateReport.profile: ValidateReport#profile.
  ValidateReport.summary: ValidateReport#summary.
  ValidateReport.issues: ValidateReport#issues.
  html.typeLiteral67.out: html().typeLiteral67:out.
  VkfInvocation.file: VkfInvocation#file.
  VkfInvocation.prefixArgs: VkfInvocation#prefixArgs.
  VkfResult: VkfResult#
  condaEnv: condaEnv.
  ValidateReport: ValidateReport#
  ValidateReport.summary.typeLiteral31.ERROR: ValidateReport#summary.typeLiteral31:ERROR.
  GraphResult: GraphResult#
  CheckResult: CheckResult#
  ValidateReport.summary.typeLiteral31.WARNING: ValidateReport#summary.typeLiteral31:WARNING.
  ValidateReport.summary.typeLiteral31.INFO: ValidateReport#summary.typeLiteral31:INFO.
---
# Module: [`extensions/pi-autoresearch-vkf/vkf.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts)

## Classes
### `CheckResult`
- def: [`extensions/pi-autoresearch-vkf/vkf.ts:188`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L188) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- signature: `interface CheckResult`
- members:
  - `allowed` — [`L190`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L190) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `available` — [`L189`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L189) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `raw` — [`L193`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L193) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `reason` — [`L192`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L192) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `requiresReview` — [`L191`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L191) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- used by: [`check`](vkf.ts.md#check)

### `GraphResult`
- def: [`extensions/pi-autoresearch-vkf/vkf.ts:146`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L146) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- signature: `interface GraphResult`
- members:
  - `available` — [`L147`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L147) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `edges` — [`L149`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L149) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `nodes` — [`L148`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L148) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `raw` — [`L150`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L150) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`buildDashboardPayload`](index.ts.md#buildDashboardPayload), [`graph`](vkf.ts.md#graph)

### `ValidateReport`
- def: [`extensions/pi-autoresearch-vkf/vkf.ts:114`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L114) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- signature: `interface ValidateReport`
- members:
  - `ERROR` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L118)
  - `INFO` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L118)
  - `WARNING` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L118)
  - `available` — [`L115`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L115) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `issues` — [`L119`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L119) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `passed` — [`L116`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L116) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `profile` — [`L117`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L117) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `raw` — [`L120`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L120)
  - `summary` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L118) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- used by: [`validate`](vkf.ts.md#validate), [`validationNote`](index.ts.md#validationNote)

### `VkfInvocation`
- def: [`extensions/pi-autoresearch-vkf/vkf.ts:24`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L24) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- signature: `interface VkfInvocation`
- members:
  - `file` — [`L25`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L25) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `prefixArgs` — [`L26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L26) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- used by: [`run`](vkf.ts.md#run), [`cached`](vkf.ts.md#cached), [`resolveVkf`](vkf.ts.md#resolveVkf)

### `VkfResult`
- def: [`extensions/pi-autoresearch-vkf/vkf.ts:29`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L29) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- signature: `interface VkfResult`
- members:
  - `code` — [`L31`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L31) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `ok` — [`L30`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L30) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `stderr` — [`L33`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L33) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `stdout` — [`L32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L32) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
  - `unavailable` — [`L35`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L35) — Set when the CLI could not be located/spawned at all. — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- used by: [`validate`](vkf.ts.md#validate), [`run`](vkf.ts.md#run), [`check`](vkf.ts.md#check), [`graph`](vkf.ts.md#graph), [`html`](vkf.ts.md#html), [`freshness`](vkf.ts.md#freshness), [`isAvailable`](vkf.ts.md#isAvailable)

## Functions
- `check(filePath: string, use: string, role?: string | undefined)` — [`L197`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L197) — Run `vkf check <file> --use <ctx> [--role <role>] --format json`. — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `freshness(memoryDir: string)` — [`L178`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L178) — Run `vkf freshness <dir>` (JSON to stdout). — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `graph(memoryDir: string)` — [`L154`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L154) — Run `vkf graph <dir>` (JSON to stdout). — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `html(memoryDir: string, outPath: string, title?: string | undefined)` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L169) — Run `vkf html <dir> --out <path>` to write a self-contained interactive graph — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `isAvailable()` — [`L108`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L108) — True when the CLI appears to be installed and runnable. — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `resetVkfCache()` — [`L73`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L73) — Reset the cached CLI resolution (used by tests).
- `resolveVkf()` — [`L43`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L43) — Locate the `vkf` CLI. Returns `null` when nothing usable is found. — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `run(args: string[], cwd?: string | undefined)` — [`L77`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L77) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `validate(memoryDir: string, profile: number)` — [`L124`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L124) — Run `vkf validate <dir> --profile N --format json`. — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)

## Module values
- `available` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L169)
- `available` — [`L178`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L178)
- `cached` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L40) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `condaEnv` — [`L38`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L38) — documented in [extensions-pi-autoresearch-vkf-vkf.ts](../../../concepts/extensions-pi-autoresearch-vkf-vkf.ts.md)
- `ok` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L169)
- `out` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L169)
- `raw` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L169)
- `raw` — [`L178`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L178)
- `report` — [`L178`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/vkf.ts#L178)

