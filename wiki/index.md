# Wiki index

**Read this first.** A content catalog of everything in this wiki — a collection of papers on
**autoresearch and auto-optimization** (summarized the classic Karpathy way) plus any optional **code
repos** (ingested by the `wikify-ingest-repo` skill). Find the relevant entry here, then drill into its
page. See [`log.md`](log.md) for the chronological history.

## Papers / Sources
One summary page (`wiki/sources/<paper>.md`) per ingested paper; the raw source lives in `raw/papers/`.

- [**tpu_performance_autoresearch_wiki — methodology summary**](sources/tpu-performance-autoresearch-wiki.md)
  — a sibling Karpathy-wiki-pattern project that specializes `autoresearch` from LLM *quality* to TPU
  *performance*: page-type schema, hierarchical `program.md`, falsifiability + HLO/AOT pre-filters, the
  optimization blueprint's phase-ordering discipline, retrospective-driven exhaustion checks, and the
  model-lane skill set. **Re-ingested 2026-08-06** at private-fork `fa480a17`, adding a whole second lane
  and the machinery it forced: the **kernel lane** (kernel-as-model, the K0–K9 loop, cost-ordered
  intervention classes with `refute` as a first-class verdict, downward-spawn/upward-validation coupling,
  lever-coverage as a set-diff); **verification independence** (author ≠ verifier, self-hashed receipts,
  pre-registration enforced by commit ordering, an anti-fabrication lint battery); the **launch-armed
  `process-auditor` watcher** that replaces the now-retired `/loop` skill and Stop hook (check / brake /
  **revive**, with a stop authorization the runner cannot write); and a **regeneratable-vs-earned**
  classification of the wiki's own knowledge files. Codebases, the ~3,580 experiment pages, and TPU-domain
  technical content remain deliberately excluded — methodology only.
- [**Harness Extensibility: Claude Code vs. Antigravity vs. Codex**](sources/2026-08-06-harness-extensibility-comparison.md)
  (2026-08-06) — from the same project: a spec-level comparison of the six agent-extension mechanisms
  (instruction files, skills, sub-agents, MCP, hooks, plugins) framed as *when should a piece of knowledge
  be loaded*, with per-mechanism portability rules and a **measured** worked example (three ~1 KB pointer
  adapters replacing three ~20 KB copies). Key findings: skills are the only ratified cross-vendor format
  and portability ends at the frontmatter; sub-agents share only the concept; hooks are the only mechanism
  that *enforces* anything, with a three-way overlap of exactly `PreToolUse`/`PostToolUse`/`Stop`.
- [**TPU Model Performance Auto-optimization**](sources/2026-05-01-tpu-model-performance-auto-optimization.md)
  (blog, 2026-05-01) — the author's own introduction to the project + first case-study results (Llama 3 8B
  reaching SOTA vs. MaxText; Qwen3 8B four-harness comparison).
- [**Making Karpathy's autoresearch production-ready**](sources/2026-06-05-making-karpathy-autoresearch-production-ready.md)
  (blog, 2026-06-05) — diagnoses loop unreliability as context pollution; introduces `/loop` re-injection,
  a Stop-hook gate, and retrospective-driven exhaustion checks.
- [**Making TPU auto-optimization work with other agents**](sources/2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)
  (blog, 2026-06-26) — decomposes the monolithic loop into skills (shared context) vs. sub-agents (isolated
  context), sub-wiki scoping, and a hypothesis-firing audit against silent no-ops; reports a 4-harness MFU
  comparison.
- [**AI for Auto-Research: Roadmap & User Guide**](sources/ai-for-auto-research-roadmap.md) — the field's own scaffold survey: an 8-stage/4-phase taxonomy (Creation→Writing→Validation→Dissemination) spanning idea generation through peer review and dissemination, with a ~250-system tool inventory and the recurring finding that artifact generation outpaces scientific verification at every stage.
- [**The AI Scientist-v2**](sources/ai-scientist-v2.md) — Sakana AI's template-free agentic-tree-search pipeline (idea → experiments → figures → manuscript → review); produced the first fully AI-generated paper to pass peer review (ICLR 2025 workshop, 6.33 avg). Later published in Nature.
- [**Co-Scientist**](sources/ai-co-scientist.md) — Google's six-agent Gemini system (Generation/Reflection/Ranking/Proximity/Evolution/Meta-review) that generates, debates, and Elo-ranks novel hypotheses, validated on three biomedical problems — but stops at a ranked hypothesis list for a human to test.
- [**RD-Agent (Microsoft)**](sources/rd-agent.md) — a Research→Development LLM-agent loop for autonomous data science, SOTA on MLE-Bench as of mid-2025 (35.1% Any-Medal Rate on the **full 75-task** split), with a quant-finance specialization (RD-Agent(Q)) that co-optimizes trading factors and models via a contextual-bandit scheduler. *The result stands as reported, but the "SOTA" framing does not: by July 2026 [Frontis-MA1's audit](sources/frontis-ma1.md) lists eight systems ≥68% on the 22-task **Lite** split — including R&D-Agent itself at 68.18% on that easier subset under the same GPT-5 backbone. See [MLE agents and their benchmarks](topics/mle-agents-and-benchmarks.md) before comparing any two numbers in this area.*
- [**Darwin Gödel Machine**](sources/darwin-godel-machine.md) — self-referential coding agent that rewrites its own tools/prompts/workflow, keeping each self-edit only if it empirically improves SWE-bench/Polyglot score, searched via a growing archive of variants rather than a single hill-climbing lineage.
- [**AlphaEvolve (DeepMind)**](sources/alphaevolve.md) — Gemini-powered evolutionary coding agent: an LLM proposes code diffs, automated evaluators score them, best survive; discovered a 48-multiplication 4×4 complex matrix-multiply (first sub-Strassen result in 56 years), improved ~50 open math problems, and auto-tuned Google's Borg scheduler, Gemini kernels, TPU circuits, and XLA IR. **Bridges autoresearch and auto-optimization.**
- [**KernelEvolve (Meta)**](sources/kernelevolve.md) — ISCA 2026 deployment report on the wiki's first
  **primarily auto-optimization** system: an agentic tree search (`F, π_sel, O, τ`) that autonomously writes,
  validates, profiles, and optimizes **Triton** kernels across NVIDIA, AMD, and Meta's proprietary **MTIA**
  accelerators, running continuously in ads-ranking production. 480/480 operator-platform configurations
  correct, 100% KernelBench pass rate, **1.25–17×** over PyTorch baselines, weeks → hours. Two mechanisms
  worth stealing: a **single universal operator** driven by retrieval-augmented prompt synthesis instead of
  static `Draft`/`Debug`/`Improve` templates, and a **hand-authored hardware knowledge base** that makes an
  accelerator absent from all training corpora tractable without retraining. Fitness is measured wall-clock
  speedup with `F = 0` on any correctness failure — no LLM judge anywhere in the selection path.
- [**Bilevel Autoresearch**](sources/bilevel-autoresearch.md) — an outer autoresearch loop that reads this wiki's `autoresearch` inner loop's runner code and traces, then generates and injects new Python search mechanisms (Tabu Search, multi-armed bandit, orthogonal design-of-experiments) at runtime, achieving ~5x over the inner loop alone while parameter-level tuning alone gave no reliable gain. Codebase ingested as a code silo — internals at [`code/bilevel-autoresearch/overview.md`](code/bilevel-autoresearch/overview.md).
- [**Frontis-MA1 / OpenMLE**](sources/frontis-ma1.md) — the wiki's first system where the **improver's
  weights** are the thing improved, not its prompts or scaffold. A full open stack for AI4AI in machine
  learning engineering: **OpenMLE-Gym** (5,758 quality-gated executable tasks + sandbox) → **OpenMLE-ERL**
  (execution-grounded SFT + RL) → **OpenMLE-Evo** (experience-guided long-horizon search), unified by four
  atomic operators — `Draft`/`Improve`/`Debug`/`Crossover` — that are simultaneously the *training targets*
  and the *moves the search composes*. The result worth remembering is the two-way ablation: at fixed
  harness, post-training is worth **+21.22 pp** Medal Average on MLE-Bench Lite (reproduced on a second
  backbone); at fixed model, the harness is worth **+7.58 pp**; composed, a **35B open model on one 12 GB
  RTX 4090** reaches **71.21%**, above GPT-5.5 + Codex. Also the wiki's best measurement of search *cost*:
  −41.7% tokens at −12.4% nodes, +84.3% new-best updates per million tokens. Introduces the
  Evolution → Self-evolution → **Meta-evolution** → RSI ladder that now organizes this wiki's
  self-improvement pages. Contests KernelEvolve's universal-operator argument. Code silo ingested —
  internals at [`code/openrsi/overview.md`](code/openrsi/overview.md), including the finding that the
  paper's four-operator vocabulary isn't uniformly realized in the wired code paths (Debug/Crossover only
  fire through the vendored AIRA-Dojo solver, not the primary SFT/RL harnesses).
- [**ResearchGym**](sources/researchgym.md) — TCS Research/Yale's withheld-method benchmark: strips five
  oral/spotlight ICML/ICLR/ACL 2025 papers of their own proposed method, leaving datasets, eval harness, and
  baselines intact, and grades an agent's replacement hypothesis against the paper's own execution scoring
  rather than an LLM judge. A GPT-5 `rg-agent` beats the strongest baseline in only 1 of 15 runs (6.7%) and
  completes 26.5% of sub-tasks on average — yet that one win surpasses an ICML 2025 Spotlight's own
  reference solution outright. The sharpest quantified instance in this wiki of "AI produces research-shaped
  artifacts more readily than it verifies or exceeds real results."
- [**RoboPhD**](sources/robophd.md) — the first controlled, three-way comparison of optimization paradigms
  for evolving agentic code artifacts under a fixed 1,500-evaluation budget: RoboPhD's own **Elo-tournament**
  selection (validation-free — all budget spent on training-data competition, whose per-round comparative
  error reports double as evolution signal), GEPA's Pareto-based selection, and a reimplementation of
  Karpathy's **`autoresearch`** as greedy single-lineage hill-climbing — citing the repo directly and
  confirmed to be the same system this wiki's `autoresearch` silo documents. RoboPhD wins 3 of 4 benchmarks
  (a 22-line ARC-AGI seed agent evolves to 1,013 lines, 27.8%→65.8% accuracy) but loses the simplest task to
  the `autoresearch`-derived agent (87 lines). A validation-budget ablation shows shrinking GEPA's/
  `autoresearch`'s held-out set consistently frees budget for better scores. The `autoresearch`
  reimplementation also independently discovered a simulator oracle exploit — a smaller-scale echo of the
  Darwin Gödel Machine's own evaluation-gaming case study.
- [**Gödel Machines**](sources/goedel-machines.md) — Schmidhuber's 2003 (rev. 2006) foundational theory
  paper the Darwin Gödel Machine is named after and descends from: a self-referential agent that rewrites
  any part of its own code, including its own proof searcher, the instant a formal proof shows the rewrite
  raises expected utility under its own axiomatized world/reward model — a design proven **globally**
  optimal (Theorem 4.1), not just locally better, at the cost of requiring a fully formalized utility
  function and axiom system its own limitations section concedes cannot always be satisfied
  (Gödel/Rice-style undecidability). DGM keeps the self-referential core but discards the provability
  requirement for empirical benchmark validation — this page works out precisely what that substitution
  keeps and discards.
- [**First Steps Toward Automated AI Research (Recursive)**](sources/recursive-automated-ai-research.md) —
  a blog-published early-results report on an automated research system closing propose→implement→run→
  validate→next-experiment with no human step, running many parallel long-horizon threads that combine
  promising branches. Three results: **NanoChat Autoresearch** — built on
  [Karpathy's `autoresearch`](code/autoresearch/overview.md) (the exact repo this wiki's own silo
  documents) — beats the `autoresearch@home` community best (0.9372→0.9109 val BPB) via hashed n-gram
  embeddings gated into attention; a **NanoGPT speedrun** win (79.7s→77.5s) via FP8 attention projections
  and annealed optimizer noise; and an **18% gap-to-optimal reduction on NVIDIA's SOL-ExecBench** (0.699→
  0.754 mean SOL score, 235 kernels) via bit-packed MoE routing and native PTX FP4 kernels. Thin on loop
  mechanism and reward-hacking-detector detail — no full technical report found, only the blog post plus a
  partial-artifacts GitHub repo — so this wiki tracks the reported numbers without treating the mechanism as
  grounded.
- [**KernelBlaster**](sources/kernelblaster.md) — NVIDIA's third concrete
  [`llm-kernel-generation`](concepts/llm-kernel-generation.md) instance, and the wiki's first targeting raw
  **CUDA** rather than Triton or Pallas. Reaches **1.43×/2.50×/1.50×** geomean over PyTorch on KernelBench
  L1/L2/L3 via **MAIC-RL**: a compact (~50 KB) Persistent CUDA Knowledge Base of
  `⟨bottleneck-signature, ⟨optimization, score⟩⟩` entries, rewritten each round by an LLM-driven
  textual-gradient loop that borrows REINFORCE's vocabulary but never touches model weights — in-context
  memory, not weight-space RL. An ablation with an empty knowledge base runs 1.67× slower, isolating the
  memory (not just profiling access) as the source of the gain.
- [**AI-Supervisor**](sources/ai-supervisor.md) — a solo-authored multi-agent framework built around a
  persistent, typed **Research World Model** (a knowledge graph surviving across separate research
  projects) and a **consensus mechanism** gating gap-verification on agent corroboration counts. Its
  Experiment 3 gives this wiki's cleanest cross-project-persistence result (16 structural links vs. 0 for a
  context-window-memory baseline), but its own seven evaluations are entirely LLM-judged text-vs-text
  comparisons — the execution/reproduction machinery its architecture describes is never shown firing — and
  its consensus mechanism, on inspection, is same-family agents corroborating each other after seeing one
  another's answers, not independent verification.

## Topics
Synthesized prose pages (`wiki/topics/<topic>.md`) — methods, concepts, entities, comparisons that span
papers (e.g. AI-scientist systems, NAS, learned optimizers, kernel auto-tuning).

- [**Wiki-driven autoresearch loop**](topics/wiki-driven-autoresearch-loop.md) — synthesizes
  `karpathy/autoresearch` and the TPU-performance wiki as two instances of one pattern: a fixed cheap
  comparable experiment unit, a domain-grounded observer, falsifiability/pre-registration, an
  accountability mechanism against premature exhaustion, and (from the blog series) the context-pollution
  root cause behind loop unreliability and its skill-vs-sub-agent decomposition fix. Updated 2026-08-06:
  supervision as a **separate process the agent doesn't control** (superseding the retired Stop-hook gate),
  evidence as a forgeable-proof artifact rather than an assertion, coverage as a set-diff against an
  enumerated lever list, the regeneratable-vs-earned split in the wiki's own knowledge, and the
  two-level (model ↔ kernel) coupling rules.
- [**Autoresearch**](topics/autoresearch.md) — the AI-scientist / research-agent landscape organized on the roadmap survey's Creation→Writing→Validation→Dissemination lifecycle: end-to-end pipelines, self-improving loops, hypothesis generation, the industrial R&D loop, and evolutionary algorithm discovery, with "who actually closes the experiment loop" as the cross-cutting axis.
- [**Auto-optimization**](topics/auto-optimization.md) — AutoML / NAS / learned-optimizer / kernel-and-compiler auto-tuning. No longer a stub on the kernel axis: anchored by [KernelEvolve](sources/kernelevolve.md) (production LLM kernel generation across three vendors), with the AlphaEvolve-vs-KernelEvolve comparison, the "value is inversely proportional to ecosystem maturity" gradient, kernel coverage as a binary deployment constraint, and the classical Halide/TVM/Triton lineage. AutoML, NAS, and learned optimizers remain unfilled.
- [**MLE agents and their benchmarks**](topics/mle-agents-and-benchmarks.md) — the machine-learning-engineering
  slice where the loop closes with **no human and no LLM judge** (a submission parses and scores, or it
  doesn't), which is why it became the standard AI4AI / RSI testbed. Holds the field's three-strand
  decomposition (inference harnesses · executable environments · post-training from execution feedback) and
  the benchmark landscape — MLE-Bench and its 22-task **Lite** split, MLE-Dojo, MLE-Smith, MLGym, DSBench,
  MLAgentBench, MLS-Bench, RE-Bench, PaperBench, ResearchGym, NatureBench. **Read the "how to not be misled"
  section before quoting any number from this area**: split, sandbox budget, and run count move these scores
  by tens of points, and single-run cross-vendor gaps under ~8 pp are noise.

## Notes
Cross-cutting answers filed back from queries (`wiki/notes/<note>.md`) — may span papers and code.

- [**Applying Frontis-MA1 / OpenMLE to TPU model + kernel optimization**](notes/frontis-openmle-applied-to-tpu-optimization.md)
  — can the meta-evolution recipe be ported to this project's TPU work, and what would it cost? Verdict:
  **yes for the kernel lane, no for the model lane as an RL environment.** Key finding: the TPU project has
  already run half of Frontis's headline ablation — its four-harness study is *fix the harness, swap the
  model*, and it measured a **14.3 pp MFU** spread (model lane) and **~2×** kernel-speedup spread on an
  identical protocol, so **the model, not the scaffold, is the binding constraint**. The untried arm is
  training one. Covers: what the TPU harness already has that OpenMLE-Evo lacks (author≠verifier, receipts,
  commit-order pre-registration, `refute` as a first-class outcome, HLO pre-filters) and the one thing it
  lacks — **a population with `Crossover`**, absent entirely, where Frontis measured 85–92% of long-horizon
  gain, and whose candidates are already committed to disk unused. Also: why a TPU kernel Gym is *easier*
  to build than MLE-Bench's (the reference implementation is the task spec, the roofline is a free score
  ceiling, the early-kill gate makes most rollouts accelerator-free), a proposed TPU-native operator set
  where **`Refute`** is the cheaply-supervised operator MLE doesn't have, a three-tier effort estimate, and
  the reward-hacking / contamination risks that bite first. **Follow-up section — "could a trained model
  beat Claude Opus 5?"**: the bar is 6.77× on GQA attention, and the README shows it came from **two
  structural jumps** (Codex plateaued at exactly Opus 5's pre-jump 3.73×), so the separating capability is
  structural insight, not stamina or syntax. Key reframing: every such jump is already banked as a class-page
  lever, so the specialist's job is **recognition over a closed lever set, not invention** — with targets
  graded A–E, the distill-from-Opus-5-then-RL-past-it path, and the one cheap experiment that should come
  first (an open 30B as a fourth arm on GQA, to establish the base number Frontis-style deltas require).

## Code repos (optional)
One `wiki/code/<slug>/` per ingested implementation. Open its `overview.md` as a map, then `grep` to the
concept/catalog page and cite the catalog anchor; drop to the pinned source for line-level certainty.

- [**autoresearch**](code/autoresearch/overview.md) — Karpathy's minimal harness for autonomous overnight
  LLM research: an AI agent edits one training file, trains for a fixed 5-minute budget, keeps/discards on
  `val_bpb`, and repeats. Pinned @ `228791f`. Answers: what the agent can change and how a run works
  ([train](code/autoresearch/concepts/train.md)), what's frozen and why the metric can't be gamed
  ([prepare](code/autoresearch/concepts/prepare.md)), and the autonomous
  [experiment loop](code/autoresearch/doc-concepts/autonomous-experiment-loop.md) itself.
- [**ai-scientist-v2**](code/ai-scientist-v2/overview.md) — Sakana AI's fully-autonomous end-to-end research
  pipeline (idea → agentic tree-search experiments → manuscript → LLM/VLM review); the implementation behind
  the paper [`sources/ai-scientist-v2.md`](sources/ai-scientist-v2.md). Pinned @ `96bd516`; 785 symbols across
  33 modules (100% represented), 15 concept + 5 doc-concept pages. Answers: how the tree search picks/expands
  experiments and judges them by LLM+VLM verdict ([ParallelAgent](code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md)),
  the four-stage research protocol ([AgentManager](code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md)),
  the experiment tree data model ([Journal & Node](code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md)),
  literature-grounded [ideation](code/ai-scientist-v2/concepts/ai_scientist-perform_ideation_temp_free.md), and the
  compile-and-measure [manuscript writeup](code/ai-scientist-v2/concepts/ai_scientist-perform_icbinb_writeup.md).
  The tree-search-vs-frozen-metric-ratchet contrast with `autoresearch` is written up in
  [`topics/autoresearch.md`](topics/autoresearch.md).
- [**rd-agent**](code/rd-agent/overview.md) — Microsoft's Research→Development LLM-agent framework for
  autonomous data-science / quant R&D (MLE-Bench SOTA); the implementation behind the paper
  [`sources/rd-agent.md`](sources/rd-agent.md). Pinned @ `4f9ecb0`; 6226 symbols across 541 modules (100%
  represented), 24 concept + 6 doc-concept pages. Answers: how the generic `while time remains` loop engine
  runs Algorithm 1 ([LoopBase](code/rd-agent/concepts/rdagent-utils-workflow-loop.md)), the Research-phase
  proposal machinery and exploration DAG ([Hypothesis/Trace/ExpGen](code/rd-agent/concepts/rdagent-core-proposal.md),
  [DSTrace + schedulers](code/rd-agent/concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)), the
  Development-phase Co-STEER coding agent ([evolving framework](code/rd-agent/concepts/rdagent-core-evolving_framework.md),
  [evaluators](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-evaluators.md),
  [RAG memory](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)), sandboxed
  [execution](code/rd-agent/concepts/rdagent-utils-env.md), and the wall-clock
  [timer](code/rd-agent/concepts/rdagent-log-timer.md) behind "explore early, exploit late". The explicit
  Research/Development split vs. the other silos' loop designs is contrasted in
  [`concepts/research-development-loop.md`](concepts/research-development-loop.md).
- [**pi-autoresearch-vkf**](code/pi-autoresearch-vkf/overview.md) — a `pi` coding-agent extension that turns a
  blind optimization loop into a self-improving researcher with verifiable long-term memory (VKF); its own
  CHANGELOG states it was "Inspired by agentic tree-search (AIDE, The AI Scientist v2) and RD-Agent's
  structured Research→Development cycle" — the cross-pollination of three silos already in this wiki. Pinned
  @ `cd8085d` (`v0.10.0-9-gcd8085d`); 746 symbols across 27 modules (100% represented), 14 concept + 5
  doc-concept pages; adversarial verify caught and fixed ~24 refuted claims across the 14 pages. Answers: how
  the VKF card trust lifecycle (candidate → verified → contradicted/retired) defends against memory poisoning
  ([VKF cards](code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-cards.ts.md)), how the
  experiment search tree judges a node against its *parent's* value rather than one global baseline and
  — unlike AIDE/AI-Scientist-v2 — always hill-climbs from a single best node rather than expanding a
  multi-node frontier ([the search tree](code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-tree.ts.md)),
  how untested ideas are proposed via contradiction mining / cross-domain transfer / composition
  ([hypothesis synthesis](code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md)),
  and the tool spine tying it together
  ([autoresearchExtension](code/pi-autoresearch-vkf/concepts/extensions-pi-autoresearch-vkf-index.ts.md)). The
  tree-search comparison is written up in
  [`concepts/agentic-tree-search.md`](concepts/agentic-tree-search.md).
- [**dgm**](code/dgm/overview.md) — the **Darwin Gödel Machine**: a self-improving coding agent that rewrites
  its own tools/prompts/orchestration and keeps each self-edit only if the edited agent scores better on
  SWE-bench/Polyglot, searched via a **growing archive** of variants (stepping-stone parent selection) rather
  than a single hill-climbing lineage. The implementation behind the paper
  [`sources/darwin-godel-machine.md`](sources/darwin-godel-machine.md). Pinned @ `a565fd2d1d`; 371 symbols
  across 37 modules (100% represented, 10/10 classes), 9 concept + 3 doc-concept pages. Answers: how the
  archive + stepping-stone parent sampling works ([DGM_outer](code/dgm/concepts/DGM_outer.md)), what one
  self-referential edit-and-validate attempt does — diagnose, run the agent in a container to edit itself,
  re-score on the benchmark ([self_improve_step](code/dgm/concepts/self_improve_step.md)), the agent being
  evolved and where "self-referential" actually happens ([coding_agent](code/dgm/concepts/coding_agent.md)),
  the model-agnostic tool-calling ([llm_withtools](code/dgm/concepts/llm_withtools.md)), and how the
  improvement target is chosen from the agent's own failures + own code
  ([prompts-self_improvement_prompt](code/dgm/concepts/prompts-self_improvement_prompt.md)). The
  archive-vs-single-lineage and self-referential contrasts against the other silos are written up in
  [`concepts/evolutionary-self-improvement.md`](concepts/evolutionary-self-improvement.md) and
  [`concepts/self-referential-code-rewriting.md`](concepts/self-referential-code-rewriting.md).
- [**bilevel-autoresearch**](code/bilevel-autoresearch/overview.md) — the **outer** autoresearch loop that
  wraps this wiki's `autoresearch` inner loop; the implementation behind the paper
  [`sources/bilevel-autoresearch.md`](sources/bilevel-autoresearch.md). Pinned @ `2010e95802`; 5644 symbols
  across 118 modules (100% represented, 427/427 classes), 15 concept + 6 doc-concept pages. Answers: the
  never-rewritten Level-1 inner loop ([InnerLoopController](code/bilevel-autoresearch/concepts/core-inner_loop.md))
  and the inner→outer information boundary that hides the task artifact
  ([extract_from_inner](code/bilevel-autoresearch/concepts/core-state.md)); Level 1.5's parameter-only
  freeze/unfreeze control surface ([SearchConfig](code/bilevel-autoresearch/concepts/domains-train_opt-config.md),
  [outer loop](code/bilevel-autoresearch/concepts/domains-train_opt-outer.md)); and the load-bearing **Level 2**
  that writes and injects new Python search-mechanism code — the shared 4-round Explore→Critique→Specify→Generate
  dialogue ([BaseMechanismResearcher](code/bilevel-autoresearch/concepts/core-base_mechanism_research.md)) and
  its two domain implementations that generate + dynamically import + activate-or-revert a mechanism
  ([train_opt](code/bilevel-autoresearch/concepts/domains-train_opt-mechanism_research.md),
  [article_opt](code/bilevel-autoresearch/concepts/domains-article_opt-mechanism_research.md)). Its
  mechanism-level (not artifact-level, not self-referential) place among the other self-improvement silos is
  in [`concepts/mechanism-level-self-improvement.md`](concepts/mechanism-level-self-improvement.md).
- [**openevolve**](code/openevolve/overview.md) — the open-source reimplementation of DeepMind's AlphaEvolve
  recipe; the implementation behind the paper [`sources/alphaevolve.md`](sources/alphaevolve.md). Pinned @
  `39db2f6da8`; 2582 symbols across 219 modules (100% represented, 177/177 classes), 13 concept + 4
  doc-concept pages. Answers: how the main evolution loop ties the three pillars together
  ([OpenEvolve.run](code/openevolve/concepts/openevolve-controller.md)), the MAP-Elites × island-model
  population database that decides which candidates survive
  ([ProgramDatabase](code/openevolve/concepts/openevolve-database.md)), the weighted LLM ensemble that
  proposes mutations ([LLMEnsemble](code/openevolve/concepts/openevolve-llm-ensemble.md)) and the
  prompt assembly that narrates evolutionary state into text
  ([PromptSampler](code/openevolve/concepts/openevolve-prompt-sampler.md)), how an LLM's text diff becomes a
  child program ([SEARCH/REPLACE](code/openevolve/concepts/openevolve-utils-code_utils.md)), and the
  cascade evaluator that scores candidates cheaply-first
  ([Evaluator](code/openevolve/concepts/openevolve-evaluator.md)). Adversarial verify caught and fixed 29
  refuted claims across 12 of the 13 pages. This is the first grounded implementation of
  [`concepts/evolutionary-algorithm-discovery.md`](concepts/evolutionary-algorithm-discovery.md), which was
  previously paper-only.
- [**openrsi**](code/openrsi/overview.md) — Frontis.AI's OpenMLE code release; the implementation behind the
  paper [`sources/frontis-ma1.md`](sources/frontis-ma1.md). Pinned @ `eab056726`; 6234 symbols across 24
  auto-discovered modules (100% represented — 16 deep concept pages over OpenMLE's own code, the remaining
  8 auto-discovered packets under the vendored `OpenMLE-ERL/SFT/slime/` RL-training runtime represented by
  catalog pages only, by design), 16 concept + 3 doc-concept pages; adversarial verify caught and fixed ~20
  refuted claims across the 16 pages. Answers: how a task's hidden test data stays hidden
  ([NodeExecutor](code/openrsi/concepts/OpenMLE-Gym-builder_core-utils-nodes.md),
  [process_runner](code/openrsi/concepts/OpenMLE-Gym-openmle_gym-process_runner.md)); how a sandbox score
  becomes an RL reward via the paper's adaptive-bound `power_clip` and a group-synchronized reward barrier
  ([reward_func_utils](code/openrsi/concepts/OpenMLE-ERL-RL-reward_func_utils.md),
  [generate_mle](code/openrsi/concepts/OpenMLE-ERL-RL-generate_mle.md)); the paper's Eq. 3 three-term
  (exploit/explore/cooling) parent-fitness sampling
  ([program_database](code/openrsi/concepts/OpenMLE-ERL-RL-program_database.md)); how the 26,259-example SFT
  corpus was collected by a decoupled generate/evaluate/reject pipeline
  ([Scheduler](code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)); and OpenMLE-Evo-Max's
  multi-GPU async search resource pool
  ([airaevo_async_resources](code/openrsi/concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)). The
  overview's dedicated comparison table is the load-bearing finding: three independent readings (the SFT
  scheduler, its tree-search event log, and its program database) all confirm the wired `GreedySearch` only
  ever emits `draft`/`improve` — `Debug`/`Crossover` as first-class operators only fire through the
  **vendored** AIRA-Dojo `Evolutionary` solver, not the primary harness this ingest grounds. See
  [`concepts/program-evolution-operators.md`](concepts/program-evolution-operators.md) for how this compares
  against the other silos' operator vocabularies.
- [**autora**](code/autora/overview.md) — Automated Research Assistant: the scope-broadening silo, closing
  the loop over **physical/behavioral** empirical experiments rather than in-silico ones. An
  experimentalist proposes the next experimental condition, an experiment runner executes it (a synthetic
  ground-truth model, or a real human participant via Prolific/Firebase), and a theorist fits an
  interpretable model whose predictions shape the next proposal — all three threaded through one shared,
  immutably-updated `State`. No paper source page — ingested as a repo only.
  `AutoResearch/autora` itself is a **namespace metapackage**: its `pyproject.toml` pins ~20
  separately-published sibling packages (`autora-core`, `autora-experimentalist-*`, `autora-theorist-*`,
  `autora-experiment-runner-*`) behind one `pip install autora`, and its own indexed surface is 16 trivial
  symbols (mkdocs doc-site helpers + one import-smoke test) — so this silo has **0 code concept pages**
  and instead 5 doc-concept pages extracted from the project's own docs. Pinned @ `fc5cc3ea21`. Answers:
  the cycle itself
  ([closed-loop-research-cycle](code/autora/doc-concepts/closed-loop-research-cycle.md)), the shared
  State/Delta object that keeps the three roles independently pluggable
  ([state-and-delta-data-model](code/autora/doc-concepts/state-and-delta-data-model.md)), and the three
  component families
  ([experimentalists](code/autora/doc-concepts/experimentalist-component-family.md),
  [experiment runners](code/autora/doc-concepts/experiment-runner-component-family.md),
  [theorists](code/autora/doc-concepts/theorist-component-family.md)). Has **zero code concept pages** (by
  design — `wikify prepare` correctly found 0 groundable concepts) so it does not appear in `wikify
  connect`'s automated "grounded implementations" lists; instead it is connected via hand-written hub
  prose on [`concepts/closed-loop-experiment-design.md`](concepts/closed-loop-experiment-design.md) — the
  only vocabulary concept it plausibly implements, and only at the documentation level.

## Cross-paper concepts (optional)
Host vocabulary (`wiki/concepts/<key>.md`), wired by the `wikify-connect-repo` skill: each concept page
links **down** to every repo's implementation, and each implementation links back up.

Seeded from the first papers pass (these will be the hook points where code silos connect in):
- [`agentic-tree-search`](concepts/agentic-tree-search.md) — best-first search over a tree of experiment nodes (AI Scientist-v2).
- [`end-to-end-discovery-pipeline`](concepts/end-to-end-discovery-pipeline.md) — idea→experiment→figures→manuscript→review, no human in the content loop.
- [`hypothesis-generation`](concepts/hypothesis-generation.md) — proposing novel testable claims (Co-Scientist).
- [`multi-agent-debate`](concepts/multi-agent-debate.md) — multi-turn argument for generation and bias-reduced ranking.
- [`research-development-loop`](concepts/research-development-loop.md) — the explicit Research→Development split (RD-Agent).
- [`closed-loop-experiment-design`](concepts/closed-loop-experiment-design.md) — feeding each result back into the next decision.
- [`evolutionary-self-improvement`](concepts/evolutionary-self-improvement.md) — archive-based search vs. single-branch hill-climbing (DGM).
- [`self-referential-code-rewriting`](concepts/self-referential-code-rewriting.md) — the agent edits the code that constitutes itself (DGM).
- [`evolutionary-algorithm-discovery`](concepts/evolutionary-algorithm-discovery.md) — code-valued candidates + LLM-as-operator + execution-grounded selection (FunSearch → AlphaEvolve → openevolve).
- [`mechanism-level-self-improvement`](concepts/mechanism-level-self-improvement.md) — optimizing the search *mechanism* that generates future candidates, not the task artifact (Bilevel Autoresearch); sits between artifact-level tuning and full self-referential scaffold rewriting.
- [`llm-kernel-generation`](concepts/llm-kernel-generation.md) — agents authoring accelerator kernels judged by differential correctness + measured wall-clock time; the *optimization* vs. *enablement* split, and why the payoff is inversely proportional to ecosystem maturity (KernelEvolve, AlphaEvolve).
- [`retrieval-augmented-prompt-synthesis`](concepts/retrieval-augmented-prompt-synthesis.md) — composing each iteration's prompt at runtime (diagnose → retrieve → compose) instead of selecting a static operator template; KernelEvolve's universal operator, and the "what the system learned" vs. "what the system was told" distinction across openevolve / rd-agent / pi-autoresearch-vkf.
- [`meta-evolution`](concepts/meta-evolution.md) — **the improver is trained**: search outcomes fed back into the *weights* of the model that proposes variations, not just into search state. Carries the Evolution → Self-evolution → Meta-evolution → RSI ladder that places every self-improvement system in this wiki, and the argument that DGM (rewrites its scaffold, frozen weights) and Frontis-MA1 (trains its weights, fixed scaffold) are **orthogonal halves** of the same ambition, with nothing yet closing both loops.
- [`program-evolution-operators`](concepts/program-evolution-operators.md) — the `Draft`/`Improve`/`Debug`/`Crossover` vocabulary (AIDE → AIRA → OpenMLE): why per-operator context is where the token cost lives, why `Crossover` is the operator most systems lack and where 85–92% of long-horizon gain comes from, and the **live disagreement** with KernelEvolve's single universal operator — including the consequence neither paper states, that a universal operator has nothing to post-train against.
- [`verification-independence`](concepts/verification-independence.md) — **the proposer must not produce the evidence its own verdict cites**. Ranks every system here by how far the grader sits from the proposer (frozen metric file → harness-run evaluator → separate verifier process + self-hashed receipt → an LLM judging its own family's output), and collects the observed failure modes: silent no-ops, self-grading (0 of 4 claimed wins survived re-checking), DGM's demonstrated **objective hacking**, Sakana's **AI CUDA Engineer** finding a memory exploit in its own evaluator (the case showing an independent grader is necessary but *not sufficient* — a hard-enough search also searches for holes in whatever scores it), constraint-gaming when the metric itself can't be gamed, and "a negative result is evidence only if the instrument worked."
