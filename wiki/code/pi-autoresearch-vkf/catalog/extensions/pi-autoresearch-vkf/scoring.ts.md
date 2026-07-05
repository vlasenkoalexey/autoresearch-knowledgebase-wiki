---
title: 'Module: extensions/pi-autoresearch-vkf/scoring.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/scoring.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`scoring.ts`/
symbols:
  scoreIdea: scoreIdea().
  selectBalanced: selectBalanced().
  rankIdeas: rankIdeas().
  IdeaInput: IdeaInput#
  classifySlot: classifySlot().
  ScoredIdea.id: ScoredIdea#id.
  ScoredIdea.factors: ScoredIdea#factors.
  pickDiverse: pickDiverse().
  BalancedPick.r: BalancedPick#r.
  tokenize: tokenize().
  ScoredIdea.priority: ScoredIdea#priority.
  clamp: clamp.
  BalancedPick.slot: BalancedPick#slot.
  ScoredIdea: ScoredIdea#
  IdeaInput.verification_level: IdeaInput#verification_level.
  Candidate: Candidate#
  maxSimilarity: maxSimilarity().
  ScoredIdea.bucket: ScoredIdea#bucket.
  bucketKey: bucketKey().
  IdeaInput.altitude: IdeaInput#altitude.
  jaccard: jaccard().
  ScoredIdea.title: ScoredIdea#title.
  ScoredIdea.max_similarity: ScoredIdea#max_similarity.
  ScoreOptions: ScoreOptions#
  ScoreFactors.evidence_strength: ScoreFactors#evidence_strength.
  ScoreFactors.novelty: ScoreFactors#novelty.
  ScoreFactors.structural_novelty: ScoreFactors#structural_novelty.
  Slot: Slot#
  EVIDENCE_STRENGTH: EVIDENCE_STRENGTH.
  ALTITUDE_AFFINITY: ALTITUDE_AFFINITY.
  BalancedPick.idea: BalancedPick#idea.
  IdeaInput.id: IdeaInput#id.
  ScoreFactors.expected_value: ScoreFactors#expected_value.
  ScoreFactors.feasibility: ScoreFactors#feasibility.
  ScoreFactors.info_gain: ScoreFactors#info_gain.
  selectBalanced.opts-typeLiteral120.exploreFraction: selectBalanced().(opts)typeLiteral120:exploreFraction.
  selectBalanced.opts-typeLiteral120.k: selectBalanced().(opts)typeLiteral120:k.
  IdeaInput.text: IdeaInput#text.
  IdeaInput.reliability_score: IdeaInput#reliability_score.
  ScoreFactors.altitude_affinity: ScoreFactors#altitude_affinity.
  ScoreFactors.implementation_cost: ScoreFactors#implementation_cost.
  BalancedPick: BalancedPick#
  DEFAULT_PLAYBOOK: DEFAULT_PLAYBOOK.
  STOPWORDS: STOPWORDS.
  IdeaInput.title: IdeaInput#title.
  IdeaInput.belief: IdeaInput#belief.
  IdeaInput.recency_score: IdeaInput#recency_score.
  IdeaInput.expected_value: IdeaInput#expected_value.
  IdeaInput.feasibility: IdeaInput#feasibility.
  IdeaInput.info_gain: IdeaInput#info_gain.
  IdeaInput.implementation_cost: IdeaInput#implementation_cost.
  IdeaInput.lever: IdeaInput#lever.
  IdeaInput.stale: IdeaInput#stale.
  ScoreFactors: ScoreFactors#
  ScoreFactors.freshness: ScoreFactors#freshness.
  ScoreOptions.explored: ScoreOptions#explored.
  ScoreOptions.playbook: ScoreOptions#playbook.
  ScoreOptions.bucketCounts: ScoreOptions#bucketCounts.
  ScoreOptions.exploredTotal: ScoreOptions#exploredTotal.
  ScoreOptions.altitudePreference: ScoreOptions#altitudePreference.
---
# Module: [`extensions/pi-autoresearch-vkf/scoring.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts)

## Classes
### `BalancedPick`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:274`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L274) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `interface BalancedPick`
- members:
  - `idea` — [`L276`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L276) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `r` — [`L275`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L275) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `slot` — [`L277`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L277) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- uses (calls/refs, reference-scoped): [`IdeaInput`](scoring.ts.md#IdeaInput), [`ScoredIdea`](scoring.ts.md#ScoredIdea), [`Slot`](scoring.ts.md#Slot)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`selectExpansion`](tree.ts.md#selectExpansion), [`selectBalanced`](scoring.ts.md#selectBalanced), [`pickDiverse`](scoring.ts.md#pickDiverse), [`Candidate`](scoring.ts.md#Candidate)

### `Candidate`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:280`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L280) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `interface Candidate`
- uses (calls/refs, reference-scoped): [`BalancedPick`](scoring.ts.md#BalancedPick)
- used by: [`selectBalanced`](scoring.ts.md#selectBalanced), [`pickDiverse`](scoring.ts.md#pickDiverse)

### `IdeaInput`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:99`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L99) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `interface IdeaInput`
- members:
  - `altitude` — [`L116`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L116) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `belief` — [`L105`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L105) — Numeric belief in [0,1] that this helps the goal. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `expected_value` — [`L110`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L110) — Optional explicit overrides for the priority factors. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `feasibility` — [`L111`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L111) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `id` — [`L100`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L100) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `implementation_cost` — [`L113`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L113) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `info_gain` — [`L112`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L112) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `lever` — [`L115`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L115) — Coverage tags (see ./cards.ts) — drive structural novelty + altitude bias. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `recency_score` — [`L107`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L107) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `reliability_score` — [`L108`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L108) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `stale` — [`L118`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L118) — Flagged stale (valid_until passed, or `vkf freshness` flagged it). Penalized.
  - `text` — [`L103`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L103) — Concatenated descriptive text (title + mechanism + context + body). — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `title` — [`L101`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L101)
  - `verification_level` — [`L106`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L106) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- uses (calls/refs, reference-scoped): [`Verification`](cards.ts.md#Verification), [`Altitude`](cards.ts.md#Altitude)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`scoreIdea`](scoring.ts.md#scoreIdea), [`selectExpansion`](tree.ts.md#selectExpansion), [`selectBalanced`](scoring.ts.md#selectBalanced), [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`rankIdeas`](scoring.ts.md#rankIdeas), [`classifySlot`](scoring.ts.md#classifySlot), [`idea`](scoring.ts.md#BalancedPick.idea), [`idea`](tree.ts.md#ExpansionPick.idea)  (2 test-only)

### `ScoreFactors`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:121`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L121)
- signature: `interface ScoreFactors`
- members:
  - `altitude_affinity` — [`L129`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L129) — Goal-gated bias for the idea's altitude (1 = neutral). — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `evidence_strength` — [`L124`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L124) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `expected_value` — [`L122`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L122) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `feasibility` — [`L123`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L123) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `freshness` — [`L133`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L133) — Freshness multiplier: 1 when current, <1 when flagged stale.
  - `implementation_cost` — [`L131`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L131) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `info_gain` — [`L130`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L130) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `novelty` — [`L125`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L125) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `structural_novelty` — [`L127`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L127) — How under-explored this idea's lever·altitude bucket is, [0,1]. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`scoreIdea`](scoring.ts.md#scoreIdea), [`classifySlot`](scoring.ts.md#classifySlot), [`factors`](scoring.ts.md#ScoredIdea.factors)

### `ScoreOptions`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:163`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L163) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `interface ScoreOptions`
- members:
  - `altitudePreference` — [`L173`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L173) — Altitude bias mode. Default "any" (neutral).
  - `bucketCounts` — [`L169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L169) — Count of already-run experiments per `lever|altitude` bucket.
  - `explored` — [`L165`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L165) — Texts of ideas already explored (tried experiments, settled claims).
  - `exploredTotal` — [`L171`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L171) — Total already-run experiments (denominator for bucket saturation).
  - `playbook` — [`L167`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L167) — Standard-playbook phrases to penalize. Defaults to DEFAULT_PLAYBOOK.
- uses (calls/refs, reference-scoped): [`AltitudePreference`](config.ts.md#AltitudePreference)
- used by: [`scoreIdea`](scoring.ts.md#scoreIdea), [`rankIdeas`](scoring.ts.md#rankIdeas)

### `ScoredIdea`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:136`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L136) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `interface ScoredIdea`
- members:
  - `bucket` — [`L144`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L144) — The `lever|altitude` bucket this idea falls in. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `factors` — [`L140`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L140) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `id` — [`L137`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L137) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `max_similarity` — [`L142`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L142) — Max similarity to already-explored / playbook text (drives novelty). — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `priority` — [`L139`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L139) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
  - `title` — [`L138`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L138) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- uses (calls/refs, reference-scoped): [`ScoreFactors`](scoring.ts.md#ScoreFactors)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`scoreIdea`](scoring.ts.md#scoreIdea), [`selectExpansion`](tree.ts.md#selectExpansion), [`selectBalanced`](scoring.ts.md#selectBalanced), [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`rankIdeas`](scoring.ts.md#rankIdeas), [`classifySlot`](scoring.ts.md#classifySlot), [`pickDiverse`](scoring.ts.md#pickDiverse), [`r`](scoring.ts.md#BalancedPick.r), [`r`](tree.ts.md#ExpansionPick.r)  (1 test-only)

### `Slot`
- def: [`extensions/pi-autoresearch-vkf/scoring.ts:260`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L260) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- signature: `type Slot`
- used by: [`tree.ts`](tree.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-tree.ts), [`classifySlot`](scoring.ts.md#classifySlot), [`slot`](scoring.ts.md#BalancedPick.slot), [`ExpansionPick`](tree.ts.md#ExpansionPick)

## Functions
- `bucketKey(lever?: string | undefined, altitude?: string | undefined)` — [`L159`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L159) — documented in [extensions-pi-autoresearch-vkf-progress_data.ts](../../../concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md)
- `classifySlot(r: ScoredIdea, idea: IdeaInput)` — [`L269`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L269) — An idea is an *explore* bet if it's high-altitude (mechanism/reframe) or it — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `jaccard(a: Set<string>, b: Set<string>)` — [`L78`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L78) — Jaccard similarity of two token sets, in [0,1]. Empty/empty = 0. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `maxSimilarity(text: string, corpus: readonly string[])` — [`L87`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L87) — Largest Jaccard similarity of `text` against any string in `corpus`. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `pickDiverse(pool: Candidate[], n: number, usedBuckets: Set<string>, chosen: Set<string>)` — [`L283`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L283) — Take up to `n` from `pool`, preferring unseen buckets, then filling the rest. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `rankIdeas(ideas: readonly IdeaInput[], opts?: ScoreOptions)` — [`L254`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L254) — Score and rank ideas, highest priority first. — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `scoreIdea(idea: IdeaInput, opts?: ScoreOptions)` — [`L185`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L185) — Score one idea, returning its priority and the factor breakdown. — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `selectBalanced(scored: readonly { r: ScoredIdea; idea: IdeaInput; }[], opts: { exploreFraction: number; k: number; })` — [`L310`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L310) — Pick the next `k` experiments, reserving ⌈exploreFraction·k⌉ slots for explore — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `tokenize(text: string)` — [`L69`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L69) — Lowercase word-token set, dropping short tokens and stopwords. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)

## Module values
- `ALTITUDE_AFFINITY` — [`L153`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L153) — Altitude bias per preference mode; missing altitude is treated as neutral. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `DEFAULT_PLAYBOOK` — [`L39`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L39) — The "standard playbook" — obvious moves an autoresearch loop rediscovers on — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `EVIDENCE_STRENGTH` — [`L26`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L26) — Evidence strength implied by a card's verification level, in [0,1]. — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `STOPWORDS` — [`L60`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L60)
- `clamp` — [`L97`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L97) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `exploreFraction` — [`L312`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L312) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)
- `k` — [`L312`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/scoring.ts#L312) — documented in [extensions-pi-autoresearch-vkf-scoring.ts](../../../concepts/extensions-pi-autoresearch-vkf-scoring.ts.md)

