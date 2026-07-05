---
title: "The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search"
type: source
authors: Yutaro Yamada, Robert Tjarko Lange, Cong Lu, Shengran Hu, Chris Lu, Jakob Foerster, Jeff Clune, David Ha (Sakana AI)
arxiv: 2504.08066
venue: "arXiv preprint (2025); later Nature (2026)"
source: ../../raw/papers/ai-scientist-v2.pdf
updated: 2026-07-04
---
# The AI Scientist-v2 — summary

## What it is
The AI Scientist-v2 (Sakana AI, arXiv:2504.08066) is an end-to-end agentic system that runs the entire
empirical-ML research loop — idea generation, experiment execution, figure production, manuscript
writing, and paper review — with no human in the content-generation loop, and it is the system behind
**the first fully AI-generated manuscript to pass a peer-review process** at a recognized workshop
([raw/papers/ai-scientist-v2.pdf](../../raw/papers/ai-scientist-v2.pdf), p.1 abstract, p.2). The paper was
posted to arXiv in April 2025 and the line of work was later published in *Nature* in 2026; this summary
is written against the arXiv v2 report, which is the fullest methodological account (p.1).

## Lineage: what v1 did, and why v2 exists
The predecessor, **The AI Scientist-v1** (Lu et al., 2024), had already shown a fully automated pipeline
from idea to manuscript, but it depended on a **human-authored code template as the starting baseline
for every new topic area**, and its experimentation was **strictly linear** — each refinement built
directly on the immediately preceding experiment, with no branching or backtracking (p.1, p.3 §2). Both
constraints capped v1's autonomy: a human had to hand-write a base experiment outline before the system
could do anything, and the "short-sighted experimentation" that resulted from linear search prevented
deep exploration of a hypothesis (p.3 §2, p.4 §3).

The AI Scientist-v2's three headline changes, stated directly against v1, are (p.2, Table 1; p.4 §3):
1. **Domain-general codebase drafting** — templates are eliminated; idea generation and experimentation
   both start from a higher level of abstraction instead of an existing codebase (p.4 §3.1).
2. **Tree-based, parallel experiment planning** — replacing v1's linear search with the *agentic tree
   search* described below, managed by a dedicated experiment-progress-manager agent (p.4–7 §3.2).
3. **VLM-in-the-loop reviewing** — a Vision-Language Model critiques figures during experimentation and
   again during manuscript reflection, which v1 did not have (p.7–8 §3.4).

Table 1 in the paper (p.2) crisply tabulates the delta: v1 is "Topic-Specific" / "Linear" / no parallel
experiments / no VLM reviewer / "Not Submitted" (to peer review); v2 is "Domain-General" / "Tree-Based" /
parallel experiments / VLM reviewer / "Workshop Acceptance-Worthy."

> [!inferred]
> The framing of v1→v2 as "remove the human-authored template, then everything else follows" is the
> paper's own narrative; it is a reasonable read of the contributions list but is a synthesis of §1–§3
> rather than a single quoted claim.

## More general idea generation (§3.1, p.4)
Rather than proposing incremental modifications to an existing codebase (v1's mode), v2 is prompted to
engage in open-ended thinking "akin to formulating a research abstract or grant proposal before
committing to a specific implementation" (p.4). Crucially, this phase is **literature-grounded**: the
system queries Semantic Scholar during idea formulation to check the proposed concept's novelty and
surface prior work, rather than relying on a post-hoc novelty check alone (p.4).

## The core method: progressive agentic tree search
### The Experiment Progress Manager and four stages (§3.2.1, p.4–5)
Removing the template dependency required a way to structure open-ended experimentation, so v2
introduces an **experiment progress manager agent** that coordinates four stages that mirror how
real scientific projects proceed (p.5):

1. **Preliminary Investigation** — get a minimal working prototype running at all; ends when a basic
   prototype executes successfully.
2. **Hyperparameter Tuning** — turn the prototype into a robust baseline; ends when training curves
   converge and the run succeeds across at least two datasets.
3. **Research Agenda Execution** — systematically run the actual research plan on the tuned baseline;
   ends when the compute budget is exhausted (with a check that flags under-running experiments so the
   system can scale up complexity).
4. **Ablation Studies** — assess the importance of each component; also budget-bounded.

After each stage the manager uses an **LLM evaluator** to pick the best-performing node, carries that
node forward as the seed for the next stage, and — for scientific rigor — launches multiple replications
of the winning experiment to get mean/standard-deviation statistics for the eventual figures (p.5).

### Parallelized agentic tree search (§3.2.2, p.5–7)
This is the mechanism that replaces v1's linear refinement chain. Every node in the tree is a full
experimental attempt: an LLM writes a concrete plan plus the Python code to implement it, the code runs
immediately in an interpreter, and the node is marked **buggy** if execution errors out. If it succeeds,
the run proceeds to a **plotting phase** where the system visualizes the stored numpy results and a
**Vision-Language Model critiques the plot** — unclear labels, missing legends, or misleading
visualizations also get the node marked buggy, with the VLM's feedback attached for the next debugging
attempt (p.5). Nodes that both execute and pass VLM review are **non-buggy** (p.5).

A node's record — code, plan, error trace, runtime, metrics, LLM feedback, plot paths, VLM feedback, and
buggy/non-buggy status — is the unit the search operates over (p.6–7). At each iteration the system picks
several nodes to expand **in parallel**: with a fixed probability it expands a buggy node (prioritizing
debugging), otherwise it uses a **best-first search over non-buggy nodes**, with an LLM judging candidates
on performance metrics, training dynamics, and plot quality (p.7). Beyond plain buggy/non-buggy, the tree
has specialized node types (p.7):
- **Hyperparameter nodes** — explore configurations in Stage 2, tracking what's already been tried so the
  search doesn't repeat itself.
- **Ablation nodes** — the Stage 4 analogue, same anti-repetition bookkeeping.
- **Replication nodes** — re-run a winning experiment under different seeds to get statistics.
- **Aggregation nodes** — don't run new experiments at all; they generate a script that combines
  replication-node results into a single figure showing means and standard deviations.

Per Table 3 (p.21), the search allocates 21 nodes to Stage 1 and 12 each to Stages 2–4, with a debug
probability of 1.0, max debug depth 3, and a 1-hour per-node runtime cap; a full paper run takes "several
hours to a maximum of 15 hours" (p.21). Code generation itself used Claude 3.5 Sonnet (v2); the
LLM/VLM feedback agents and summary-report agent used GPT-4o (Table 2, p.21).

> [!inferred]
> The paper doesn't name this a "MCTS variant" explicitly — it calls it "agentic tree search" and cites
> AIDE (Jiang et al., 2025) as the direct inspiration (p.3–4, p.6). Framing it as best-first search guided
> by an LLM-as-judge, rather than a classic UCB/backprop tree search, is my reading of the described
> mechanism (p.7), not a term the paper uses.

### Dataset loading and the VLM reviewer (§3.3–3.4, p.7–8)
Datasets are pulled via Hugging Face's `datasets.load_dataset` wherever possible — the paper flags this as
"somewhat ad-hoc" since not every dataset repo supports the one-line loader (p.7). The VLM is used twice:
during tree search (critiquing generated plots, as above) and during manuscript writing, where it is
shown a screenshot of each figure alongside its caption and the surrounding "Figure X" text, and checks
for caption/figure misalignment, unclear visuals, and duplicated figures across the main text and
appendix (p.7–8).

## The end-to-end pipeline
Chaining the above together, the full pipeline is: **idea generation** (with Semantic Scholar novelty
checking and idea scoring/archiving) → **tree-based experimentation** across the four manager stages →
**plotting + VLM feedback** → a **manuscript template** and **single-pass manuscript generation**,
followed by a **separate reflection stage** using a reasoning model (o1) rather than v1's incremental
Aider-based editing loop → **LLM paper reviewing** (p.3 Figure 1, p.4 §3). The reflection stage is
also given the target page limit and the current compiled PDF length so it can trim content to fit
submission constraints without manual editing (p.10).

## The peer-review milestone
To evaluate the system rigorously, the authors generated **three complete manuscripts** targeting the
ICLR 2025 "I Can't Believe It's Not Better" (ICBINB) workshop, extracting the workshop's theme from its
website, and submitted them blind among 43 total submissions; reviewers were told in advance that some
submissions might be AI-generated and could opt out of reviewing them (p.8–9 §4.1). One manuscript —
on compositional regularization for sequence models — scored **6.33 average (6, 6, 7)**, enough to clear
the workshop's acceptance bar (roughly top 45% of submissions) and, per the authors, would have been
accepted at meta-review had it been human-authored: **the first fully AI-generated manuscript to
successfully navigate peer review** (p.2, p.9). The other two submissions were not accepted (p.9). Per a
prior arrangement with ICLR leadership and the workshop organizers, the accepted manuscript was withdrawn
after review rather than entered into the official record, and the study ran under University of British
Columbia IRB approval (H24-02652) (p.9, p.13–14).

The paper's own internal review of the accepted paper (p.11–12, Appendix C.1.1) — reproduced in the
supplementary annotations — is candid about real flaws a code-level audit turned up: the regularizer
described in the text as acting on "hidden states" was actually applied to input **embeddings**, not LSTM
hidden states (p.42 code review); the paper's own Figure 3 caption misdescribed validation loss behavior,
and Figure 5's attention-augmented LSTM was reported as "on par" with the plain LSTM when it actually
performed far better (p.11, p.41); and an independent regeneration of the dataset found roughly **57%
train/test overlap** in the arithmetic-expression benchmark (p.11, p.42–43) — a data-leakage issue the
generated manuscript itself did not surface. The two rejected submissions (label-noise calibration,
p.45–57; pest detection, p.58–69) show a similar pattern under the team's own code review: claims in the
text (e.g., that temperature scaling and multi-dataset domain adaptation were evaluated) did not match
what the underlying generated code actually ran (p.55, p.66) — the code implemented temperature scaling
and a domain-discriminator loss but never executed them in the version that ended up in the paper.

## Limitations the authors flag
The paper is explicit that this is a **workshop-level**, not conference-level, result: only one of three
submissions was accepted, workshop acceptance rates (60–80%) are structurally far more forgiving than
main-track rates at ICLR/ICML/NeurIPS (20–30%), and the system "does not yet consistently reach the
rigorous standard required for top-tier conference publications, nor does it even reach workshop-level
consistently" (p.13 §5). Deeper limitations named directly: formulating genuinely novel, high-impact
hypotheses and rigorously justifying design choices with domain expertise remain hard for a purely
automated system (p.13); the internal review separately notes citation hallucinations and insufficient
methodological depth for main-conference rigor (p.9). The authors also frame the withdrawal-after-review
protocol and the IRB process as a deliberate norm-setting exercise, arguing the community has not yet
reached consensus on how (or whether) to admit AI-generated papers into the formal literature (p.13–14).

## Contrast with the Karpathy-ratchet path
The AI Scientist-v2 and Karpathy's [`autoresearch`](../code/autoresearch/overview.md) sit at opposite ends
of the autoresearch design space this wiki tracks. `autoresearch` is deliberately minimal: one file
(`train.py`) an agent may edit, a frozen `prepare.py` that guarantees a single incorruptible scalar metric
(`val_bpb`) under a fixed 5-minute wall-clock budget, and a keep/revert ratchet with no tree search, no
VLM, and no manuscript stage at all — trust comes from the frozen half of the harness, not from an
evaluator agent. The AI Scientist-v2 instead removes *all* fixed scaffolding (no template code at all) and
replaces it with an agentic **tree search plus LLM/VLM judges** deciding what counts as a "better" node —
i.e. it trusts a learned evaluator where `autoresearch` trusts an unfalsifiable metric. The AI Scientist-v2's
own internal code review (p.41–44, p.55–57, p.66–69) is in effect a demonstration of the risk in that
design choice: LLM-evaluated progress can diverge from what the generated manuscript claims (mismatched
captions, unexecuted ablations, undetected train/test leakage), precisely the class of failure the
`autoresearch` ratchet is structurally immune to by keeping the scoring function frozen and out of the
agent's, or an evaluator LLM's, hands.

## Where this fits in the wiki
See [`../topics/autoresearch.md`](../topics/autoresearch.md) for how this compares to other AI-scientist
systems, and the concept pages [`agentic-tree-search`](../concepts/agentic-tree-search.md) and
[`end-to-end-discovery-pipeline`](../concepts/end-to-end-discovery-pipeline.md) for the two mechanisms
this paper contributes. Raw source: [`raw/papers/ai-scientist-v2.pdf`](../../raw/papers/ai-scientist-v2.pdf).
