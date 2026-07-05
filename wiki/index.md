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
- [**Bilevel Autoresearch**](sources/bilevel-autoresearch.md) — an outer autoresearch loop that reads this wiki's `autoresearch` inner loop's runner code and traces, then generates and injects new Python search mechanisms (Tabu Search, multi-armed bandit, orthogonal design-of-experiments) at runtime, achieving ~5x over the inner loop alone while parameter-level tuning alone gave no reliable gain. Codebase queued for ingest.

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
