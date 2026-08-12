---
title: "AI-Supervisor: Autonomous AI Research Supervision via a Persistent Research World Model"
type: source
authors: Yunbo Long (solo author)
arxiv: 2603.24402
venue: "arXiv preprint, 2026-03 (v2, 26 Mar 2026)"
source: ../../raw/papers/ai-supervisor.pdf
updated: 2026-08-06
---
# AI-Supervisor — summary

## What it is
AI-Supervisor is a solo-authored multi-agent orchestration framework that targets not just research
*execution* but research *supervision* — the literature navigation, gap-finding, and rigor-checking
normally done by an advisor — so that a user with "no domain expertise required" can hand it a plain-
language research interest and receive literature review, gap discovery, method development,
evaluation, and paper writing in return
([raw/papers/ai-supervisor.pdf](../../raw/papers/ai-supervisor.pdf), p.1 Abstract, p.3). Its headline
architectural claim is a **Research World Model (RWM)**: a continuously-evolving, typed,
uncertainty-annotated knowledge graph that serves as shared memory and orchestration backbone
across all agents, explicitly contrasted against what the paper calls "stateless, linear pipelines" that
"process papers sequentially" and "propose ideas without structured gap analysis" (p.1 Abstract). The
abstract names three architectural contributions — structured gap discovery, self-correcting discovery
loops, and cross-domain self-improving development loops — plus a **consensus mechanism** under
which "independent findings are corroborated before being committed to the Research World Model"
(p.1). The framework is released as open-source composable skills
(github.com/autoproflab-debug/AI-Supervisor), is model-agnostic (GPT-4, Claude, Gemini, LLaMA,
Qwen, DeepSeek, p.3), and every one of its seven reported experiments runs on Qwen-72B-Instruct
"to ensure fair comparison," at roughly $80 total cost (p.9).

## Architecture: agents, the Research World Model, and gap discovery
The pipeline runs eight phases, each a transformation of the world model (p.7–9): **Phase 0
(Supervision)** — Paper Reader agents extract seed papers in parallel, a Brainstorm agent (conditioned
on any prior `Wprev` for cross-project transfer) ranks candidate directions, a Query Expander builds
search queries. **Phase 1 (Literature Search)** — 6–12 Venue Search agents run in parallel, one per
venue, with two-pass scoring (`S1` on abstracts keeps the top 20, `S2` on full reads produces the final
ranking, Appendix A.5). **Phase 2a (World Model Construction)** — 20 Paper Extraction agents apply
section-specific extraction: methods sections yield module nodes, results sections yield
benchmark-evaluation edges carrying an actual metric vector, limitations sections yield limitation
nodes; a Module Deduplication agent merges near-duplicate modules, and a Gap Synthesis agent
promotes any limitation shared by ≥3 papers to a field-level gap (Eq. 13, p.17). **Phase 2b (Gap
Probing with Consensus)** — described mechanically below. **Phase 3 (Self-Correcting Development)**
— for each verified gap, search agents retrieve cross-domain techniques and "parallel testing agents
implement and evaluate different techniques, verifying mechanism predictions before building full
methods" (p.8), gated by a 10-criterion quality checklist (Table 2, p.9: novelty, beating ≥2 published
baselines, `p<0.001`/`n≥50`/3 seeds, per-component ablation, reproducibility, honest compute
reporting). **Phases 4–7** run multi-seed evaluation, package code/results, write the paper with
parallel section agents, and route each reviewer weakness back to the phase responsible for it
(novelty concerns → Phase 2b, method weaknesses → Phase 3, etc., p.9).

Formally (Definition 1, p.6), the Research World Model is `W = (V, E, U, M)`: six typed node classes
(paper, method, module, benchmark, gap, limitation); six relation types (`proposes`, `uses`,
`evaluated_on`, `has_limitation`, `causes`, `solves`, plus `equivalent_to` in Appendix B);
`U: V∪E → {0,1}` marking each node/edge unverified (1) or verified (0); and `M` mapping evaluation
edges to a real metric vector. Every node starts at `U=1`; the merge rule
`Ut+1(x) = min(Ut(x), ΔUt(x))` (Appendix A.6) makes verification irreversible — once `U=0` it never
reverts. Gap discovery itself is a two-step formal procedure: a **5-WHY causal chain**
`g →w1 c1 →w2 c2 →w3 c3 →w4 c4 →w5 μ(g)` traces a gap through the graph's module and benchmark
nodes down to a specific mathematical mechanism (Eq. 5, p.7 — the paper's own worked example:
"safety methods degrade" → "Lagrangian methods fail on Benchmark b3" → "the multiplier update
assumes stationarity" → μ(g) = "optimization under non-stationarity"); then that mechanism is mapped
to cross-domain fields and translated into each field's vocabulary, with the explicit constraint
`fi ≠ foriginal` forcing the search outside the gap's home domain (Eq. 6, p.8).

**The consensus mechanism, mechanically (Definition 2, p.6–7).** Given `K` probing agents, the
protocol runs two rounds. **Round 1 (independent):** each agent `k` independently produces gap
candidates `G_k^(1) = a_k(W)` from the world model alone. **Round 2 (shared visibility):** each agent
is now shown the *union of every agent's Round-1 output* and, conditioned on that, produces a
refined finding set `G_k^(2)` plus proposed next-step tasks `P_k^(2)`:
`G_k^(2), P_k^(2) = a_k(W, ∪_j G_j^(1))` (Eq. 2). An orchestrator then aggregates across all agents'
Round-2 outputs, choosing `MERGE`, `KILL`, `REDIRECT`, or `CONTINUE` per line of investigation
(Eq. 3). Crucially, a gap's verification label is a **corroboration count, not an independent
re-derivation**: `U(g) = 0 if |{k : g ∈ G_k^(2)}| ≥ 2, else 1` (Eq. 4) — a gap is "verified" exactly
when at least two of the K agents' post-visibility Round-2 outputs still contain it. The cycle repeats
until no new tasks are proposed or a round limit is hit. Section 2.3 states the design goal directly:
"Only findings corroborated across multiple agents *or verified by empirical testing* are committed to
the KG with U = 0" (p.5) — corroboration and empirical testing are named as two *separate* paths to
`U=0`; the formalized consensus protocol (Eqs. 1–4) covers only the corroboration path, for gap
nodes specifically. Separately, Related Work §2.1 describes a **reproduction** step — "cloning the
top 5 methods into a unified evaluation repository, auto-detecting available compute, and reproducing
each method on its own benchmarks — updating KG edges to verified (U=0) or failed (U=1) before
any gap analysis begins" (p.4) — as the empirical-testing path for method/benchmark edges, distinct
from gap-level consensus.

Appendix D's "Consensus quality bound" models Round-1 agents as independent Bernoulli draws (hit
rate `p`) giving system recall `1-(1-p)^K`, then treats Round-2 corroboration the same way with a
higher rate `p2 > p`, giving pairwise reliability `≥ 1-(1-p2)^2` — the paper reports this is "consistent
with `p2 ≈ 0.5`" given the observed 1.000 recall (p.19).

## Results and evaluation
Seven experiments, all judged by an LLM (never by re-executing code), all on Qwen-72B-Instruct,
total cost ≈$80 (p.9–13):

- **Exp. 1 — Gap discovery** (27 Scientist-Bench tasks, Table 3): AI-Supervisor reaches best-alignment
  4.44/5, precision 0.807, recall 1.000, vs. an LLM-only-brainstorm baseline (4.15, 0.679, 0.926) and a
  divergent-convergent baseline (4.04, 0.755, 0.926); 12/27 tasks hit an exact 5/5 match vs. 6 and 3
  respectively.
- **Exp. 2 — Method development** (5 curated gaps, Table 4): full loop and single-pass both reach
  8.0/10 on the quality gate, but only the full loop grounds all 5 methods cross-domain (5/5 vs. 0/5);
  cross-domain search *without* the quality-gated loop is worst (5.6/10, highest variance 1.2).
- **Exp. 3 — Cross-project persistence** (3 sequential AI-safety projects, Table 5): the persistent RWM
  finds 16 cross-project structural connections and 13 verified edges vs. 0 for isolated runs, a
  context-window-memory baseline, and a static-KG baseline; KG size grows monotonically 7→13→19
  nodes. Context-window memory gets 2/3 "cross-insights" through text recall but zero structural
  connections — the paper's stated reason: "these relationships exist only in graph structure, not
  natural language" (p.11).
- **Exp. 4 — Scalability** (10 tasks, 1/3/5/7 agents, Table 6): gaps/task fall from 6.2 to 3.9 as agent
  count rises (stricter corroboration), while best alignment stays ~4.0; mean alignment peaks at 3
  agents (3.39).
- **Exp. 5 — Consensus quality** (15 tasks, Table 7): consensus beats both individual-best-agent and
  naive-union selection — mean alignment 3.27 vs. 3.16, precision 0.297 vs. 0.240 (+24% relative);
  naive union is *worse* than picking one agent (0.227), i.e. merging without the corroboration filter
  adds noise.
- **Exp. 6 — Cross-domain novelty** (5 gaps, Table 8–9): cross-domain-with-mechanism-analysis wins
  all 5 gaps (20.6/25 avg) vs. within-domain (15.6) and naive cross-domain (10.8, the *worst*
  approach) — confirming the 5-WHY step, not just field-hopping, drives the gain.
- **Cost** (Table 10): AI-Supervisor at $8–16/run (Qwen-72B, listed **"No" GPU**), $50–100 on
  frontier models, ~$0 local, vs. AI Scientist v1 ~$15 (GPU), Agent Lab $2.33–13.10 (config. GPU).

> [!inferred]
> **The paper's own evaluation never exercises the execution/reproduction machinery it specifies.**
> Every quantitative result above is an LLM judging text against text: Appendix F.1's protocol for
> Experiments 1/4/5 is "prompt an LLM judge with the gap description and the target paper's title and
> abstract... score alignment 1–5"; F.2's protocol for Experiment 2 is "the judge receives the method
> description and the gap, then scores each criterion as PASS or FAIL with evidence" — including the
> quality gate's "beats ≥2 published baselines" and "`p<0.001`, `n≥50`, 3 seeds" criteria, graded from a
> method *description*, not a re-run; F.3's "verified edges" metric for Experiment 3 comes from "a
> consistency-checking step where the LLM evaluates whether the edge's claimed metric is supported by
> the paper's description" — again reading, not executing. Two of the three benchmarks (the 5 curated
> gaps, the 3 sequential AI-safety projects) were designed by the paper's own author (Appendix F.2–F.3
> label them "(Designed)"), with no independent ground truth beyond that curation. Table 10 lists **"No"
> GPU** for AI-Supervisor's cost tiers, and the total $80 spent across all seven experiments is far too
> little to have cloned and re-run five baseline methods per gap on real compute as Related Work §2.1's
> "Reproduction" paragraph describes. Read together, the paper specifies a system that clones repos,
> re-runs baselines, and statistically tests methods, but nothing in its own reported evaluation shows
> that machinery firing — the numbers in Section 5 are entirely proxy scores from an LLM reading
> descriptions, not measurements from executed code. This is the wiki's own synthesis from the
> appendix protocols and cost table, not a gap the paper concedes about itself.

## Comparison to Co-Scientist
[Co-Scientist](ai-co-scientist.md) (Google, arXiv:2502.18864) is never mentioned in AI-Supervisor's
related work or its Table 1 comparison — despite being arguably the most prominent prior multi-agent
hypothesis-generation-and-ranking system, the paper benchmarks itself only against AI Scientist v1/v2,
AI-Researcher, Agent Laboratory, SciAgents, ResearchAgent, PaperQA2, and MLR-Copilot (Table 1,
p.6). That gap is worth naming plainly before drawing the comparison this wiki cares about.

**Persistent world model vs. per-run context memory.** Co-Scientist's own paper frames its
"self-improvement" as in-context feedback propagation (the Meta-review agent's critique appended to
other agents' prompts) plus "a persistent context memory for long-horizon state" — explicitly **not**
"an explicit trained or symbolic world model" (see [`ai-co-scientist.md`](ai-co-scientist.md), §"The
multi-agent architecture") — and that memory operates *within* one research goal's run, not across
separate projects. AI-Supervisor's Experiment 3 is a direct, if self-designed, test of exactly this
axis: running 3 sequential projects on one persistent RWM produces 16 structural cross-project
connections and monotonic KG growth, while a "context-window memory" baseline built to simulate
exactly Co-Scientist/Agent-Laboratory-style memory achieves 2/3 text-level "cross-insights" but
**zero** structural connections (Table 5). Whatever one makes of AI-Supervisor's other claims, a typed
graph that survives across projects and lets a later run's gap-discovery agents literally re-read shared
nodes (the paper's own example: a "PPO optimizer" node reused between an RLHF-robustness project
and a Constitutional-AI project, p.11) is a structural capability Co-Scientist's design does not have —
Co-Scientist's memory is prose carried in context, not queryable graph structure.

**Who closes the experiment loop?** This is where the comparison gets murkier than the architecture
suggests. Co-Scientist's paper is explicit and consistent that it *never* executes anything: all three
biomedical validations were confirmed by human-run wet-lab assays outside the system, and the paper
names closing that gap via "laboratory automation platforms" as future work (see `ai-co-scientist.md`,
§"Where Co-Scientist stops"). AI-Supervisor's architecture description reads as claiming the opposite —
Related Work §2.1 describes cloning and re-running baseline methods on real compute, and Phase 3
describes "testing agents [that] implement and evaluate different techniques" before building a full
method, with a quality gate requiring real statistical significance and ablations (Table 2). On paper,
that puts AI-Supervisor's stated design closer to [The AI Scientist-v2](ai-scientist-v2.md) — which
does execute Python and gets back real metrics — than to Co-Scientist's text-only tournament. But
where AI Scientist-v2 *shows* that loop closing (real training-run plots, a workshop-accepted
manuscript) and Co-Scientist is honest that its loop stays open (named compounds, wet-lab IC50
numbers, human-in-the-loop hours quantified), AI-Supervisor's own seven experiments never exhibit
the reproduction/execution step at all — see the `[!inferred]` block above. So on the "who closes the
loop" axis this wiki organizes around, Co-Scientist's position (never, explicitly, and it says so) is
better evidenced by its own paper than AI-Supervisor's implied position (architecturally yes, but
unshown).

**Consensus vs. debate/tournament.** The two systems' "let multiple agents look at each other's work"
mechanisms are structurally different from [`multi-agent-debate`](../concepts/multi-agent-debate.md):
Co-Scientist's Ranking agent runs an Elo tournament with actual multi-turn argumentative debate
between hypotheses to reduce positional bias (see `multi-agent-debate.md`). AI-Supervisor's Round 2
has no argument, no pairwise comparison, and no Elo — it is parallel generation, a shared-visibility
second pass, and a mechanical count of how many agents still list the same candidate (Eq. 4). It is
closer to a self-consistency/majority-vote ensemble than to a debate.

## Judging the consensus mechanism against `verification-independence.md`

> [!inferred]
> The following is this wiki's own reading of AI-Supervisor's consensus mechanism against the strict
> criterion on [`verification-independence.md`](../concepts/verification-independence.md) — "the party
> that produces a candidate must not be the party that produces the evidence its verdict cites" — not a
> claim the AI-Supervisor paper makes about itself.
>
> By that test, the gap-consensus mechanism (Eqs. 1–4) does **not** qualify as genuine verification
> independence. The `K` probing agents that propose gap candidates in Round 1 are the *identical* pool
> that "corroborates" them in Round 2 — same role, same prompt family, same backbone model in every
> reported experiment. Worse, Round 2 is explicitly built on shared visibility: each agent sees the
> union of everyone's Round-1 output *before* producing the finding that gets counted toward
> corroboration (Eq. 2). So the "evidence" that a gap is verified is not an independent party
> re-deriving it blind — it is whether ≥2 members of the same undifferentiated pool, having already
> read the candidate, still list it. That is closer to a self-consistency / majority-vote ensemble than
> to a proposer/grader split at all. It sits at or below [AI Scientist-v2](ai-scientist-v2.md)'s "weak"
> rung on the wiki's independence table (a model of the same family judging the output of the model
> that produced it) — AI Scientist-v2 at least has a role-distinct reviewer step over a *finished*
> artifact, where AI-Supervisor's Round 2 is the same proposers re-voting in the same round, with
> foreknowledge of what they're being asked to agree with.
>
> The one place the design *gestures* at real structural independence — reproduction, "cloning the top
> 5 methods... reproducing each method on its own benchmarks" to set `U=0`/`U=1` on method-benchmark
> edges (§2.1) — would be genuinely closer to `autoresearch`'s frozen-evaluator model *if executed*, but
> per the Results section above it is not exercised anywhere in the paper's own evaluation; even
> Experiment 3's "verified edges" metric resolves to an LLM "evaluat[ing] whether the edge's claimed
> metric is supported by the paper's description" (Appendix F.3) — reading, not re-running. There is
> also an internal tension in Appendix D's "consensus quality bound," which derives a reliability bound
> by treating Round-2 agents as *independent* Bernoulli draws — but Round 2 (Eq. 2) is defined precisely
> to give every agent full visibility of the others' Round-1 answers before that draw, so the
> independence the math assumes is the same shared visibility the protocol exists to break.
>
> Net: AI-Supervisor is a new, precisely-specified data point for the wiki's "same-family agents
> corroborating each other" failure mode, not a counter-example to it — worth adding to
> `verification-independence.md`'s comparison table alongside AI Scientist-v2, at the same "weak"
> distance-from-proposer rung or slightly below it.

## Where this fits in the wiki
See [`../topics/autoresearch.md`](../topics/autoresearch.md) for how this compares to other
AI-scientist systems, especially the "Hypothesis generation and idea evaluation" section's framing of
who closes the experiment loop. See [`ai-co-scientist.md`](ai-co-scientist.md) for the closest architectural
analog (multi-agent, LLM-backed, text-heavy hypothesis pipeline) and
[`ai-scientist-v2.md`](ai-scientist-v2.md) for the system whose code-executing tree search
AI-Supervisor's architecture (but not its own evaluation) claims to resemble. See
[`hypothesis-generation`](../concepts/hypothesis-generation.md) and
[`multi-agent-debate`](../concepts/multi-agent-debate.md) for the two mechanisms this paper's Phase 2b
most directly parallels and diverges from, and
[`verification-independence`](../concepts/verification-independence.md) for the grader-independence
axis this page's closing section evaluates AI-Supervisor against. Raw source:
[`raw/papers/ai-supervisor.pdf`](../../raw/papers/ai-supervisor.pdf).
