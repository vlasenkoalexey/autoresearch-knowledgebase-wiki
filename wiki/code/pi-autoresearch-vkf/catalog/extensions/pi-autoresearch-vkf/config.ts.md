---
title: 'Module: extensions/pi-autoresearch-vkf/config.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/config.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`config.ts`/
symbols:
  makeConfig: makeConfig().
  researchMode: researchMode().
  readConfig: readConfig().
  sessionMode: sessionMode().
  ResearchConfig.metricName: ResearchConfig#metricName.
  autonomyMode: autonomyMode().
  ResearchConfig.name: ResearchConfig#name.
  ResearchConfig.direction: ResearchConfig#direction.
  MetricDirection: MetricDirection#
  ResearchConfig: ResearchConfig#
  ResearchConfig.owner: ResearchConfig#owner.
  ResearchConfig.maxIterations: ResearchConfig#maxIterations.
  deriveResearchMode: deriveResearchMode().
  ResearchConfig.goal: ResearchConfig#goal.
  ResearchConfig.memoryProfile: ResearchConfig#memoryProfile.
  ResearchConfig.altitudePreference: ResearchConfig#altitudePreference.
  researchMode.typeLiteral7.altitudePreference: researchMode().typeLiteral7:altitudePreference.
  writeConfig: writeConfig().
  AltitudePreference: AltitudePreference#
  ResearchConfig.baseline: ResearchConfig#baseline.
  researchMode.typeLiteral7.exploreFraction: researchMode().typeLiteral7:exploreFraction.
  ResearchConfig.exploreFraction: ResearchConfig#exploreFraction.
  AutonomyMode: AutonomyMode#
  ResearchConfig.command: ResearchConfig#command.
  ResearchConfig.autonomy: ResearchConfig#autonomy.
  ResearchConfig.mode: ResearchConfig#mode.
  makeConfig.params-typeLiteral14.direction: makeConfig().(params)typeLiteral14:direction.
  makeConfig.params-typeLiteral14.autonomy: makeConfig().(params)typeLiteral14:autonomy.
  SessionMode: SessionMode#
  ResearchConfig.workingDir: ResearchConfig#workingDir.
  deriveResearchMode.typeLiteral3.exploreFraction: deriveResearchMode().typeLiteral3:exploreFraction.
  deriveResearchMode.typeLiteral3.altitudePreference: deriveResearchMode().typeLiteral3:altitudePreference.
  makeConfig.params-typeLiteral14.altitudePreference: makeConfig().(params)typeLiteral14:altitudePreference.
  makeConfig.params-typeLiteral14.goal: makeConfig().(params)typeLiteral14:goal.
  makeConfig.params-typeLiteral14.name: makeConfig().(params)typeLiteral14:name.
  makeConfig.params-typeLiteral14.command: makeConfig().(params)typeLiteral14:command.
  makeConfig.params-typeLiteral14.metricName: makeConfig().(params)typeLiteral14:metricName.
  makeConfig.params-typeLiteral14.filesInScope: makeConfig().(params)typeLiteral14:filesInScope.
  makeConfig.params-typeLiteral14.workingDir: makeConfig().(params)typeLiteral14:workingDir.
  makeConfig.params-typeLiteral14.maxIterations: makeConfig().(params)typeLiteral14:maxIterations.
  makeConfig.params-typeLiteral14.memoryProfile: makeConfig().(params)typeLiteral14:memoryProfile.
  ResearchConfig.filesInScope: ResearchConfig#filesInScope.
  ResearchConfig.createdAt: ResearchConfig#createdAt.
  DEFAULT_OWNER: DEFAULT_OWNER.
  DEFAULT_MEMORY_PROFILE: DEFAULT_MEMORY_PROFILE.
  makeConfig.params-typeLiteral14.exploreFraction: makeConfig().(params)typeLiteral14:exploreFraction.
  makeConfig.params-typeLiteral14.owner: makeConfig().(params)typeLiteral14:owner.
---
# Module: [`extensions/pi-autoresearch-vkf/config.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts)

## Classes
### `AltitudePreference`
- def: [`extensions/pi-autoresearch-vkf/config.ts:19`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L19) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- doc: How strongly idea selection should favor higher-altitude (less incremental)
- signature: `type AltitudePreference`
- used by: [`researchMode`](config.ts.md#researchMode), [`scoring.ts`](scoring.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-scoring.ts), [`deriveResearchMode`](config.ts.md#deriveResearchMode), [`altitudePreference`](config.ts.md#ResearchConfig.altitudePreference), [`ScoreOptions`](scoring.ts.md#ScoreOptions), [`ALTITUDE_AFFINITY`](scoring.ts.md#ALTITUDE_AFFINITY), [`altitudePreference`](config.ts.md#makeConfig.params-typeLiteral14.altitudePreference)

### `AutonomyMode`
- def: [`extensions/pi-autoresearch-vkf/config.ts:27`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L27) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- doc: Whether the loop is pre-authorized to keep iterating without checking in.
- signature: `type AutonomyMode`
- used by: [`autonomyMode`](config.ts.md#autonomyMode), [`autonomy.ts`](autonomy.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-autonomy.ts), [`autonomy`](autonomy.ts.md#AutonomySnapshot.autonomy), [`autonomy`](config.ts.md#ResearchConfig.autonomy), [`autonomy`](config.ts.md#makeConfig.params-typeLiteral14.autonomy)

### `MetricDirection`
- def: [`extensions/pi-autoresearch-vkf/config.ts:12`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L12) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- doc: Which direction of the metric counts as an improvement.
- signature: `type MetricDirection`
- used by: [`summarize`](experiments.ts.md#summarize), [`progress_data.ts`](progress_data.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-progress_data.ts), [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`direction`](config.ts.md#ResearchConfig.direction), [`bestNode`](tree.ts.md#bestNode), [`frontier`](tree.ts.md#frontier), [`experiments.ts`](experiments.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-experiments.ts), [`bestValue`](progress_data.ts.md#bestValue), [`deriveOutcome`](experiments.ts.md#deriveOutcome), [`direction`](progress_data.ts.md#BuildDashboardInput.direction), [`direction`](config.ts.md#makeConfig.params-typeLiteral14.direction), [`direction`](tree.ts.md#selectExpansion.opts-typeLiteral110.direction), [`direction`](progress_data.ts.md#DashboardData.direction)

### `ResearchConfig`
- def: [`extensions/pi-autoresearch-vkf/config.ts:37`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L37) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- signature: `interface ResearchConfig`
- members:
  - `altitudePreference` — [`L62`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L62) — Altitude bias for scoring (see {@link AltitudePreference}). — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `autonomy` — [`L64`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L64) — Loop autonomy (see {@link AutonomyMode}). Missing (legacy) ⇒ continuous. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `baseline` — [`L49`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L49) — Baseline metric value before any change (filled once measured). — documented in [extensions-pi-autoresearch-vkf-dashboard.ts](../../../concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md)
  - `command` — [`L43`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L43) — Command (run via `bash -lc`) that prints `METRIC name=number` lines. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `createdAt` — [`L70`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L70) — ISO timestamp the session was created. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `direction` — [`L47`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L47) — Which direction is better. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `exploreFraction` — [`L60`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L60) — Fraction of the experiment budget reserved for exploratory (high-altitude / — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `filesInScope` — [`L51`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L51) — Files/globs the loop is allowed to modify. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `goal` — [`L41`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L41) — The research goal / optimization objective, in words. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `maxIterations` — [`L55`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L55) — Optional cap on loop iterations. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `memoryProfile` — [`L57`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L57) — VKF conformance profile the memory bundle commits to (1 governed, 2 verified). — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `metricName` — [`L45`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L45) — Display name of the metric being optimized, e.g. "wall_clock_s". — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `mode` — [`L66`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L66) — Session kind (see {@link SessionMode}). Missing (legacy) ⇒ optimize. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `name` — [`L39`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L39) — Human-readable session name, e.g. "Speed up the test suite". — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `owner` — [`L68`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L68) — Actor id recorded as the owner/author of agent-written VKF objects. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
  - `workingDir` — [`L53`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L53) — Working directory for experiment commands (defaults to project root). — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- uses (calls/refs, reference-scoped): [`MetricDirection`](config.ts.md#MetricDirection), [`AltitudePreference`](config.ts.md#AltitudePreference), [`AutonomyMode`](config.ts.md#AutonomyMode), [`SessionMode`](config.ts.md#SessionMode)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`buildDashboardPayload`](index.ts.md#buildDashboardPayload), [`makeConfig`](config.ts.md#makeConfig), [`dashboard.ts`](dashboard.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-dashboard.ts), [`buildFullscreenLines`](dashboard.ts.md#buildFullscreenLines), [`buildWidgetLines`](dashboard.ts.md#buildWidgetLines), [`experimentLine`](dashboard.ts.md#experimentLine), [`loopLine`](dashboard.ts.md#loopLine), [`researchMode`](config.ts.md#researchMode), [`resolveRoot`](runtime.ts.md#resolveRoot), [`readConfig`](config.ts.md#readConfig), [`continuationNote`](index.ts.md#continuationNote), [`promptStub`](index.ts.md#promptStub), [`sessionMode`](config.ts.md#sessionMode), [`autonomyMode`](config.ts.md#autonomyMode), [`writeConfig`](config.ts.md#writeConfig)

### `SessionMode`
- def: [`extensions/pi-autoresearch-vkf/config.ts:35`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L35) — documented in [extensions-pi-autoresearch-vkf-autonomy.ts](../../../concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md)
- doc: What kind of session this is. `optimize` (default): the classic loop against a
- signature: `type SessionMode`
- used by: [`sessionMode`](config.ts.md#sessionMode), [`autonomy.ts`](autonomy.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-autonomy.ts), [`sessionMode`](autonomy.ts.md#AutonomySnapshot.sessionMode), [`mode`](config.ts.md#ResearchConfig.mode)

## Functions
- `autonomyMode(config: ResearchConfig)` — [`L108`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L108) — The effective autonomy mode for a config (legacy configs ⇒ continuous).
- `deriveResearchMode(goal: string)` — [`L82`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L82) — Pick the default research mode from the goal text. An explicit tuning goal — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `makeConfig(params: { name: string; goal: string; command?: string | undefined; metricName?: string | undefined; direction?: MetricDirection | undefined; filesInScope?: string[] | undefined; ... 6 more ...; owner?: string | undefined; })` — [`L129`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L129) — Build a config from init params, applying defaults. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `readConfig(configPath: string)` — [`L117`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L117) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `researchMode(config: ResearchConfig)` — [`L96`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L96) — The effective explore/exploit mode for a config, falling back to a goal-derived — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `sessionMode(config: ResearchConfig)` — [`L113`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L113) — The effective session mode (legacy configs ⇒ optimize). — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `writeConfig(configPath: string, config: ResearchConfig)` — [`L124`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L124)

## Module values
- `DEFAULT_MEMORY_PROFILE` — [`L74`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L74) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `DEFAULT_OWNER` — [`L73`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L73) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `altitudePreference` — [`L84`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L84) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `altitudePreference` — [`L98`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L98) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `altitudePreference` — [`L141`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L141) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `autonomy` — [`L142`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L142) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `command` — [`L133`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L133) — Omit (or pass empty) for an ideation session — no measurement loop. — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `direction` — [`L135`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L135) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `exploreFraction` — [`L83`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L83) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `exploreFraction` — [`L97`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L97) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `exploreFraction` — [`L140`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L140) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `filesInScope` — [`L136`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L136)
- `goal` — [`L131`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L131) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `maxIterations` — [`L138`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L138)
- `memoryProfile` — [`L139`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L139) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `metricName` — [`L134`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L134) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `name` — [`L130`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L130) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `owner` — [`L143`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L143) — documented in [extensions-pi-autoresearch-vkf-config.ts](../../../concepts/extensions-pi-autoresearch-vkf-config.ts.md)
- `workingDir` — [`L137`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/config.ts#L137)

