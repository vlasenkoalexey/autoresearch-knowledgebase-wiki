---
title: 'Module: extensions/pi-autoresearch-vkf/synthesis.ts'
type: catalog
provenance: extracted
module: extensions/pi-autoresearch-vkf/synthesis.ts
status: fresh
symbol_base: scip-typescript npm pi-autoresearch-vkf 0.12.0 extensions/pi-autoresearch-vkf/`synthesis.ts`/
symbols:
  findCompositions: findCompositions().
  findContradictions: findContradictions().
  findTransfers: findTransfers().
  CardLike.id: CardLike#id.
  CardLike: CardLike#
  CardLike.memory_state: CardLike#memory_state.
  contextSimilarity: contextSimilarity().
  topicSimilarity: topicSimilarity().
  mechanismSimilarity: mechanismSimilarity().
  mechTokens: mechTokens.
  ctxTokens: ctxTokens.
  CardLike.title: CardLike#title.
  Tension.kind: Tension#kind.
  CardLike.text: CardLike#text.
  CardLike.lever: CardLike#lever.
  CardLike.mechanism: CardLike#mechanism.
  CardLike.context: CardLike#context.
  Tension.a: Tension#a.
  Tension.b: Tension#b.
  Tension.detail: Tension#detail.
  Tension.question: Tension#question.
  Tension.strength: Tension#strength.
  Composition.score: Composition#score.
  WORKED: WORKED.
  Transfer.transfer_score: Transfer#transfer_score.
  Composition.a: Composition#a.
  Composition.b: Composition#b.
  COMPOSABLE: COMPOSABLE.
  Transfer.from: Transfer#from.
  Composition.titleA: Composition#titleA.
  Composition.titleB: Composition#titleB.
  CardLike.conflicts_with: CardLike#conflicts_with.
  Tension: Tension#
  Transfer: Transfer#
  Transfer.title: Transfer#title.
  Transfer.mechanism_similarity: Transfer#mechanism_similarity.
  Transfer.context_similarity: Transfer#context_similarity.
  Composition: Composition#
  Composition.goal_relevance: Composition#goal_relevance.
  Composition.mechanism_overlap: Composition#mechanism_overlap.
  TensionKind: TensionKind#
  ContradictionOptions: ContradictionOptions#
  ContradictionOptions.topicThreshold: ContradictionOptions#topicThreshold.
  ContradictionOptions.contextThreshold: ContradictionOptions#contextThreshold.
  ContradictionOptions.mechanismThreshold: ContradictionOptions#mechanismThreshold.
  Transfer.suggestion: Transfer#suggestion.
  findTransfers.opts-typeLiteral88.minMechanismSimilarity: findTransfers().(opts)typeLiteral88:minMechanismSimilarity.
  findTransfers.opts-typeLiteral88.maxContextSimilarity: findTransfers().(opts)typeLiteral88:maxContextSimilarity.
  Composition.suggestion: Composition#suggestion.
  CompositionOptions: CompositionOptions#
  CompositionOptions.minGoalRelevance: CompositionOptions#minGoalRelevance.
  CompositionOptions.maxMechanismOverlap: CompositionOptions#maxMechanismOverlap.
---
# Module: [`extensions/pi-autoresearch-vkf/synthesis.ts`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts)

## Classes
### `CardLike`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:28`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L28) — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- doc: Minimal shape the synthesis functions need from a memory card.
- signature: `interface CardLike`
- members:
  - `conflicts_with` — [`L38`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L38) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `context` — [`L34`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L34) — The context/goal — *where* it applies. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `id` — [`L29`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L29) — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
  - `lever` — [`L40`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L40) — System part the claim touches (see ./cards.ts LEVERS) — different levers compose better. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `mechanism` — [`L32`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L32) — The mechanism — *how/why* it works. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `memory_state` — [`L37`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L37) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `text` — [`L36`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L36) — Full descriptive text (title + assertion/body) for topic similarity. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `title` — [`L30`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L30) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- uses (calls/refs, reference-scoped): [`MemoryState`](cards.ts.md#MemoryState)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`index.ts`](index.ts.md#scip-typescript-npm-pi-autoresearch-vkf-0.12.0-extensions-pi-autoresearch-vkf-index.ts), [`findCompositions`](synthesis.ts.md#findCompositions), [`findContradictions`](synthesis.ts.md#findContradictions), [`findTransfers`](synthesis.ts.md#findTransfers), [`toCardLike`](index.ts.md#toCardLike), [`contextSimilarity`](synthesis.ts.md#contextSimilarity), [`topicSimilarity`](synthesis.ts.md#topicSimilarity), [`mechanismSimilarity`](synthesis.ts.md#mechanismSimilarity), [`ctxTokens`](synthesis.ts.md#ctxTokens), [`mechTokens`](synthesis.ts.md#mechTokens)  (2 test-only)

### `Composition`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:221`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L221) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- signature: `interface Composition`
- members:
  - `a` — [`L223`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L223) — The two parent claims to combine. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `b` — [`L224`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L224) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `goal_relevance` — [`L228`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L228) — How relevant the *weaker* parent is to the goal, [0,1]. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `mechanism_overlap` — [`L230`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L230) — Mechanism overlap between the parents — low means complementary. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `score` — [`L232`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L232) — Ranking score: relevance × complementarity × evidence. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `suggestion` — [`L233`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L233) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `titleA` — [`L225`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L225) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `titleB` — [`L226`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L226) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`findCompositions`](synthesis.ts.md#findCompositions)

### `CompositionOptions`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:236`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L236) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- signature: `interface CompositionOptions`
- members:
  - `maxMechanismOverlap` — [`L240`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L240) — Max mechanism overlap — above this the pair is redundant, not composable. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `minGoalRelevance` — [`L238`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L238) — Min per-parent goal relevance (topic similarity to the goal text). — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- used by: [`findCompositions`](synthesis.ts.md#findCompositions)

### `ContradictionOptions`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:75`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L75) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- signature: `interface ContradictionOptions`
- members:
  - `contextThreshold` — [`L79`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L79) — Min context similarity for "same goal". — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `mechanismThreshold` — [`L81`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L81) — Max mechanism similarity for "different mechanism". — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `topicThreshold` — [`L77`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L77) — Min topic similarity to consider two claims "about the same thing". — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- used by: [`findContradictions`](synthesis.ts.md#findContradictions)

### `Tension`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:63`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L63) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- signature: `interface Tension`
- members:
  - `a` — [`L65`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L65) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `b` — [`L66`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L66) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `detail` — [`L68`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L68) — Human-readable description of the tension. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `kind` — [`L64`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L64) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `question` — [`L70`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L70) — A generative question this tension poses — the seed for a new hypothesis. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `strength` — [`L72`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L72) — Strength of the signal, [0,1], for ranking. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- uses (calls/refs, reference-scoped): [`TensionKind`](synthesis.ts.md#TensionKind)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`findContradictions`](synthesis.ts.md#findContradictions)  (1 test-only)

### `TensionKind`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:61`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L61)
- signature: `type TensionKind`
- used by: [`kind`](synthesis.ts.md#Tension.kind)

### `Transfer`
- def: [`extensions/pi-autoresearch-vkf/synthesis.ts:169`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L169) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- signature: `interface Transfer`
- members:
  - `context_similarity` — [`L174`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L174) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `from` — [`L171`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L171) — The source card whose mechanism might transfer. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `mechanism_similarity` — [`L173`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L173) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `suggestion` — [`L177`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L177) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `title` — [`L172`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L172) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
  - `transfer_score` — [`L176`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L176) — mechanism_similarity × (1 − context_similarity): high = strong analogy. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- used by: [`autoresearchExtension`](index.ts.md#autoresearchExtension), [`findTransfers`](synthesis.ts.md#findTransfers)

## Functions
- `contextSimilarity(a: CardLike, b: CardLike)` — [`L55`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L55) — How similar two cards' contexts/goals are. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `findCompositions(goal: string, cards: readonly CardLike[], opts?: CompositionOptions)` — [`L250`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L250) — Find pairs of *trusted* claims worth composing into a single novel hypothesis: — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `findContradictions(cards: readonly CardLike[], opts?: ContradictionOptions)` — [`L88`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L88) — Find tensions among a set of claim cards. Returns one {@link Tension} per — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `findTransfers(target: CardLike, cards: readonly CardLike[], opts?: { minMechanismSimilarity?: number | undefined; maxContextSimilarity?: number | undefined; })` — [`L187`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L187) — Find cross-domain transfer candidates for a target problem: cards whose — documented in [extensions-pi-autoresearch-vkf-index.ts](../../../concepts/extensions-pi-autoresearch-vkf-index.ts.md)
- `mechanismSimilarity(a: CardLike, b: CardLike)` — [`L51`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L51) — How similar two cards' mechanisms are. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `topicSimilarity(a: CardLike, b: CardLike)` — [`L47`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L47) — Topic similarity from full text. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)

## Module values
- `COMPOSABLE` — [`L219`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L219) — States trusted enough to be a composition parent. — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `WORKED` — [`L59`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L59) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `ctxTokens` — [`L44`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L44) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `maxContextSimilarity` — [`L190`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L190) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `mechTokens` — [`L43`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L43) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)
- `minMechanismSimilarity` — [`L190`](../../../../../../raw/code/pi-autoresearch-vkf/extensions/pi-autoresearch-vkf/synthesis.ts#L190) — documented in [extensions-pi-autoresearch-vkf-synthesis.ts](../../../concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)

