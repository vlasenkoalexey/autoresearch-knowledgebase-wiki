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
  `create-experiment`/`formulate-hypothesis`/`start-experiment`/`stop-experiment`/`ingest-source`/`lint`
  skill set. Codebases, per-model experiment logs, and TPU-domain technical content were deliberately
  excluded — methodology only.
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
- [**RD-Agent (Microsoft)**](sources/rd-agent.md) — a Research→Development LLM-agent loop for autonomous data science, SOTA on MLE-Bench (35.1% Any-Medal Rate), with a quant-finance specialization (RD-Agent(Q)) that co-optimizes trading factors and models via a contextual-bandit scheduler.
- [**Darwin Gödel Machine**](sources/darwin-godel-machine.md) — self-referential coding agent that rewrites its own tools/prompts/workflow, keeping each self-edit only if it empirically improves SWE-bench/Polyglot score, searched via a growing archive of variants rather than a single hill-climbing lineage.
- [**AlphaEvolve (DeepMind)**](sources/alphaevolve.md) — Gemini-powered evolutionary coding agent: an LLM proposes code diffs, automated evaluators score them, best survive; discovered a 48-multiplication 4×4 complex matrix-multiply (first sub-Strassen result in 56 years), improved ~50 open math problems, and auto-tuned Google's Borg scheduler, Gemini kernels, TPU circuits, and XLA IR. **Bridges autoresearch and auto-optimization.**
- [**Bilevel Autoresearch**](sources/bilevel-autoresearch.md) — an outer autoresearch loop that reads this wiki's `autoresearch` inner loop's runner code and traces, then generates and injects new Python search mechanisms (Tabu Search, multi-armed bandit, orthogonal design-of-experiments) at runtime, achieving ~5x over the inner loop alone while parameter-level tuning alone gave no reliable gain. Codebase ingested as a code silo — internals at [`code/bilevel-autoresearch/overview.md`](code/bilevel-autoresearch/overview.md).

## Topics
Synthesized prose pages (`wiki/topics/<topic>.md`) — methods, concepts, entities, comparisons that span
papers (e.g. AI-scientist systems, NAS, learned optimizers, kernel auto-tuning).

- [**Wiki-driven autoresearch loop**](topics/wiki-driven-autoresearch-loop.md) — synthesizes
  `karpathy/autoresearch` and the TPU-performance wiki as two instances of one pattern: a fixed cheap
  comparable experiment unit, a domain-grounded observer, falsifiability/pre-registration, an
  accountability mechanism against premature exhaustion, and (from the blog series) the context-pollution
  root cause behind loop unreliability and its skill-vs-sub-agent decomposition fix.
- [**Autoresearch**](topics/autoresearch.md) — the AI-scientist / research-agent landscape organized on the roadmap survey's Creation→Writing→Validation→Dissemination lifecycle: end-to-end pipelines, self-improving loops, hypothesis generation, the industrial R&D loop, and evolutionary algorithm discovery, with "who actually closes the experiment loop" as the cross-cutting axis.
- [**Auto-optimization**](topics/auto-optimization.md) — AutoML / NAS / learned-optimizer / kernel-and-compiler auto-tuning (stub); currently anchored by the bridge systems AlphaEvolve (superoptimization) and RD-Agent(Q).

## Notes
Cross-cutting answers filed back from queries (`wiki/notes/<note>.md`) — may span papers and code.

_None yet._

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
