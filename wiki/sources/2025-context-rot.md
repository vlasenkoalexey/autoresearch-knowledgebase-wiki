# Context Rot: How Increasing Input Tokens Impacts LLM Performance

Chroma's controlled study (Kelly Hong, Anton Troynikov, Jeff Huber; published 2025-07-14) isolating **input
length** as the sole variable and measuring accuracy across 18 frontier models (GPT-4.1, Claude 4 family,
Gemini 2.5, Qwen3, and others). Its finding — performance degrades well before a context window fills, and
non-uniformly — is the empirical premise behind the recursive-language-model line of work this wiki ingests
alongside it (see [Connections](#connections)). Ingested 2026-08-12 as background for
[Recursive Language Models](recursive-language-models.md) and
[Prime Agent](prime-agent-launch.md), which cite it as their starting problem.

## Overview

Prior long-context evaluation leaned on Needle-in-a-Haystack (NIAH): drop a known sentence into an
unrelated document and ask the model to retrieve it verbatim. Chroma's contribution is to hold task
*difficulty* constant while varying only input *length*, across four experiment families — NIAH variants,
semantic (non-lexical) retrieval, LongMemEval (conversational QA over up to 113k-token chat histories), and
a Repeated-Words exact-replication task — at 8 input lengths from 25 to 10,000+ words, 11 needle positions
each.

## Key claims

- **Degradation starts long before the window is full.** Accuracy declines as input grows even on tasks
  simple enough that length alone shouldn't matter — the paper's framing is that this is a property of how
  models allocate attention across a longer input, not a capacity limit being reached.
- **Degradation is non-uniform, and semantic similarity is the lever.** Lower similarity between a question
  and the sentence that answers it makes accuracy fall faster as length grows; the effect is much smaller
  when question and answer share vocabulary. So two needles at the same position and the same document
  length can degrade at different rates depending on how directly they're phrased.
- **Distractors compound the effect, unevenly.** Adding one topically-related distractor lowers accuracy
  below a needle-only baseline; four distractors compound further, and some individual distractors hurt
  far more than others of similar surface plausibility.
- **Coherent context can be worse than incoherent context.** Counterintuitively, all 18 models did better
  on a shuffled (logically incoherent) haystack than on one that read as a coherent document — the opposite
  of what a purely capacity-based account would predict.
- **Position and behavior effects compound the accuracy numbers.** On the Repeated-Words task, models
  increasingly *under-generate* (stop early rather than reproduce the full text) past roughly 2,500 words,
  and refusal/hallucination rates rise with length and vary by model family (Claude models showed the
  lowest hallucination rates in the study; GPT models the highest).
- **The stated conclusion is architectural, not a tuning fix**: reliability depends on *how* relevant
  information is presented — placement, distractor load, structural coherence — not merely on *whether* it
  is present in the window. The paper frames "context engineering" (deliberate management of what enters
  the window) as the response, rather than assuming a longer window is strictly better.

## Key data points

| Signal | Finding |
|---|---|
| Models tested | 18 frontier models (GPT-4.1, Claude 4 family, Gemini 2.5, Qwen3, others) |
| Input range | 25 to 10,000+ words, 8 lengths, 11 needle positions per configuration |
| Semantic similarity range tested | 0.445–0.829 (question-answer similarity score) |
| Repeated-Words breakdown point | errors increase sharply past ~2,500 words |
| Refusal rates at that point | GPT-4.1 ≈ 2.55%; Claude Opus 4 ≈ 2.89% |
| Haystack structure effect | shuffled (incoherent) haystacks outperformed logically structured ones, across all 18 models |
| LongMemEval | accuracy on a focused ~300-token prompt is substantially higher than on the full 113k-token history for every model tested |

## Techniques referenced
Needle-in-a-Haystack retrieval; LongMemEval conversational QA; controlled distractor injection; haystack
coherence manipulation (shuffled vs. structured); exact-replication (Repeated-Words) probing for
under-generation and hallucination as length grows.

## Gaps & caveats
- This is a **measurement** paper, not a fix — it explicitly declines to explain the underlying attention
  mechanism producing the decay, only that it's real and non-uniform. Systems built in response to it (RLM,
  Prime Agent) are downstream inferences about what the right fix is, not something this paper validates.
- All results are on *retrieval and light-synthesis* tasks. The paper itself flags that real applications
  requiring multi-step reasoning or synthesis over long context should be expected to degrade *more*, not
  less — that extrapolation is stated, not measured here.
- No comparison to a context-avoidance architecture (RLM-style) is in scope; this paper only characterizes
  the problem the later systems respond to.

## Connections
- [Recursive Language Models](recursive-language-models.md) — cites this study's core finding (accuracy
  degrades well before the window fills) as the reason to keep long input out of the model's context
  entirely rather than try to manage it in-window.
- [Prime Agent launch post](prime-agent-launch.md) — the product built around RLM + Continual Harness,
  positioned as the shipped answer to the problem this paper measures.
- [Wiki-driven autoresearch loop](../topics/wiki-driven-autoresearch-loop.md) — this wiki's own
  skills-vs-sub-agents context-pollution discussion (from the TPU autoresearch wiki's blog series)
  independently arrives at "isolate work that would burn context the caller doesn't need to see," which is
  the same design response one level up the stack (session context rather than a single model call).

## Sources
- [Context Rot: How Increasing Input Tokens Impacts LLM Performance](https://www.trychroma.com/research/context-rot),
  Kelly Hong, Anton Troynikov, Jeff Huber — Chroma, 2025-07-14
