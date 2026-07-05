# AI for Auto-Research: Roadmap & User Guide

**Source:** Kong, Sun, Chow, et al. (Awesome AI Auto-Research Team), "AI for Auto-Research: Roadmap & User
Guide," arXiv:2605.18661 (18 May 2026). Project page:
[worldbench.github.io/awesome-ai-auto-research](https://worldbench.github.io/awesome-ai-auto-research);
GitHub: [worldbench/awesome-ai-auto-research](https://github.com/worldbench/awesome-ai-auto-research).
Raw source: [`../../raw/papers/ai-for-auto-research-roadmap.pdf`](../../raw/papers/ai-for-auto-research-roadmap.pdf).

## What this paper is

This is not a paper reporting a new system or a new result — it is a **field map**. It surveys AI-assisted
research end-to-end, covering developments through April 2026, and its central contribution is a **taxonomy**:
four "epistemological phases" containing eight stages, which the paper uses to organize hundreds of systems,
benchmarks, and empirical findings (a 65-page reference list and a ~250-row tool inventory in the appendix).
Because this wiki's scope is exactly "autoresearch" (AI-scientist systems, hypothesis generation,
self-improving research loops) and "auto-optimization" (AutoML, NAS, learned optimizers, kernel/schedule
auto-tuning) — this paper is the scaffold that should shape how `wiki/topics/autoresearch.md` is organized,
and other ingested papers should be understood as filling in specific cells of its taxonomy.

## The lifecycle taxonomy — four phases, eight stages

The paper's organizing device is a **research lifecycle**: eight interconnected stages grouped into four
phases, each phase serving "a shared function in the production, validation, and communication of scientific
knowledge" (Section 2.1).

- **Phase 1 — Creation** (produces the research contribution and its evidence):
  - **S1 Idea Generation** — hypothesis/direction generation and refinement. Subdivided into (a) LLM
    internal-knowledge generation (direct prompting, iterative refinement, learned quality signals like
    Spark's judge model trained on 600K OpenReview reviews, adaptive test-time compute like IRIS's MCTS),
    (b) external signal-driven generation (knowledge-graph reasoning as in SciAgents/MOOSE-Chem, paper
    retrieval as in SciPIP/IdeaSynth, trend analysis as in Nova), and (c) multi-agent collaborative
    generation (VirSci's virtual scientific community, "Artificial Hivemind" diversity-collapse findings).
  - **S2 Literature Review** — retrieval, survey/related-work generation, and deep research agents
    (OpenScholar, Tongyi DeepResearch, PaperQA2). Four evaluation axes crystallize here: citation accuracy,
    coverage completeness, narrative coherence, factual grounding.
  - **S3 Coding & Experiments** — code generation, paper-to-code translation, experiment orchestration, and
    result analysis (SWE-agent/OpenHands, PaperCoder, AIDE, AlphaEvolve, Karpathy's `autoresearch`).
  - **S4 Tables & Figures** — scientific figure generation, table understanding/generation, formulas and
    algorithm pseudocode (AutoFigure, DeTikZify, AbGen).
- **Phase 2 — Writing** (organizes Creation's outputs into a scholarly argument):
  - **S5 Paper Writing** — semi-automated writing assistance (ScholarCopilot, PaperDebugger, XtraGPT) and
    fully automated paper generation (The AI Scientist, Agent Laboratory, CycleResearcher).
- **Phase 3 — Validation** (external scrutiny and iterative refinement):
  - **S6 Peer Review** — automated review generation, meta-review synthesis, reviewer–paper matching
    (DeepReviewer-14B, MARG, AgentReview, RATE).
  - **S7 Rebuttal & Revision** — reviewer-comment analysis and evidence-grounded rebuttal generation
    (RebuttalAgent, Paper2Rebuttal, DRPG) — the paper calls this the **newest** and most under-served stage.
- **Phase 4 — Dissemination** (converts the validated manuscript into audience-facing artifacts):
  - **S8 Paper2X** — posters (Paper2Poster), slides (PPTAgent, SlideGen), videos/talks (Paper2Video,
    PresentAgent), social media/web (Paper2Web), and **paper-to-agent conversion** (Paper2Agent, which wraps
    a paper + its codebase into an MCP server so the paper becomes queryable/executable rather than only
    readable).

> [!inferred] The eight-stage / four-phase split is the paper's own framework, not this wiki's invention —
> but treating it as the organizing skeleton for `wiki/topics/autoresearch.md` (rather than, say, organizing
> by "system name" or by "training method") is a choice this wiki is making because it is the taxonomy most
> other autoresearch papers in this collection are likely to slot into cleanly.

The lifecycle is explicitly **not strictly linear**: reviewer critiques (S6) can send work back to S3/S4/S5,
and dissemination (S8) can expose ambiguities that trigger revisions in S5 — the paper treats these feedback
loops as central to where AI-assisted workflows silently propagate errors.

## Five methodological families (Section 2.2)

Recurring across all eight stages, not mutually exclusive: **(1) prompt engineering** (no training, lightweight,
prompt-sensitive), **(2) retrieval-augmented generation (RAG)** (grounds outputs in external sources but
doesn't guarantee faithful use of them), **(3) training-free agentic methods** (planning/tool-use/memory/
self-reflection; strong at orchestration, but propagate errors when a sub-step fails), **(4) training-based
methods** (SFT/RLHF/preference optimization specialized to a stage's data distribution; risk overfitting to
narrow benchmark distributions), and **(5) hybrid approaches** (increasingly dominant — e.g., RAG + agentic
planning + fine-tuned submodules together). Table 1 in the source maps which families dominate at each of
the eight stages.

## Five central findings

1. AI capability is strongest on **structured, grounded, tool-mediated** tasks and drops sharply on
   **open-ended tasks requiring novelty, implicit domain knowledge, or scientific judgment**.
2. **Artifact generation consistently outpaces verification** — systems can produce a plausible output faster
   than they (or reviewers) can confirm it is correct, faithful, or meaningful.
3. **Human-governed collaboration**, not full autonomy, is the most reliable deployment mode validated so far
   — e.g., the ICLR 2025 randomized study found LLM feedback on human reviews improved review quality in 89%
   of cases without moving acceptance rates, whereas standalone AI review inflates scores and misclassifies
   ~96% of rejected papers as acceptable.
4. Effective systems converge on **layered architectures**: an exploration layer (search over hypotheses/code
   variants), an execution layer (tool interaction), and a verification layer (execution feedback, citation
   validation, critique).
5. AI use in research has become a **governance problem, not a detection problem** — AI text detectors are
   unreliable (high false-positive rates on formal/non-native prose), so venues are shifting from "detect" to
   "declare" policies; one 2026 conference rejected 497 papers for AI-use policy violations.

## The recurring capability-boundary pattern, stage by stage

The paper's most citable empirical numbers, useful for grounding claims other papers in this wiki might make:

- **S1 Idea Generation**: LLM-generated ideas rated higher in novelty than human ideas in a 100+-researcher
  study (Si et al., p<0.05), but degrade far more after implementation (Δ = −1.98 vs. −0.63 for human ideas —
  the "ideation–execution gap"). IdeaBench: novelty scores >0.6 but feasibility <0.5. "Artificial Hivemind"
  study: LLM-generated ideas cluster in narrow regions of idea space — diversity collapse looks structural,
  not fixable by adding more agents.
- **S2 Literature Review**: fastest-maturing stage (four architectural generations in two years); citation
  top-1 accuracy stuck around 40.1% (ScholarCopilot) — hallucination has shifted from obvious fabrication to
  subtle misgrounding (well-cited-looking claims that aren't actually supported).
- **S3 Coding & Experiments**: the sharpest capability cliff in the survey — 76%+ on SWE-bench Verified vs.
  37–39% on dedicated novel-research-code benchmarks (ResearchCodeBench, SciReplicate-Bench), and 58.6% of
  errors on ResearchCodeBench are *semantic* (code runs but implements the wrong algorithm). MLR-Bench:
  ~80% of fully autonomous results are fabricated.
- **S4 Tables & Figures**: visual plausibility ≠ scientific correctness; TeXpert shows LaTeX accuracy dropping
  from 78.8% to 15% as task complexity increases.
- **S5 Paper Writing**: CycleResearcher scores 5.36 on the ICLR scale vs. 5.69 for accepted papers — the gap
  is argumentative depth, not fluency ("valley of mediocrity"). Up to 17.5% of CS abstracts show detectable
  AI modification.
- **S6 Peer Review**: strongest validated mode is AI-improves-human-review, not AI-replaces-review (89% ICLR
  2025 study above). Adversarial fragility is severe — prompt injection (even white-text-on-white) can push
  scores to the maximum, and 5% of manipulated reviews can flip 12% of rankings.
- **S7 Rebuttal & Revision**: rebuttal materially affects borderline papers (score-improved papers: 55.7–57.6%
  acceptance vs. 7.8–12.4% for unchanged scores) but current systems **cannot generate new experimental
  evidence** in response to reviewer requests — the S7→S3 feedback loop remains unautomated. ~25% of ICLR 2025
  rebuttal commitments go unfulfilled in camera-ready versions.
- **S8 Dissemination (Paper2X)**: cost is essentially solved ($0.005/poster); the bottleneck is **trust**, not
  generation cost — video remains the hardest format (must coordinate slides, subtitles, narration, pacing).

## End-to-end systems and evaluation (Section 7)

The paper classifies end-to-end auto-research systems into **four architectural families**: (1) sequential
pipelines (The AI Scientist, Agent Laboratory — simple but error-propagating), (2) search-based/self-improving
systems (AI Scientist v2's tree search, AlphaEvolve-style evolution — better matches how real research
branches and backtracks, but needs reliable evaluators or it optimizes toward superficial novelty),
(3) skill-based/tool-integrated systems (ARIS, Biomni — modular and inspectable, but need shared state across
stages), and (4) multi-agent/community-scale systems (VirSci, ResearchTown — reduce self-confirmation via role
separation, but introduce coordination overhead). Across all four families, coverage of Phase 3 (Validation)
and Phase 4 (Dissemination) lags far behind Phase 1/2 coverage — it's easier to build systems that *generate*
research artifacts than systems that *validate and communicate* them with accountable fidelity.

On evaluation methodology, the paper distinguishes five families: expert evaluation (gold-standard but
expensive/noisy — even human–human inter-rater correlation is only ρ≈0.41), LLM-as-Judge/Agent-as-Judge
(scalable but biased — positivity, length, authority, self-preference biases), automated metrics (narrow,
Goodhart-prone), execution-grounded evaluation (PaperBench decomposes papers into gradable, executable
subtasks), and process/trace-based evaluation (judges *how* a system reached an answer, not just the final
artifact). It argues no benchmark yet evaluates the **full chain from ideation to dissemination** while
preserving cross-artifact traceability — this "lifecycle evaluation gap" is presented as the field's central
open measurement problem.

## Open challenges (Section 7.4)

Six themes: (1) faithfulness across phase boundaries (most consequential failures happen at handoffs between
stages, not within one), (2) scientific judgment/novelty assessment (novelty is socially/temporally situated,
not a fixed property an LLM-as-Judge can score), (3) verification/reproducibility/accountability (rebuttal
commitment-fulfillment gaps as a case study), (4) citation/versioning/source provenance (the same paper exists
as preprint/workshop/conference/journal versions with inconsistent metadata — citation is a "versioned
source-grounding problem," not a formatting task), (5) governance/disclosure/research integrity (shift from
detection to disclosure), and (6) cross-domain generalization and infrastructure access (almost everything
surveyed is CS/ML/NLP; chemistry/biology/medicine/materials science need different evidence standards and are
under-tested; compute/infrastructure access risks becoming a new inequality axis), plus (7) human expertise
and cognitive ownership (delegating too aggressively may erode the judgment skills that define expertise).

## How this paper should shape the wiki

Because this is the field's own self-organizing taxonomy (Appendix B explicitly compares it against five
concurrent surveys — AI4Research, "From Automation to Autonomy," LLM4SR, the Automated Scholarly Paper Review
survey, and the AI Scientist Survey — and shows it is the only one covering all eight stages, notably being
first to treat **S7 Rebuttal & Revision** and **S8 Dissemination** as first-class stages rather than
afterthoughts), it is proposed below as the organizing skeleton for `wiki/topics/autoresearch.md`. Individual
systems this paper names in passing (The AI Scientist, AI Scientist v2, Agent Laboratory, CycleResearcher,
VirSci, ResearchTown, AlphaEvolve, R&D-Agent, Karpathy's `autoresearch`, PaperBench, MLE-Bench, SWE-bench,
KernelBench, and dozens more across Appendix A's four-phase tool inventory) are candidates for their own
`wiki/sources/` pages or mentions as later papers are ingested — this survey is the map, not the territory.
