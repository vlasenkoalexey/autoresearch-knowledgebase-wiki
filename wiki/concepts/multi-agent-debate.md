---
title: "Multi-Agent Debate"
type: concept
tags: [autoresearch, llm-as-judge, self-play]
created: 2026-07-04
updated: 2026-07-04
sources: 1
---

A technique where an LLM simulates **multiple turns of argument between opposing (or comparing) positions**
— rather than a single-shot judgment — before reaching a conclusion. Used both to *generate* better ideas
(argue a hypothesis's own weaknesses into a stronger version) and to *judge* between candidates (compare two
items via simulated debate rather than a single pairwise-preference prompt), with the debate transcript
itself sometimes kept as part of the record.

## As instantiated by Co-Scientist

[Co-Scientist](../sources/ai-co-scientist.md) uses multi-agent debate in two distinct places:

1. **Generation** — the Generation agent runs *simulated scientific debates* among self-played expert
   personas as one of its hypothesis-generation strategies, refining an idea across multiple turns of
   argument before it enters the tournament (self-play/self-critique, not multi-model debate).
2. **Ranking** — the Ranking agent's Elo tournament uses **multi-turn scientific-debate matches** for
   top-ranked hypotheses specifically to reduce **positional/ordering bias** in pairwise comparison (cheaper
   single-turn comparisons are reserved for lower-ranked pairs). The paper's own ablation is the clean
   causal evidence for the mechanism: replacing a plain comparison prompt with a scientific-debate prompt in
   the Ranking agent "significantly enhance[d] ranking accuracy for high-quality hypotheses and, critically,
   reduce[d] the positional bias" — i.e., debate format, not just more tokens, is what corrects the known
   LLM-as-judge failure mode where the first- or second-shown item is systematically favored.

Debate here is explicitly not adversarial-to-a-fault: it is bounded by the tournament's Elo bookkeeping
(each match produces a single "which is better" decision that updates ratings) and by the Proximity agent
steering debates toward comparably-relevant pairs rather than debating unrelated hypotheses against each
other.

## Why this matters beyond Co-Scientist

Multi-agent debate is Co-Scientist's concrete answer to a known weakness of naive LLM-as-judge setups:
single-prompt pairwise comparisons carry measurable positional bias (favoring whichever candidate is shown
first or second). Any system in this wiki that uses an LLM (or VLM) as an evaluator/judge over generated
candidates — e.g. The AI Scientist-v2's best-first tree search, which uses an LLM judge over experiment
nodes and a VLM judge over plots — faces the same bias risk; Co-Scientist's ablation is direct evidence that
structuring the judgment as a multi-turn debate, rather than a single verdict, is one mitigation worth
checking for in any such system.

## See also

- [`../sources/ai-co-scientist.md`](../sources/ai-co-scientist.md)
- [`hypothesis-generation`](hypothesis-generation.md)
- [`../sources/ai-scientist-v2.md`](../sources/ai-scientist-v2.md) — a related LLM/VLM-as-judge design that
  does not use multi-turn debate, for contrast.
