---
title: "Accelerating scientific discovery with Co-Scientist (né \"Towards an AI co-scientist\")"
type: source
authors: Juraj Gottweis, Wei-Hung Weng, Alexander Daryin, Tao Tu, et al. (51 authors; Google Cloud AI Research, Google DeepMind, Google Research, Stanford University School of Medicine, Houston Methodist, Sequome, Fleming Initiative / Imperial College London)
arxiv: 2502.18864
venue: "arXiv preprint, v1 26 Feb 2025 as \"Towards an AI co-scientist\"; v2 29 Jun 2026, retitled \"Accelerating scientific discovery with Co-Scientist\""
source: ../../raw/papers/ai-co-scientist.pdf
updated: 2026-07-04
---
# Co-Scientist — summary

## What it is
Co-Scientist is a multi-agent AI system built on Google's Gemini models that acts as a "structured
scientific thinking engine": given a research goal in natural language, it searches and reasons over
literature and proposes **novel, testable research hypotheses and experimental protocols** for a scientist
to evaluate ([raw/papers/ai-co-scientist.pdf](../../raw/papers/ai-co-scientist.pdf), p.2 Summary, p.5). It
is explicitly framed as going beyond literature summarization or "deep research" retrieval tools — the
target output is not a synthesis of what's known but a hypothesis about what might be true and not yet
demonstrated (p.5, p.29). The system is validated on three biomedical problems of increasing complexity —
drug repurposing for acute myeloid leukemia (AML), novel epigenetic-target discovery for liver fibrosis, and
explaining a bacterial gene-transfer mechanism in antimicrobial resistance (AMR) — with wet-lab confirmation
of some of its top-ranked hypotheses (p.2, Table 1 p.5–6).

> [!inferred]
> **A version note worth recording explicitly.** The paper downloaded for this summary (arXiv:2502.18864,
> fetched July 2026) is titled *"Accelerating scientific discovery with Co-Scientist,"* which per arXiv's
> version history is the **v2 revision** (last revised 29 June 2026) of a paper originally posted 26
> February 2025 under the title *"Towards an AI co-scientist."* The v2 text itself reflects the later date —
> it references "the most recent Gemini 3 models" and frames model-agnosticism against "Gemini 3, GPT 5.4
> and Opus 4.6" (p.24, p.30) — models that postdate the original 2025 preprint. The core system,
> architecture, and biomedical validations described below appear unchanged from the original report; the
> retitling and forward-looking model references are the visible delta. Readers citing this work by its
> original name should be aware the canonical arXiv id now serves the retitled v2.

## The multi-agent architecture
At the core is an **asynchronous, continuous task-execution framework**: a **Supervisor agent** parses the
natural-language research goal into a research-plan configuration (desired attributes, evaluation criteria,
constraints), then creates a task queue and allocates specialized **worker agents** to it, periodically
computing summary statistics to decide how to keep allocating compute (p.29–30). Six specialized agents,
each with its own library of prompts and access to tools (web search, domain databases, specialized AI
models like AlphaFold), do the actual scientific reasoning (p.29–30, p.32–37):

- **Generation agent** — starts the process: explores literature via web search, runs simulated multi-turn
  scientific debates between simulated experts (self-play/self-critique) to sharpen an initial idea,
  iteratively identifies testable sub-assumptions, and does "research expansion" by reading the
  Meta-review agent's prior research overview to find unexplored parts of the hypothesis space (p.32).
- **Reflection agent** — plays the peer-reviewer role, with several distinct review modes: an *initial
  review* (no tools, fast filter for obviously flawed/non-novel ideas), a *full review* (web search-grounded
  correctness/quality/novelty check), a *deep verification review* (recursively decomposes a hypothesis into
  assumptions and sub-assumptions and independently checks each for validity), an *observation review*
  (checks whether the hypothesis better explains existing, possibly under-explained experimental
  observations than current theory does), and a *simulation review* (has the model step through the
  proposed mechanism or experiment as a simulation to surface failure modes, on the premise that a frontier
  LLM may have an implicit "world model" of scientific phenomena) (p.33–34).
- **Ranking agent** — orchestrates an **Elo-based tournament** (initial rating 1200) over all live
  hypotheses: top-ranked hypotheses face off in **multi-turn scientific-debate matches** (to reduce
  positional/ordering bias), lower-ranked ones get cheaper **single-turn pairwise comparisons**; match
  scheduling is prioritized toward similar hypotheses (via the Proximity agent's graph) and toward newer,
  currently-top-ranked hypotheses, so strong ideas quickly climb and shape which comparisons happen next
  (p.34–35).
- **Proximity agent** — asynchronously builds a similarity/proximity graph over all hypotheses relative to
  the research goal, used to cluster and de-duplicate ideas and to help the Ranking agent schedule matches
  between similar hypotheses rather than at random (p.35).
- **Evolution agent** — continually generates *new* hypotheses derived from top-ranked ones via several
  strategies: grounding-driven improvement (find weaknesses, search, revise), coherence/feasibility repair,
  drawing inspiration from one or more top hypotheses, directly combining the best aspects of several
  top hypotheses, simplification for easier testing, and deliberate "out-of-the-box" divergence away from
  the current leaders. Critically, **it never edits or replaces an existing hypothesis in place** — every
  evolved idea is a new candidate that must re-earn its rank by competing in the tournament, which the
  paper frames as protection against a flawed "improvement" silently corrupting a good hypothesis (p.35).
- **Meta-review agent** — closes the loop: it reads across all reviews and tournament debates to synthesize
  a meta-review critique of recurring failure patterns, which is **appended to other agents' prompts in the
  next iteration** — i.e. the whole system's "learning" is in-context feedback propagation, explicitly
  **not** gradient-based fine-tuning or RL (p.30, p.36). At the end of a run it also synthesizes the
  top-ranked hypotheses into a **research overview** (a roadmap of promising directions, each with
  illustrative sub-topics and suggested experiments — optionally formatted to match a grant template like
  an NIH Specific Aims page) and can suggest qualified domain experts to consult, drawn from the literature
  it reviewed (p.36).

Because the Meta-review agent's feedback is just appended to prompts rather than used to update weights, the
paper's own framing is that Co-Scientist's "self-improvement" over a run is an emergent property of the
feedback loop between these agents plus a persistent **context memory** for long-horizon state — not an
explicit trained or symbolic world model (p.29–30, p.5 Discussion).

## Test-time compute scaling via the tournament
Rather than argue for scaling test-time compute in the abstract, the paper measures it directly: across 203
distinct research goals run through February 3, 2025, hypotheses were bucketed into ten sequential deciles
of generation time, and both the **average Elo of the top-10 hypotheses** and the **single best Elo**
climbed monotonically as more compute/time was spent, with **no observed saturation** (p.7–8, Fig. 2a). On a
harder, expert-curated subset of 15 goals, Co-Scientist was entered into a tournament alongside outputs from
Gemini 2.0 Pro/Flash-Thinking, OpenAI o1, o3-mini-high, DeepSeek R1, and each expert's own "best guess"
solution, evaluated by Co-Scientist's own Elo metric; Co-Scientist eventually surpassed all of them, though
o3-mini-high and DeepSeek R1 were competitive at a fraction of the compute (p.8, Fig. 2b). It also
progressively **improved on the experts' own best-guess solutions** over the course of a run, per Elo — a
preliminary result the paper is careful to flag as needing further validation (p.8, Extended Data Fig. 1).

## Ablations: what each agent actually buys
Quantitative ablations (p.37–38, and Supplementary Notes 2–3 which this summary does not have direct access
to) attribute concrete gains to each component: the Reflection agent's novelty judgment is unreliable
without web search — it scored known non-novel ideas 6.14/10 for novelty without search vs. a correct
2.38/10 with search, and search also lifted correctness auto-eval from 7.4 to 8.46/10 and GPQA AUC from
0.643 to 0.651 (p.38); scientific-debate-style ranking prompts (vs. plain pairwise comparison) improved
ranking accuracy and reduced positional bias (p.38); the Evolution agent's iterative refinement raised GPQA
precision from 70.9% to 75.4% and average hypothesis-quality score from 4.7 to 5.6 (p.38); the Proximity
agent's similarity scores correlated with actual quality differences between hypotheses (p.38); and the
Meta-review agent raised AUC for predicting a correct solution from 0.521 to 0.597 on the authors'
constructed dataset and 0.629 to 0.634 on GPQA-diamond (p.38).

## Human-expert evaluation
On 11 of the 15 curated goals, blinded domain experts rated Co-Scientist, Gemini 2.0 Flash-Thinking, Gemini
2.0 Pro Experimental, and OpenAI o1 outputs for novelty, impact (both 5-point Likert), and overall
preference. Co-Scientist was the most preferred system and scored highest on both novelty (3.64/5) and
impact (3.09/5); a separate LLM-as-judge evaluation (four different judge models) also ranked Co-Scientist
first across all four judges, though the paper flags the small sample size as limiting how much weight
these numbers can bear (p.9–10, Fig. 2c, Extended Data Fig. 2).

## Real-world biomedical validations — and how much human labor they still take
All three validations were run with an expert scientist in the loop end to end, and the paper is explicit
about quantifying that human time: for the AML study, the initial goal-definition prompt took under an hour
of a clinician's time, and reviewing/selecting the system's ranked candidates for wet-lab testing took
roughly three hours (p.36).

- **AML drug repurposing** (p.11–17): constrained to search over 2,300 approved drugs across 34 cancer
  types, with an oncologist review of the resulting predictions. In vitro testing of five expert-selected
  candidates showed three (Binimetinib, Pacritinib, Cerivastatin) inhibited AML cell viability, with
  Binimetinib reaching an IC50 as low as 2 nM in several AML lines (p.12–13, Fig. 3a–c). Separately, run
  *without* expert guidance or external data like DepMap scores, the system nominated a fully novel
  candidate, **KIRA6** (an IRE1α inhibitor), which showed an 18-fold selectivity window between the KG-1a
  AML line (IC50 10 nM) and a non-AML control line (IC50 180 nM) (p.14–15, Fig. 3d–h). The system also
  proposed seven multi-drug combinations, several validated as synergistic by the Chou-Talalay /
  Highest-Single-Agent / Bliss-independence methods across two AML lines (p.16–18, Fig. 4). A further
  structured "translational analysis" task correctly identified a specific clinical niche for Binimetinib —
  frail, heavily pretreated patients — by reasoning that its UGT1A1 metabolic pathway avoids the CYP3A4
  drug-drug interactions that limit competing targeted therapies (p.18–19).
- **Liver fibrosis target discovery** (p.19): tasked with proposing epigenetic-modifier targets and drugs
  against them, using human hepatic organoids with live-cell imaging as the validation assay; three
  top-ranked modifiers were tested and two showed significant anti-fibrotic activity without toxicity,
  including **Vorinostat**, already FDA-approved for a cancer indication — an example of the system making
  a cross-disease connection (cancer drug → liver fibrosis) (p.19, citing Guan et al. 2025 as the companion
  validation paper).
- **Antimicrobial resistance mechanism** (p.19–20): given only minimal background, the system was asked to
  explain why capsid-forming phage-inducible chromosomal islands (cf-PICIs) can transfer across diverse
  bacterial species. It independently proposed, as its top-ranked hypothesis, that cf-PICIs interact with
  diverse **phage tails** to expand host range — matching, within two days of compute, the finding of an
  independent, co-timed wet-lab discovery from the same research group that had not yet been published
  (p.19–20, citing Penadés et al. 2025 in *Cell*).

## Where Co-Scientist stops: hypothesis generation, not autonomous experimentation
The paper is explicit that **Co-Scientist itself never executes a physical experiment** — it proposes and
ranks hypotheses and experimental protocols; every wet-lab step (cell-line selection, dosing, running the
assay, reading it out) in all three validations was performed by human domain experts, with the system's
role ending at a ranked candidate list and a synthesized research overview (p.11, p.36 "Expert-in-the-loop"
workflow). The Discussion names this as a current boundary rather than an oversight: *"In the fullness of
time, integrating Co-Scientist with laboratory automation platforms could create a closed-loop, autonomous
system for hypothesis generation, experimental validation, and iterative learning"* (p.25) — phrased as
future work, i.e. **not yet implemented**. The system's own "self-improvement" loop (Generation → Reflection
→ Ranking/tournament → Evolution → Meta-review) operates entirely over text: hypotheses, reviews, debate
transcripts, and Elo scores, not over any executed code or lab result the system itself produced. Where
literature-grounding happens, it is via web search and a scientist-supplied document repository, not by
running an experiment to generate new data (p.30, p.37 "Tool use").

The Discussion also flags concrete limitations consistent with that boundary: Co-Scientist's knowledge is
capped by open-access literature (missing paywalled prior art and, structurally, negative results that
rarely get published), so a hypothesis can propagate an erroneous or irreproducible claim from its source
material; the system inherits its base LLM's factuality and hallucination limitations; and validation of its
hypotheses so far is still described by the authors as "preliminary" (p.24–25).

## Contrast with the closed-loop end-to-end systems
This is the sharpest architectural contrast in the wiki's autoresearch topic: Co-Scientist and
[The AI Scientist-v2](ai-scientist-v2.md) both scale test-time compute through an iterative,
multi-candidate search loop with an LLM (and, for AI Scientist-v2, VLM) acting as judge, but they differ on
**who closes the loop that produces new evidence**. The AI Scientist-v2 runs its own experiments — an LLM
writes and executes Python, gets back real metrics and plots from that code, and a VLM critiques the
resulting figures, all inside the system's own agentic tree search, with no human step between hypothesis
and result (see [`ai-scientist-v2.md`](ai-scientist-v2.md), §"The core method"). Co-Scientist's tournament
never touches an execution environment at all: what gets ranked and evolved is prose (a hypothesis plus its
reasoning and reviews), and what turns a top-ranked hypothesis into evidence is a human scientist running a
wet-lab assay outside the system, on their own timescale (hours to days), reporting back only informally to
inform the next research goal. That difference tracks the domains: AI Scientist-v2's ML experiments are
themselves code that a computer can run, so the loop *can* close inside the agent; Co-Scientist's target
experiments are physical biology (cell viability assays, organoid imaging) that current agentic systems
cannot execute, so the loop necessarily opens onto a human — a structural rather than a design limitation of
the current system, and exactly the gap the Discussion's "laboratory automation platforms" aside gestures at
closing next (p.25).

> [!inferred]
> Framing this as "the key contrast on who closes the experiment loop" is this wiki's synthesis for
> organizing the autoresearch topic page, not a comparison the Co-Scientist paper itself draws — Co-Scientist
> never mentions The AI Scientist or Sakana AI.

## Where this fits in the wiki
See [`../topics/autoresearch.md`](../topics/autoresearch.md) for how this compares to other AI-scientist and
autoresearch systems, and the concept pages [`hypothesis-generation`](../concepts/hypothesis-generation.md)
and [`multi-agent-debate`](../concepts/multi-agent-debate.md) for the two mechanisms this paper contributes.
Raw source: [`raw/papers/ai-co-scientist.pdf`](../../raw/papers/ai-co-scientist.pdf).
