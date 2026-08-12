# Wiki log

Append-only, chronological. One entry per operation, prefixed so it stays greppable with plain Unix
tools (`grep '^## \[' wiki/log.md | tail -5`). Prefixes: `ingest-code | <slug>` (code repo via the
skill), `ingest | <source>` (article/doc/note), `connect | <scope>` (cross-repo), `lint | <scope>`,
`note | <title>`. Newest at the bottom.

## [2026-07-04] ingest-code | autoresearch
Ingested [karpathy/autoresearch](https://github.com/karpathy/autoresearch) @ `228791f` as a submodule under
`raw/code/autoresearch`. 177 symbols, 2 modules. Wrote concept pages
[train](code/autoresearch/concepts/train.md) and [prepare](code/autoresearch/concepts/prepare.md), an
[overview](code/autoresearch/overview.md), and 4 doc-concepts from `program.md`/`README.md` (autonomous
experiment loop, experiment logging, fixed time budget, single-file agent edits). Finalize green, 100%
symbol coverage (7/7 classes). Adversarial verify caught and fixed one error (Muon momentum is
step-indexed, not `progress`-indexed). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | tpu-performance-autoresearch-wiki
Ingested the methodology layer of [vlasenkoalexey/tpu_performance_autoresearch_wiki](https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki)
@ `3344c6a` — README, SCHEMA, sample-program.md, the optimization blueprint + index, and all 8 procedural
skills (`create-experiment`, `formulate-hypothesis`, `start-experiment`, `stop-experiment`,
`create-retrospective`, `ingest-source`, `edit-model-code`, `lint`), clipped verbatim into
`raw/papers/tpu-performance-autoresearch-wiki/`. Deliberately skipped: ~26 ingested reference codebases
(`wiki/codebases/`), 900+ per-model experiment logs (`wiki/experiments/`), and TPU-domain technical content
(`wiki/concepts/`, `wiki/sources/`) — implementation, not methodology. Wrote
[wiki/sources/tpu-performance-autoresearch-wiki.md](sources/tpu-performance-autoresearch-wiki.md) (summary)
and [wiki/topics/wiki-driven-autoresearch-loop.md](topics/wiki-driven-autoresearch-loop.md) (synthesis
against `karpathy/autoresearch`). Cross-linked from
[code/autoresearch/overview.md](code/autoresearch/overview.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | vlasenkoalexey-blog-autoresearch-series
Ingested the last 3 posts from [vlasenkoalexey/vlasenkoalexey.github.io](https://github.com/vlasenkoalexey/vlasenkoalexey.github.io/tree/main/_posts)
@ `010a622` (2026-05-01, 2026-06-05, 2026-06-26) — the author's own narrative of the
`tpu_performance_autoresearch_wiki` project: initial case studies (Llama 3 8B vs. MaxText; Qwen3 8B
four-harness comparison), the context-pollution diagnosis behind loop unreliability and its `/loop`
Stop-hook + retrospective fixes, and the later skill-vs-sub-agent decomposition (+ sub-wiki scoping +
hypothesis-firing audit) that made the loop portable across Claude Code/Codex/Antigravity. Raw clips in
`raw/papers/2026-0{5,6}-*.md`. Wrote 3 summary pages under `wiki/sources/` and substantially extended
[wiki/topics/wiki-driven-autoresearch-loop.md](topics/wiki-driven-autoresearch-loop.md) with the
context-pollution/decomposition generalization and cross-harness evidence. Registered in
[`index.md`](index.md).

## [2026-07-04] ingest | ai-for-auto-research-roadmap
Downloaded arXiv:2605.18661 ("AI for Auto-Research: Roadmap & User Guide", 18 May 2026) to
`raw/papers/ai-for-auto-research-roadmap.pdf` and read all 65 pages. Wrote
[wiki/sources/ai-for-auto-research-roadmap.md](sources/ai-for-auto-research-roadmap.md) summarizing its
4-phase/8-stage lifecycle taxonomy (Creation→Writing→Validation→Dissemination), 5 methodological families,
5 central findings (verification lags generation; human-governed collaboration beats full autonomy; layered
architectures win; governance is the bottleneck), and 6 open-challenge themes. This paper's structural role
seeded the new [wiki/topics/autoresearch.md](topics/autoresearch.md) scaffold. Part of a 6-paper parallel
pass (Sonnet 5 subagents). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | ai-scientist-v2
Downloaded arXiv:2504.08066 ("The AI Scientist-v2", Sakana AI) to `raw/papers/ai-scientist-v2.pdf` and read
it in full including the annotated appendices. Wrote
[wiki/sources/ai-scientist-v2.md](sources/ai-scientist-v2.md) covering progressive agentic tree search, the
four manager-coordinated stages, template removal vs. v1, the end-to-end pipeline, the first-AI-paper
peer-review milestone (6.33 avg, ICLR 2025 workshop; later Nature), and the paper's own candid failure-mode
audit. Seeded concept pages [agentic-tree-search](concepts/agentic-tree-search.md) and
[end-to-end-discovery-pipeline](concepts/end-to-end-discovery-pipeline.md), and added a subsection to
[topics/autoresearch.md](topics/autoresearch.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | ai-co-scientist
Downloaded arXiv:2502.18864 (Google Co-Scientist, v2 "Accelerating scientific discovery with Co-Scientist")
to `raw/papers/ai-co-scientist.pdf` and read it. Wrote
[wiki/sources/ai-co-scientist.md](sources/ai-co-scientist.md): the six-agent Gemini architecture
(Generation/Reflection/Ranking/Proximity/Evolution/Meta-review), Elo-tournament + scientific-debate ranking,
test-time-compute scaling, three human-confirmed biomedical validations, and the explicit stop at hypothesis
generation (no autonomous experimentation) — the key contrast with AI Scientist-v2 on "who closes the loop."
Seeded [hypothesis-generation](concepts/hypothesis-generation.md) and
[multi-agent-debate](concepts/multi-agent-debate.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | rd-agent
Ingested two companion Microsoft papers as one project: the general R&D-Agent framework (arXiv:2505.14738,
MLE-Bench SOTA 35.1% Any-Medal Rate) → `raw/papers/rd-agent.pdf`, and RD-Agent(Q) (arXiv:2505.15155, NeurIPS
2025) → `raw/papers/rd-agent-quant.pdf`, which specializes the Research/Development split into a five-unit
quant-finance pipeline with a contextual-bandit factor/model scheduler. Wrote
[wiki/sources/rd-agent.md](sources/rd-agent.md) and seeded
[research-development-loop](concepts/research-development-loop.md) and
[closed-loop-experiment-design](concepts/closed-loop-experiment-design.md); added the "Industrial R&D loop"
section to [topics/autoresearch.md](topics/autoresearch.md). Registered in [`index.md`](index.md).

## [2026-07-04] ingest | darwin-godel-machine
Downloaded arXiv:2505.22954 ("Darwin Gödel Machine") to `raw/papers/darwin-godel-machine.pdf` and read it.
Wrote [wiki/sources/darwin-godel-machine.md](sources/darwin-godel-machine.md): the archive-based,
empirically-validated self-modification loop (SWE-bench 20→50%, Polyglot 14.2→30.7% over 80 iters), the
stepping-stone selection ablations, and the Appendix-H objective-hacking case as a Goodhart warning. Seeded
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md) and
[self-referential-code-rewriting](concepts/self-referential-code-rewriting.md), framing `autoresearch` as the
archive-size-1, non-self-referential special case. Registered in [`index.md`](index.md).

## [2026-07-04] ingest | alphaevolve
Downloaded arXiv:2506.13131 ("AlphaEvolve", DeepMind) to `raw/papers/alphaevolve.pdf` and read all 44 pages.
Wrote [wiki/sources/alphaevolve.md](sources/alphaevolve.md): the LLM-driven evolutionary code-search loop
(FunSearch successor, MAP-elites/island database, programmatic `evaluate`), its provably-correct discoveries
(rank-48 4×4 complex matmul; ~50 open math problems) and four production auto-optimization wins (Borg
scheduling, Gemini kernels, TPU RTL, XLA IR). Seeded
[evolutionary-algorithm-discovery](concepts/evolutionary-algorithm-discovery.md); flagged as the bridge
between [topics/autoresearch.md](topics/autoresearch.md) and
[topics/auto-optimization.md](topics/auto-optimization.md) (new stub). Registered in [`index.md`](index.md).

## [2026-07-04] ingest-code | ai-scientist-v2
Ingested [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) @ `96bd516` as a submodule
under `raw/code/ai-scientist-v2` — the implementation behind the paper source
[sources/ai-scientist-v2.md](sources/ai-scientist-v2.md). 785 documentable symbols across 33 modules; 15 deep
concept pages + 5 README doc-concepts; finalize green, 100% symbol coverage (32/32 classes). Core pages:
[ParallelAgent](code/ai-scientist-v2/concepts/ai_scientist-treesearch-parallel_agent.md) (agentic tree search),
[AgentManager](code/ai-scientist-v2/concepts/ai_scientist-treesearch-agent_manager.md) (four-stage protocol),
[Journal & Node](code/ai-scientist-v2/concepts/ai_scientist-treesearch-journal.md) (experiment tree data model),
[ideation](code/ai-scientist-v2/concepts/ai_scientist-perform_ideation_temp_free.md),
[interpreter](code/ai-scientist-v2/concepts/ai_scientist-treesearch-interpreter.md), and
[writeup](code/ai-scientist-v2/concepts/ai_scientist-perform_icbinb_writeup.md);
[overview](code/ai-scientist-v2/overview.md). Adversarial verify on the 5 core mechanism pages caught and fixed
3 errors: AgentManager stage identity is carried by a `stage_number` int field (not purely the `name` string);
the writeup's citation persistence lives in `gather_citations`'s loop (not `get_citation_addition`); and the
interpreter re-sends `SIGINT` each ~1s poll (not once). Registered in [`index.md`](index.md). Connect step next.

## [2026-07-04] connect | 4 concepts wired across 2 repos
Connected `ai-scientist-v2` on the concept axis via `wikify connect --apply`. Wired 4 authoritative
tag-matched vocabulary concepts down to their grounded implementations (and up-linked each silo page):
[agentic-tree-search](concepts/agentic-tree-search.md) → ParallelAgent + AgentManager + Journal/Node;
[end-to-end-discovery-pipeline](concepts/end-to-end-discovery-pipeline.md) → launch_scientist_bfts;
[closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → same three tree-search pages;
[hypothesis-generation](concepts/hypothesis-generation.md) → ideation. Added hub prose above the `connect:auto`
blocks on the two headline concepts framing the tree-search-plus-LLM/VLM-judge path against `autoresearch`'s
frozen-metric ratchet. Left the other 6 vocabulary concepts unconnected (this repo doesn't implement them).

## [2026-07-04] ingest | bilevel-autoresearch
Ingested Qu & Lu, "Bilevel Autoresearch: Meta-Autoresearching Itself" (arXiv:2603.23420) →
`raw/papers/bilevel-autoresearch.pdf`. An outer loop wraps this wiki's own `autoresearch` inner loop
(unmodified) and, at runtime, reads its runner code + search trace and injects new Python search-mechanism
code (Tabu Search, multi-armed bandit, orthogonal design-of-experiments); ~5x val_bpb gain over the inner
loop alone vs. no reliable gain from parameter-only tuning. Wrote
[wiki/sources/bilevel-autoresearch.md](sources/bilevel-autoresearch.md), seeded new concept
[mechanism-level-self-improvement](concepts/mechanism-level-self-improvement.md), added contrastive cross-links
to [self-referential-code-rewriting](concepts/self-referential-code-rewriting.md) and
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md), and added a "Bilevel Autoresearch"
subsection to [topics/autoresearch.md](topics/autoresearch.md). Its codebase
([EdwardOptimization/Bilevel-Autoresearch](https://github.com/EdwardOptimization/Bilevel-Autoresearch)) is
queued for code ingest (after `dgm`). Registered in [`index.md`](index.md).

## [2026-07-04] ingest-code | rd-agent
Ingested [microsoft/RD-Agent](https://github.com/microsoft/RD-Agent) @ `4f9ecb0` as a submodule under
`raw/code/rd-agent` — the implementation behind the paper source [sources/rd-agent.md](sources/rd-agent.md)
(the general R&D-Agent framework + RD-Agent(Q)). 6226 documentable symbols across 541 modules (100%
represented, 592/592 classes); 24 deep concept pages + 6 README doc-concepts; finalize green. Core pages:
[LoopBase](code/rd-agent/concepts/rdagent-utils-workflow-loop.md) (the generic `while time remains` engine
realizing Algorithm 1), [Hypothesis/Trace/ExpGen](code/rd-agent/concepts/rdagent-core-proposal.md) +
[DSTrace + schedulers](code/rd-agent/concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) (the
Research phase), [Experiment/Workspace/Task](code/rd-agent/concepts/rdagent-core-experiment.md) (the shared
currency), the Co-STEER coding agent ([evolving framework](code/rd-agent/concepts/rdagent-core-evolving_framework.md),
[evaluators](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-evaluators.md),
[knowledge management](code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)),
[Env](code/rd-agent/concepts/rdagent-utils-env.md) sandbox, and the
[RDAgentTimer](code/rd-agent/concepts/rdagent-log-timer.md); [overview](code/rd-agent/overview.md).
Adversarial verify on 8 core mechanism pages caught and fixed 4 errors: `withdraw_loop` reloads the
*earliest* (min step-index) dump of the previous loop, not the last (`loop.py:408`); the `-1`→`len-1`
index translation lives in `get_sota_experiment`, not `get_parents` (`proposal.py:309`); only the three
`ExpGen2TraceAndMerge*` dispatchers gate on `merge_hours` (the inner `MergeExpGen`/`ExpGen2Hypothesis`
recombine unconditionally); and `MCTSScheduler` scores over *every* recorded node index while only
`ProbabilisticScheduler` restricts to `get_leaves()` (`trace_scheduler.py:365`). Registered in
[`index.md`](index.md). Connect step next (3rd silo).

## [2026-07-04] connect | 2 concepts wired across 2 repos (rd-agent joined)
Connected `rd-agent` on the concept axis via `wikify connect --apply`. Wired the two strong, tag-matched
vocabulary concepts down to rd-agent's grounded implementations (and up-linked each silo page):
[research-development-loop](concepts/research-development-loop.md) → 10 rd-agent pages (LoopBase, the
Experiment/Task/Trace core, the Co-STEER coder+evaluators+knowledge-mgmt, Env) — RD-Agent is this concept's
canonical instance; [closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → refreshed to
span BOTH repos (8 rd-agent + the 3 existing ai-scientist-v2 tree-search pages). Added hub prose to
`closed-loop-experiment-design` contrasting RD-Agent's explicit Research→Development split (feedback = a
recorded `Trace` driving the next proposal) against ai-scientist-v2's in-tree LLM/VLM-verdict feedback.
Deliberately left rd-agent's other two tag matches — `agentic-tree-search` and `hypothesis-generation` —
unconnected (preferring the two strong matches; connecting everything drowns the pages, per SCHEMA).

## [2026-07-04] ingest-code | pi-autoresearch-vkf
Ingested [EricJahns/pi-autoresearch-vkf](https://github.com/EricJahns/pi-autoresearch-vkf) @ `cd8085d`
(`v0.10.0-9-gcd8085d`) as a submodule under `raw/code/pi-autoresearch-vkf` — a `pi` coding-agent extension
(TypeScript) that turns a blind optimization loop into a self-improving researcher with verifiable long-term
memory (VKF). 746 symbols across 27 modules (100% represented, 72/72 classes); 14 concept pages (autonomy
watchdog, VKF cards, session config, context pruning, terminal dashboard, experiment log, frontmatter
parser, the tool spine, workspace layout, dashboard payload assembly, idea scoring, hypothesis synthesis,
the experiment search tree, the vkf CLI bridge) + 5 README/CLAUDE.md doc-concepts (skills architecture, tool
reference, benchmark methodology, browser dashboard export, configuration env vars). Finalize green on the
first full pass (a dozen dead module-namespace citations — a packet-generation quirk where `Namespace`-kind
symbols aren't in the coverage-documentable set — were de-linked to plain page references rather than
symbol anchors). Adversarial verify (5 parallel passes, one per page-group) checked all 218 load-bearing
claims and refuted/fixed ~24: notably confirmed as *true* (not refuted) the page's central claim that
`selectExpansion` never calls `frontier` — this implementation always hill-climbs from the single current
best node rather than expanding a multi-node frontier, unlike AIDE/The AI Scientist v2's tree search: a real,
citable design contrast, not a bug. Also fixed a `paths.ts` claim that `dashboard.ts`'s top-level exports read
"exclusively through `sessionPaths`" — they also route through `memoryPaths` via `listCards`/`memoryCounts`,
directly contradicting the module's own "two halves mirror the architecture" docstring. Registered in
[`index.md`](index.md). Connect step next (4th silo).

## [2026-07-04] connect | 4 concepts wired across 4 repos (pi-autoresearch-vkf joined)
Connected `pi-autoresearch-vkf` (4th silo) via `wikify connect --apply`, using its own `concepts:` frontmatter
tags (applied during synthesis, not guessed post hoc): [agentic-tree-search](concepts/agentic-tree-search.md)
→ +3 pi-autoresearch-vkf pages (tree.ts, experiments.ts, index.ts) alongside ai-scientist-v2's 3;
[research-development-loop](concepts/research-development-loop.md) → +2 (config.ts, index.ts) alongside
rd-agent's 10; [closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) → +4 (cards.ts,
scoring.ts, tree.ts, index.ts), now spanning all 3 code silos; [hypothesis-generation](concepts/hypothesis-generation.md)
→ +1 (synthesis.ts) alongside ai-scientist-v2's ideation page. Deliberately excluded rd-agent's two
`agentic-tree-search`/`hypothesis-generation` tag matches from those two concepts (via `--exclude`), preserving
the prior connect pass's decision to keep those two selective — but this required a two-call sequence
(`--apply research-development-loop,closed-loop-experiment-design` first with no exclude, then
`--apply agentic-tree-search,hypothesis-generation --exclude <rd-agent's 2 paths>` second) plus a manual fix:
the second call's per-(repo,path) `--exclude` blanket-dropped those same 2 rd-agent pages from *all* keys'
up-block regeneration that call (not just the 2 being applied), silently deleting their
`closed-loop-experiment-design`/`research-development-loop` up-links even though those concepts' down-blocks
(untouched that call) still correctly listed them — a real tool-mechanics gap between `--exclude`'s per-call,
per-(repo,path) scope and the intended per-(repo,path,key) exclusion. Manually restored both up-blocks to
match their down-block state. Did **not** connect `mechanism-level-self-improvement` — no
pi-autoresearch-vkf page was tagged with it (the VKF layer operates the search mechanism, it doesn't optimize
it, so the tag was correctly withheld during synthesis) — nor `end-to-end-discovery-pipeline` (no manuscript/
figures pipeline here). Added hub prose on all 4 connected concept pages: `agentic-tree-search` gets the
sharpest contrast — a source-verified finding that `selectExpansion` never calls `frontier`, so unlike
ai-scientist-v2's multi-node frontier expansion this implementation always hill-climbs from a single best
node; `research-development-loop` contrasts RD-Agent's six fixed components against pi-autoresearch-vkf's
single optimize/ideate config fork; `closed-loop-experiment-design` extends the existing 2-repo comparison to
a 3-way axis (live tree state vs. recorded Trace vs. durable trust-gated VKF card store);
`hypothesis-generation` contrasts Co-Scientist/ai-scientist-v2's LLM-mediated generation against
pi-autoresearch-vkf's deterministic contradiction/transfer/composition mining over already-verified memory.

## [2026-07-05] ingest-code | dgm
Ingested [jennyzzt/dgm](https://github.com/jennyzzt/dgm) @ `a565fd2d1d` (the **Darwin Gödel Machine**,
arXiv:2505.22954) as a submodule under `raw/code/dgm` — the 5th code silo, and the implementation behind the
paper source [`sources/darwin-godel-machine.md`](sources/darwin-godel-machine.md). 371 documentable symbols
across 37 modules (100% represented, 10/10 classes); 9 concept pages + 3 README doc-concepts. Auto-discovery
seeded 7 concepts; added 2 config seed concepts (`DGM_outer`, `self_improve_step`) so the archive/parent-
selection loop and the self-referential edit-and-validate step each got a deep page. Concept pages: the outer
archive loop (`DGM_outer` — stepping-stone `score_child_prop` parent sampling + `keep_all` archive growth),
one self-improvement attempt (`self_improve_step` — diagnose → container-run the agent to self-edit →
re-score on SWE-bench/Polyglot), the coding agent being evolved (`coding_agent`), model-agnostic tool-calling
(`llm_withtools`), the diagnosis-prompt builder (`prompts-self_improvement_prompt`), the bash tool
(`tools-bash`), per-framework test-log parsing (`utils-swe_log_parsers`), the Polyglot Docker image pipeline
(`polyglot-docker_build`), and offline lineage plotting (`analysis-visualize_archive`). Finalize green on the
second pass (first pass hit 4 lint errors — 2 `filter_compiled` citations outside the DGM_outer subgraph,
de-linked to plain-name references; 2 uncited Mechanism steps, re-cited to in-subgraph `main`/`choose_selfimproves`
and one demoted to `[!inferred]`). Adversarial verify (parallel, all 120 load-bearing claims across 9 pages)
refuted + fixed 3: `DGM_outer`'s `best` method sorts *ascending* (takes the lowest scorers — an apparent
upstream bug, now noted in-page rather than described as "top scorers"); `polyglot-docker_build` over-claimed
that `build_instance_image` cascade-removes downstream images (only `get_env_configs_to_build` does, via
`find_dependent_images`); `analysis-visualize_archive` claimed lineage edges are colored by score direction,
but the source renders all edges black (the color code is commented out — only edge *thickness* distinguishes
the lineage). Manually confirmed the load-bearing `coding_agent` claim that `self.self_improve` is nearly
inert (its only use is forcing `instance_id='dgm'` at coding_agent.py:84; `forward()` never branches on it —
the self-referential effect comes entirely from `self_improve_step.py` pointing the agent at DGM's own repo).
Registered in [`index.md`](index.md). Connect step next (5th silo).

## [2026-07-05] connect | 2 concepts wired to dgm (5th silo joined)
Connected `dgm` (5th silo) via `wikify connect --apply self-referential-code-rewriting,evolutionary-self-improvement`
— using dgm's own `concepts:` frontmatter tags (applied during synthesis). Both are DGM-exclusive concepts (no
other silo implements them, correctly): [self-referential-code-rewriting](concepts/self-referential-code-rewriting.md)
→ 3 dgm pages (coding_agent, self_improve_step, prompts-self_improvement_prompt);
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md) → 1 dgm page (DGM_outer). Up-link
blocks written on all 4 dgm silo pages. Added hub prose to both concept pages above their auto blocks:
`evolutionary-self-improvement` now lays out the four-silo ladder ratchet (autoresearch) → single-node
hill-climb (pi-autoresearch-vkf) → best-first tree (ai-scientist-v2) → genuine growing archive (dgm), noting
only DGM keeps every viable variant selectable; `self-referential-code-rewriting` pins down where the
self-reference actually lives (the agent's self_improve flag is nearly inert — the effect is an emergent
wiring effect in self_improve_step pointing the generic agent at its own code) and notes even DGM leaves its
own outer archive loop human-owned. Deliberately did NOT connect `mechanism-level-self-improvement` (no dgm
page tagged it — DGM's outer loop is fixed, not itself optimized, so the tag was correctly withheld) nor any
of the 5 already-connected concepts (dgm implements none of them — not a candidate for any). **Known `--exclude`/
up-link-regeneration bug hit again (differently):** the `--apply` run regenerated ALL silos' up-link blocks
from page frontmatter tags, re-adding `agentic-tree-search` + `hypothesis-generation` up-links to two rd-agent
pages (rdagent-core-proposal, rdagent-scenarios-data_science-proposal-exp_gen-base) even though those two
concepts' down-blocks deliberately exclude rd-agent (the 2026-07-04 pass kept them selective). Since the
regeneration keys off the page's `concepts:` tags rather than actual down-block membership, it re-introduced
the exact links the prior pass had pruned. Restored both rd-agent up-link blocks to their committed
2-concept state (`closed-loop-experiment-design`, `research-development-loop`) and re-ran `wikify finalize
rd-agent` (green, 6226 symbols 100%). ai-scientist-v2 and pi-autoresearch-vkf up-links were untouched (their
tags match their down-block membership). dgm finalize re-confirmed green after connect (371 symbols, 100%).

## [2026-07-05] ingest-code | bilevel-autoresearch
Ingested `bilevel-autoresearch` (https://github.com/EdwardOptimization/Bilevel-Autoresearch) as the **6th
code silo**, pinned @ `2010e958028fa13e5aacfe2bf73d65314ecdde65` (submodule under `raw/code/bilevel-autoresearch`).
This is the implementation behind the already-summarized paper [`sources/bilevel-autoresearch.md`](sources/bilevel-autoresearch.md)
(arXiv:2603.23420) — the **outer** autoresearch loop that wraps this wiki's `autoresearch` inner loop. `wikify
prepare` indexed 5644 symbols (scip-python), auto-seeded 15 concepts from centrality (no config seeds). Wrote
15 grounded concept pages + overview + 6 README doc-concepts. `wikify finalize` green on first pass (lint OK,
100% coverage — 5644/5644 symbols across 118 modules, 427/427 classes; 118 catalog pages). Adversarial `wikify
verify` ran over 185 load-bearing claims across the 15 pages (3 parallel review passes).
Structure mirrors the paper's three levels: **Level 1** = the never-rewritten inner ratchet
([core-inner_loop](code/bilevel-autoresearch/concepts/core-inner_loop.md)) with a hard inner→outer boundary
([core-state](code/bilevel-autoresearch/concepts/core-state.md), `extract_from_inner` returns process stats but
never the task artifact); **Level 1.5** = parameter-only adjustment
([domains-train_opt-config](code/bilevel-autoresearch/concepts/domains-train_opt-config.md) /
[outer](code/bilevel-autoresearch/concepts/domains-train_opt-outer.md), tagged `closed-loop-experiment-design`
only — verified `outer.py` has zero references to Level 2); **Level 2** = code-generating mechanism research
([core-base_mechanism_research](code/bilevel-autoresearch/concepts/core-base_mechanism_research.md) shared 4-round
dialogue + [train_opt](code/bilevel-autoresearch/concepts/domains-train_opt-mechanism_research.md) /
[article_opt](code/bilevel-autoresearch/concepts/domains-article_opt-mechanism_research.md) implementations),
tagged `mechanism-level-self-improvement`. Two domains (train_opt = paper's GPT-pretraining val_bpb headline
experiment; article_opt = no-GPU 5-stage article-revision demo) prove the `core/` bilevel skeleton is
domain-agnostic. Deliberately did NOT tag `self-referential-code-rewriting` (Level 2's own dialogue logic is
fixed/human-authored — only Level 1 is rewritten) or `evolutionary-self-improvement` (no archive — single active
mechanism, generate-then-activate-or-revert, archive size 1), matching the paper's explicit contrasts.
Registered in [`index.md`](index.md) (Code repos section + updated the paper-source line). Connect step next
(6th silo joins).

## [2026-07-05] connect | 2 concepts wired to bilevel-autoresearch (6th silo joined)
Connected `bilevel-autoresearch` (6th silo) into the concept spine. Newly wired the headline concept
[mechanism-level-self-improvement](concepts/mechanism-level-self-improvement.md) via
`wikify connect --apply mechanism-level-self-improvement` — 4 bilevel pages (core-base_mechanism_research,
domains-article_opt-cli, domains-article_opt-mechanism_research, domains-train_opt-mechanism_research), the
only silo that implements it. Then `wikify connect --refresh` so the three already-connected concepts bilevel
also tags picked up its pages: [closed-loop-experiment-design](concepts/closed-loop-experiment-design.md) +5
bilevel pages, [hypothesis-generation](concepts/hypothesis-generation.md) +3, and
[research-development-loop](concepts/research-development-loop.md) +1. Deliberately did NOT connect bilevel to
[self-referential-code-rewriting](concepts/self-referential-code-rewriting.md) or
[evolutionary-self-improvement](concepts/evolutionary-self-improvement.md) — bilevel's Level 2 keeps one active
mechanism (generate → import-validate → activate-or-revert, archive size 1) and its dialogue logic is fixed, so
those pages stay dgm-only in their auto-blocks and contrast bilevel in prose (added a silo `See also` pointer +
`mechanism-level-self-improvement` cross-link to each). Added a "Grounded in code" hub paragraph to the
mechanism-level page above its auto-block, up-linking the bilevel silo overview and the `autoresearch` inner-loop
overview (the fixed-floor ratchet it wraps).
**Known up-link-regeneration bug hit again (rd-agent, as expected):** the `--refresh` regenerated all silos'
up-links + down-blocks from frontmatter `concepts:` tags, re-adding `agentic-tree-search` + `hypothesis-generation`
to the two rd-agent pages (rdagent-core-proposal, rdagent-scenarios-data_science-proposal-exp_gen-base) whose
down-blocks deliberately exclude them. Fix: re-applied those two concepts with the exact-match excludes
(`rd-agent/code/rd-agent/concepts/<page>.md`) to drop rd-agent from their down-blocks, then — because a
single-concept `--apply` regenerates a page's up-link block from only that invocation's keys and so wiped the
two pages' legitimate closed-loop/research-development up-links — manually restored both up-link blocks to their
committed 2-concept state (`closed-loop-experiment-design`, `research-development-loop`). Re-ran `wikify finalize
rd-agent` (green, 6226 symbols 100%) and `wikify finalize bilevel-autoresearch` (green, 5644 symbols 100%).
Verified via before/after snapshots: the only up-link changes are bilevel's 9 new blocks; every other silo
(ai-scientist-v2, pi-autoresearch-vkf, dgm, autoresearch) is byte-identical, and rd-agent's two pages match
their pre-ingest state.

## [2026-07-05] ingest-code | openevolve (7th silo)
Ingested `openevolve` (https://github.com/codelion/openevolve, an open-source reimplementation of DeepMind's
AlphaEvolve) as a git submodule at `raw/code/openevolve`, pinned @ `39db2f6da8`. `wikify prepare` indexed 2590
symbols (scip-python; the vendored scip-typescript/rust-analyzer passes found no TS/Rust of consequence to
index) and auto-seeded 13 concept packets by centrality — synthesized in parallel: the main evolution loop
([openevolve-controller](code/openevolve/concepts/openevolve-controller.md)), the MAP-Elites × island-model
population database ([openevolve-database](code/openevolve/concepts/openevolve-database.md)), process-based
parallelism ([openevolve-process_parallel](code/openevolve/concepts/openevolve-process_parallel.md)), the
weighted LLM ensemble ([openevolve-llm-ensemble](code/openevolve/concepts/openevolve-llm-ensemble.md)) and its
OpenAI-compatible client ([openevolve-llm-openai](code/openevolve/concepts/openevolve-llm-openai.md)), prompt
assembly ([openevolve-prompt-sampler](code/openevolve/concepts/openevolve-prompt-sampler.md)) and its template
registry ([openevolve-prompt-templates](code/openevolve/concepts/openevolve-prompt-templates.md)), the
SEARCH/REPLACE diff mechanism ([openevolve-utils-code_utils](code/openevolve/concepts/openevolve-utils-code_utils.md)),
the cascade evaluator ([openevolve-evaluator](code/openevolve/concepts/openevolve-evaluator.md)) and its
metrics+artifacts contract ([openevolve-evaluation_result](code/openevolve/concepts/openevolve-evaluation_result.md)),
lineage logging ([openevolve-evolution_trace](code/openevolve/concepts/openevolve-evolution_trace.md)),
configuration ([openevolve-config](code/openevolve/concepts/openevolve-config.md)), and the library entry point
([openevolve-api](code/openevolve/concepts/openevolve-api.md)). Wrote [`overview.md`](code/openevolve/overview.md)
and, from the README, 4 doc-concept pages: [EVOLVE-BLOCK markers](code/openevolve/doc-concepts/evolve-block-markers.md),
[reproducibility via hash-derived seeding](code/openevolve/doc-concepts/reproducibility-seeding.md),
[system message design](code/openevolve/doc-concepts/system-message-design.md), and the
[artifacts feedback loop](code/openevolve/doc-concepts/artifacts-feedback-loop.md).

`wikify finalize` needed two repair rounds (a wrong `LLMModelConfig.models` anchor → `LLMConfig.models` in two
pages; several Mechanism/Entry-points items missing an in-subgraph citation) before going green: 2582 symbols
across 219 modules, 100% represented (177/177 classes), 267 deep (10.3%). Adversarial verify then checked ~231
load-bearing claims across all 13 concept pages (13 parallel reviewers) and refuted-and-fixed 29 of them —
notably a reversed operation order in `ProgramDatabase.add` (best-tracking was documented as running before
`_enforce_population_limit`; the source explicitly does it after, to avoid evicting a program before its
best-tracking update), four backwards/incomplete claims in the controller page (sampling wrongly attributed to
the worker process instead of the main-process `_submit_iteration`; "archive" conflated with "population" as
the eviction cap; `current_island` wrongly credited with driving round-robin submission; a reversed
close-tracer-then-pick-best diagram ordering), and a causal claim in process_parallel.md that attributed child
island re-pinning to migration staleness when the source comment names a different bug (issue #391, fallback
sampling) — `migrate_programs` never actually moves a program's own island, it only copies. Re-ran `wikify
finalize openevolve` after all edits: still green, same coverage.

Registered in [`index.md`](index.md) (Code repos section) and connected `evolutionary-algorithm-discovery`
(previously paper-only, now grounded for the first time) — see the following connect entry.

## [2026-07-05] connect | 1 concept wired to openevolve (7th silo joined)
`wikify connect` showed only one vocabulary concept with candidates in openevolve:
[evolutionary-algorithm-discovery](concepts/evolutionary-algorithm-discovery.md), 7/13 pages, 1 repo — no
other already-connected concept (`agentic-tree-search`, `closed-loop-experiment-design`,
`hypothesis-generation`, `research-development-loop`, `mechanism-level-self-improvement`,
`self-referential-code-rewriting`, `end-to-end-discovery-pipeline`, `evolutionary-self-improvement`) listed
openevolve as a candidate, so skipped `--refresh` entirely (nothing for it to pick up) and ran only
`wikify connect --apply evolutionary-algorithm-discovery` — wired 7 openevolve pages (controller, database,
evaluator, llm-ensemble, process_parallel, prompt-sampler, utils-code_utils) into the concept's down-block
and gave each an up-link. This is the concept's first grounded implementation; it was paper-only before
(cited only through AlphaEvolve's white paper). Added a "Grounded in code" hub paragraph above the auto
block, tying the three Core Mechanism pillars to real openevolve symbols (island-partitioned MAP-Elites in
`ProgramDatabase`, the weighted `LLMEnsemble` mutation operator + SEARCH/REPLACE splicing, the cascade
`Evaluator`) and positioning it against the wiki's other self-improvement mechanisms: openevolve evolves an
arbitrary user-supplied target program (unlike DGM's self-referential agent-rewrite or bilevel's
mechanism-rewrite), with a population database closer in spirit to DGM's growing archive than to bilevel's
single-active-mechanism ratchet.

**Known up-link-regeneration bug hit again (rd-agent) — even on a single-concept `--apply`, not just
`--refresh`.** The apply call regenerated up-link blocks for unrelated pages from their frontmatter
`concepts:` tags, re-adding `agentic-tree-search` + `hypothesis-generation` to the same two rd-agent pages
(`rdagent-core-proposal`, `rdagent-scenarios-data_science-proposal-exp_gen-base`) whose down-blocks
deliberately exclude them. Down-blocks on `agentic-tree-search.md`/`hypothesis-generation.md` were
unaffected (no rd-agent entries reappeared there) — only the two pages' own up-link lines regressed. Fix:
manually restored both up-link blocks to their committed 2-concept state
(`closed-loop-experiment-design`, `research-development-loop`), re-ran `wikify finalize rd-agent` (green,
6226 symbols 100%, 592/592 classes). Verified via before/after snapshot diff against a pre-ingest baseline:
the only changes anywhere in `wiki/code/*/concepts/*.md` up-link blocks are openevolve's 7 new ones; every
other silo (ai-scientist-v2, pi-autoresearch-vkf, dgm, bilevel-autoresearch, autoresearch, and rd-agent
post-repair) is byte-identical to its pre-ingest state.

## [2026-07-05] ingest-code | autora (8th and final code silo)
Ingested [AutoResearch/autora](https://github.com/AutoResearch/autora) @ `fc5cc3ea21` as a submodule under
`raw/code/autora`. No paper source page exists for it (repo-only ingest, per instruction). `synthesis_focus`:
the closed-loop empirical/behavioral-cognitive science cycle — experimentalist → experiment-runner →
theorist — as a physical/behavioral loop, not an in-silico ML self-play loop.

`AutoResearch/autora` turned out to be a **namespace metapackage, not a monorepo**: its `pyproject.toml`
declares dependencies on ~20 separately-published, separately-hosted sibling packages (`autora-core`,
nine `autora-experimentalist-*` packages, `autora-theorist-{bms,bsr,darts}`, four
`autora-experiment-runner-*` packages) and vendors none of them. `wikify prepare autora` correctly indexed
only **16 symbols across 3 modules** — all either `mkdocs` doc-site generation helpers or the repo's one
test, `tests/test_core_imports.py` — and derived an agenda of **0 concepts** (no-op converged on the first
run). This is an honest, correct outcome, not a tooling failure: there is no application logic in this
repo to ground a mechanism page in. Rather than force concept pages, broadened `config/autora.md`'s
`docs:` list from just `README.md` to also include `docs/index.md`, `docs/terminology.md`,
`docs/experimentalist/index.md`, `docs/experiment-runner/index.md`, `docs/theorist/index.md` (skipped
`docs/cheat-sheet.md` as install/usage boilerplate) and wrote **5 doc-concept pages** instead: the
closed-loop cycle itself, the shared State/Delta data model (immutable updates via a Delta, threaded
through all three roles), and the three pluggable component families (experimentalist/experiment-runner/
theorist), each naming which sibling package implements which strategy. Grounded the one honest local
citation point — [`test_core_imports`](code/autora/catalog/tests/test_core_imports.md#test_core_imports),
which enumerates the default (non-extra) install surface — everywhere it was relevant; every other claim
about the cycle's mechanics is sourced to the docs, not to code, since none exists locally. Caught and fixed
one drafting error during a self-review pass: the experimentalist doc-concept originally said "ten"
implementations including "Bandit Random," but `docs/experimentalist/index.md`'s table lists only nine —
`bandit-random` is a `pyproject.toml` extra not yet reflected in that doc; corrected the page and flagged
the doc/manifest drift in an `[!inferred]` block. Wrote `wiki/code/autora/overview.md` explaining the
metapackage boundary explicitly (what ships here vs. what's declared-but-elsewhere) plus two Mermaid
diagrams (the closed-loop cycle over the shared State; the metapackage's dependency fan-out). `wikify
finalize autora` green on the first run (no concept-page citations to violate the gate; doc-concept
citations all resolve): 16 documentable symbols across 3 modules, 100% represented, 0% deep (by design —
0 concept pages), 0/0 classes. `wikify verify autora` correctly reports 0 load-bearing claims (verify scopes
to `concepts/` pages, which don't exist here); did a manual accuracy pass over the 5 doc-concept pages
against the source docs instead (caught the "ten vs. nine" error above). Registered in
[`index.md`](index.md) (Code repos section, explicit "no paper source page" note) — see the following
connect entry for how it was (or wasn't) wired into the concept vocabulary.

## [2026-07-05] connect | autora — hub prose only (8th silo joined, no automated grounded link)
`wikify connect` scans `overview.md` + sibling `concepts/` directories to find candidate silo pages; since
autora has **zero `concepts/` pages** (only `doc-concepts/`), it produced **no new candidates for any of
the 9 vocabulary concepts** and does not count toward the tool's own silo count (`wikify connect` still
reports "7 silo(s)" post-ingest). This is a structural property of the tool, not a bug: `doc-concepts/`
pages are explicitly outside the "grounded implementation" contract those down-blocks assert. Per the
task's own framing, autora's experimentalist→experiment-runner→theorist cycle most plausibly corresponds to
[`closed-loop-experiment-design`](concepts/closed-loop-experiment-design.md) — but forcing it into that
concept's auto-generated "Grounded implementations" list (title: "Grounded implementations of
**closed-loop-experiment-design**... generated by `wikify connect`") would misrepresent an ungrounded,
doc-extracted description as equivalent to the other entries' real symbol citations. Instead, added a new
hand-written section, "A different axis: physical/behavioral vs. in-silico closed loops," **above** the
`connect:auto` block (the skill's sanctioned "deepen a hub" step) — framing autora's cycle as closing the
same four-step loop over **physical/behavioral** experiments (a real human participant via Prolific/Firebase,
or a synthetic ground-truth model) rather than the in-silico training runs / code edits / simulated
benchmarks every other silo iterates on, with an explicit `[!inferred]` block stating why it doesn't (and
shouldn't) appear in the auto-generated list below it. Zero other concepts were connected — autora
implements none of the other 8 (no tree search, no self-referential rewriting, no evolutionary archive, no
mechanism-level rewriting); reporting zero for those is the honest outcome, per SCHEMA.

Ran `wikify connect --refresh` to regenerate the 9 already-connected concepts' links. **Known up-link
regeneration bug hit again — 4th time** (previously: rd-agent after openevolve's connect, and twice before
that): the refresh regenerated `agentic-tree-search` and `hypothesis-generation` back onto rd-agent's
`rdagent-core-proposal` and `rdagent-scenarios-data_science-proposal-exp_gen-base` up-link blocks, and this
time — unlike the openevolve-connect round — it also re-added both rd-agent pages into those two concepts'
own **down-blocks** (`agentic-tree-search.md`, `hypothesis-generation.md`), which hadn't happened before.
Root-caused it this time instead of re-patching the rendered blocks: both rd-agent pages' own frontmatter
`concepts:` list still carried all 4 tags (`hypothesis-generation`, `research-development-loop`,
`closed-loop-experiment-design`, `agentic-tree-search`) from the original ingest, even though the connect
step immediately after rd-agent's ingest ([2026-07-04] connect | 2 concepts wired across 2 repos) explicitly
chose to connect only the latter two and leave the other two tag-matches unconnected. `wikify connect`
treats a `concepts:` frontmatter entry as an *authoritative* tag match regardless of what was previously
chosen at `--apply` time, so every subsequent `--refresh` re-derives the two unwanted links from the stale
tags — the three prior "fixes" only reverted the *rendered* block, which was guaranteed to regress on the
next refresh. Fixed the root cause instead: trimmed both pages' frontmatter `concepts:` to
`[research-development-loop, closed-loop-experiment-design]` (verified `concepts:` frontmatter is read only
by `connect.py`'s tag-matcher, so this is safe — no lint/coverage/state code path depends on it), then
re-ran `wikify connect --refresh`. Result: `rdagent-core-proposal.md`/`rdagent-scenarios-...-base.md`'s
up-link blocks and `agentic-tree-search.md`/`hypothesis-generation.md`'s down-blocks are now byte-identical
to their pre-connect committed state (verified via `git diff` — zero diff on all four), and this fix should
hold across future refreshes since the tag source itself is corrected, not just its rendering. Re-ran
`wikify finalize rd-agent`: green, 6226 symbols across 541 modules, 100% represented, 592/592 classes —
unchanged. Full before/after `git diff --stat` across `wiki/` confirms the *only* changes from this
connect step, wiki-wide, are: (1) the two rd-agent frontmatter corrections above, (2) `wiki/code/index.md`
gaining the one-line autora row, and (3) this repo's own manual edits (`index.md`, `log.md`, and the hub
prose on `closed-loop-experiment-design.md`) — no other silo's up-link or down-block changed.

## [2026-08-06] ingest | kernelevolve
Ingested **KernelEvolve: Scaling Agentic Kernel Coding for Heterogeneous AI Accelerators at Meta**
(arXiv:2512.23236 **v4**, 6 Jul 2026; ISCA 2026; project leads Gang Liao, Gaoxiang Liu) — downloaded to
[`raw/papers/kernelevolve.pdf`](../raw/papers/kernelevolve.pdf) (65 pp.) and read in full. Summary page:
[`sources/kernelevolve.md`](sources/kernelevolve.md).

**Why it matters here:** the first ingested paper whose center of mass is **auto-optimization** rather than
autoresearch. It generates/optimizes Triton kernels across NVIDIA, AMD, and Meta's proprietary MTIA, running
continuously in ads-ranking production — 480/480 operator-platform configurations correct, 100% KernelBench
pass rate, 1.25–17× over PyTorch baselines. Mechanism: kernel optimization formalized as graph search
`(F, π_sel, O, τ)` with `F = t_pytorch/t_triton` and `F = 0` on any `allclose`/compile failure; a **single
universal operator** replacing static `Draft`/`Debug`/`Improve` templates; a two-stage
diagnose-then-retrieve prompt pipeline over a ≥100-document hand-authored hardware knowledge base; the search
graph persisted in a relational DB enabling concurrency, checkpointing, and cross-session warm starts.

**Pages touched (11).** New: [`sources/kernelevolve.md`](sources/kernelevolve.md),
[`concepts/llm-kernel-generation.md`](concepts/llm-kernel-generation.md),
[`concepts/retrieval-augmented-prompt-synthesis.md`](concepts/retrieval-augmented-prompt-synthesis.md).
Rewritten: [`topics/auto-optimization.md`](topics/auto-optimization.md) — **de-stubbed** on the kernel axis
(KernelEvolve section, the AlphaEvolve-vs-KernelEvolve comparison, the ecosystem-maturity gradient, kernel
coverage as a binary deployment constraint, the Halide/TVM/Triton/GEVO lineage, a reading queue of
un-ingested kernel-agent papers; AutoML/NAS/learned-optimizers explicitly still stubs). Updated:
[`concepts/agentic-tree-search.md`](concepts/agentic-tree-search.md) (oracle-vs-judge, swappable `π_sel`,
tree-as-database, and the single-vs-multi-operator disagreement),
[`concepts/evolutionary-algorithm-discovery.md`](concepts/evolutionary-algorithm-discovery.md) (KernelEvolve
as a boundary case — evolution is one setting, not the architecture; GEVO added to the lineage),
[`concepts/closed-loop-experiment-design.md`](concepts/closed-loop-experiment-design.md) (a fourth point on
the persistence axis: cross-session warm start, plus the staleness failure mode it introduces),
[`topics/autoresearch.md`](topics/autoresearch.md) (what an ops-side system gives back to the research-loop
page), [`sources/alphaevolve.md`](sources/alphaevolve.md) (sibling comparison + the contested claim below),
[`index.md`](index.md).

**Contradiction flagged.** KernelEvolve §7 characterizes AlphaEvolve as targeting "single hardware platforms
with synthetic workloads… lacking production operator coverage and deployment infrastructure integration."
Against this wiki's own [`sources/alphaevolve.md`](sources/alphaevolve.md) that is only half right: the
Pallas kernel result was measured on real TPUs against Gemini's actual training and the Borg heuristic was
deployed fleet-wide — production, not synthetic. The defensible narrower claim is about heterogeneity.
Recorded on both pages rather than silently resolved.

**Grounding cautions recorded** (v4 preprint internal inconsistencies, in the summary page's "Reading
cautions" section, so later pages don't propagate the wrong number): the headline range is stated four
different ways (1.2× / 1.25× / "up to 17"); MI350 conv1d is 2.54× in text vs. 2.64× in Figure 13, whose
caption says "6.22×" where text and plot both say 6.54×; §5.4's MTIA generation labels are transposed (v3
compared against a nonexistent "v1"; better coverage attributed to v2i when Table 5 shows v3); Table 8 row 1
reports 1.0× where 0.148 ms vs. 0.313 ms is a 0.47× regression; §3.1 and Figure 12 use two different fitness
definitions (speedup vs. 1/latency); and several figures still carry the system's internal name
**AlphaKernel** (`alpha_kernel_*_interpreter`, a stale duplicated §3.4.2 block on p.21).

**Open thread queued:** the cross-session warm start cites a companion paper this wiki lacks — *"Experience
Graphs: The Data Foundation for Self-Improving Agents"* (Liao et al., 2026, arXiv:2606.29823) — the natural
next ingest for the durable-agent-memory thread. Also queued from §1/§7: KernelBench, TritorX
(arXiv:2512.10977), GEAK, Kevin, AutoTriton, KernelLLM, CWM, TritonRL, KernelAgent.

**Not done:** no code silo — KernelEvolve is internal to Meta with no public implementation, so there is
nothing to ingest via `wikify-ingest-repo` and no `connect` step. `llm-kernel-generation` and
`retrieval-augmented-prompt-synthesis` are therefore paper-only concepts for now; they are deliberately
written as hook points for a future kernel-agent silo (TritorX and GEAK are both public).

## [2026-08-06] ingest | frontis-ma1
Ingested **Frontis-MA1 / OpenMLE** — "Training an AI4AI Model towards Recursive Self-Improvement in Machine
Learning Engineering," Horizon Research / Frontis.AI + Tsinghua, [arXiv:2607.28568v1](https://arxiv.org/abs/2607.28568)
(30 Jul 2026), 61 pp — downloaded to [`raw/papers/frontis-ma1.pdf`](../raw/papers/frontis-ma1.pdf). Summary
page: [`sources/frontis-ma1.md`](sources/frontis-ma1.md).

**Why it mattered to this wiki.** Every self-improvement system ingested so far modifies **text** proposed by
a **frozen** model — a training config (`autoresearch`), an agent scaffold (DGM), a search mechanism (Bilevel
Autoresearch), a candidate program (AlphaEvolve/openevolve). This is the first paper where the improver's
**weights** are the target: SFT + RL on the execution outcomes the evolutionary search itself produced, with
`Draft`/`Improve`/`Debug`/`Crossover` serving simultaneously as training targets and as the search's moves.
It also supplies the ladder the wiki's self-improvement pages were missing — Evolution → Self-evolution →
**Meta-evolution** (the improver is trained) → RSI, with rung 4 explicitly *not* claimed.

**New pages (4):** [`sources/frontis-ma1.md`](sources/frontis-ma1.md);
[`concepts/meta-evolution.md`](concepts/meta-evolution.md) (the ladder, the shared-operator-interface
requirement, the DGM-orthogonality argument, and what training on execution outcomes forces you to change);
[`concepts/program-evolution-operators.md`](concepts/program-evolution-operators.md) (the operator
vocabulary, why `Crossover` is the one most systems lack, and the KernelEvolve disagreement);
[`topics/mle-agents-and-benchmarks.md`](topics/mle-agents-and-benchmarks.md) (the three-strand
decomposition, the benchmark landscape, and how to read these numbers without being misled).

**Updated (9):** [`index.md`](index.md) · [`topics/autoresearch.md`](topics/autoresearch.md) (new
self-improving-loops subsection + the ladder) · [`topics/auto-optimization.md`](topics/auto-optimization.md)
(AutoML's target reached by trained code evolution) ·
[`concepts/evolutionary-algorithm-discovery.md`](concepts/evolutionary-algorithm-discovery.md) (a *trained*
mutation operator; the two reward-shaping consequences frozen-model instances never face) ·
[`concepts/evolutionary-self-improvement.md`](concepts/evolutionary-self-improvement.md) (three-factor
selection; a population is also for *recombining*, not only resampling) ·
[`concepts/mechanism-level-self-improvement.md`](concepts/mechanism-level-self-improvement.md) (the rung
above: mechanism-in-weights vs. mechanism-in-text, with the unclaimed combination flagged) ·
[`concepts/self-referential-code-rewriting.md`](concepts/self-referential-code-rewriting.md) (the
contrastive case — "the improver improves" is not "the improver improves itself") ·
[`concepts/agentic-tree-search.md`](concepts/agentic-tree-search.md) (OpenMLE-Evo's experience-guided
expansion + the p99 context result) · [`concepts/closed-loop-experiment-design.md`](concepts/closed-loop-experiment-design.md)
(a fifth feedback destination: the weights; plus the deterministic-record-vs-LLM-prose split) ·
[`concepts/research-development-loop.md`](concepts/research-development-loop.md) (operator seam vs. phase
seam).

**Cross-paper tension recorded, not resolved.** This ingest landed alongside a concurrent `kernelevolve`
ingest, and the two papers disagree directly. KernelEvolve replaces `Draft`/`Debug`/`Improve` with a
**single universal operator**; Frontis-MA1 keeps four and makes them post-training targets. Both cite the
*same* premise (Toledo et al. 2025 — operator design, not search algorithm, is the bottleneck). Wrote it up
as a narrower disagreement than it looks: KernelEvolve's stated objection is to *static prompt templates*,
and OpenMLE-Evo's operators are not static templates (§5.4 builds different runtime context per operator).
Added the consequence neither paper states — **a universal operator has nothing to post-train against**, so
the choice may track frozen-model vs. trainable-model architecture rather than search quality. Recorded on
[`program-evolution-operators`](concepts/program-evolution-operators.md) (full treatment),
[`agentic-tree-search`](concepts/agentic-tree-search.md) (updating the "open disagreement" note the
kernelevolve ingest left there), and
[`retrieval-augmented-prompt-synthesis`](concepts/retrieval-augmented-prompt-synthesis.md).

**Claim contextualized, not overwritten.** [`sources/rd-agent.md`](sources/rd-agent.md)'s "SOTA on
MLE-Bench, 35.1% Any-Medal" is the **full 75-task** split and stands exactly as reported; Frontis-MA1's
Appendix E audit lists R&D-Agent at 68.18% on the 22-task **Lite** split under the same GPT-5 backbone and
12 h/V100 budget — the same system on the easier subset, not a revision. Annotated `index.md` and
`topics/autoresearch.md` to that effect rather than editing the rd-agent page's result.

**Variance caveat carried into every page that quotes a number.** Medal Average carries ±5.7–8.6 pp over
three epochs; the Codex / Claude Code / Gemini CLI references were run **once**; one of 22 tasks is 4.5 pp.
So the quoted findings throughout are the **controlled** comparisons (+21.22 pp post-training at fixed
harness, reproduced at +18.18 pp on a second backbone; +7.58 pp harness at fixed model; the 66-run matched
token study), not the leaderboard placement. The 3.03 pp margin over GPT-5.5+Codex sits inside one σ and is
flagged as such wherever it appears.

**Not done: no code silo — but the repo exists and is a strong candidate.** The title page's release links
render as icon glyphs and do not survive text extraction; recovering them from the PDF's link annotations
gives project <https://frontisai.github.io/OpenRSI>, code **<https://github.com/FrontisAI/OpenRSI>**, and
weights <https://huggingface.co/collections/FrontisAI/frontis-ma1>. The request was a paper ingest, so no
`wikify-ingest-repo` run and no `connect` step — `meta-evolution` and `program-evolution-operators` are
paper-only concepts for now, deliberately written as hook points. Ingesting `OpenRSI` would ground
OpenMLE-Gym's task contract, OpenMLE-ERL's reward shaping (adaptive bounds, entropic advantage), and
OpenMLE-Evo's experience cards / three-factor selection against real symbols; it is also the only wiki
concept pair with **zero** grounded implementations, so it would be the highest-value next silo.
**Queued reading
from §7:** the meta-evolution survey this paper takes its name from (Jiang et al. 2026), AIRA-2
(arXiv:2603.26499) as OpenMLE-Evo's direct ancestor, AIDE (arXiv:2502.13138), MLE-Bench (arXiv:2410.07095),
MLE-Dojo, MLE-Smith, NatureBench (Wang et al. 2026), and ADAS (Hu et al. 2024).

## [2026-08-06] ingest | tpu_performance_autoresearch_wiki (re-ingest) + harness-extensibility comparison

**Re-ingest** of the methodology source first ingested 2026-07-04 (public template @ `3344c6a`), now read
from the private fork `vlasenkoalexey/tpu_performance_autoresearch_wiki_private` @ `fa480a17` (2026-08-05),
on request: *"new updated process for optimizing kernels and interesting ideas for process optimization."*
Same exclusion as the first pass — methodology only, no codebases, no per-model/per-kernel experiment logs
(now ~3,580 pages), no TPU-domain technical content.

**Raw snapshot refreshed** at `raw/papers/tpu-performance-autoresearch-wiki/` — 8 updated files
(`SCHEMA.md` 457 → 686 lines, `README.md` 305 → 524, the blueprint, the model index, and all 8 model-lane
skills) plus 16 new ones: `kernel-experiments-program.md` (the K0–K9 protocol), `kernel-optimization-index.md`,
`BRIEFS.md`, `design-class-catalog.md`, `classes-attention.md` (exemplar class page),
`experiments-program.md` (the model-lane root, which replaced the retired `sample-program.md` template —
kept for provenance), 4 `regenerate-prompts/`, 2 new skills (`author-kernel`,
`formulate-kernel-hypothesis`), and 4 agents (`process-auditor`, `kernel-verifier`, `profile-analyzer`,
`wikify-repo-navigator`). `profile-analyzer-index.md` (55 KB) was **not** clipped — domain-technical
throughout; its methodological role (the cardinal-rule separation from the hypothesis-generation indexes)
is cited from `SCHEMA.md` instead.

**Pages created**: [`sources/2026-08-06-harness-extensibility-comparison.md`](sources/2026-08-06-harness-extensibility-comparison.md)
(the same project's cross-harness design reference — its own source page, raw clip at
`raw/papers/2026-08-06-harness-extensibility-comparison.md`);
[`concepts/verification-independence.md`](concepts/verification-independence.md).
**Pages updated**: [`sources/tpu-performance-autoresearch-wiki.md`](sources/tpu-performance-autoresearch-wiki.md)
(substantially rewritten), [`topics/wiki-driven-autoresearch-loop.md`](topics/wiki-driven-autoresearch-loop.md),
[`topics/auto-optimization.md`](topics/auto-optimization.md),
[`concepts/llm-kernel-generation.md`](concepts/llm-kernel-generation.md), `index.md`.

**Two contradictions filed, not overwritten.** (1) The first ingest reported `/start-experiment`'s
**never-stop mode** — a marker file plus a registered Claude `Stop` hook blocking session termination until
a fresh lane-specific retrospective exists. That machinery, along with the `/loop` re-injection skill and
its opt-in marker, was **retired 2026-07-21**: the hook was harness-specific and opt-in, and could only stop
a turn from *ending*, never restart a session already idle. Filed as a `[!warning]` block on the source page
and on `topics/wiki-driven-autoresearch-loop.md`, which had generalized the hook as *the* accountability
mechanism. (2) `topics/auto-optimization.md` described the project as operating only at model granularity
with KernelEvolve as "the comparison one level down" — it now runs both lanes, explicitly coupled.

**What was new and worth carrying.** The **kernel lane** (kernel-as-model over the same page schema; K0–K9;
a cost-ordered intervention ladder `refute → flag → xla-rewrite → kernel-authored` where authoring is *last*
and `refuted` is a first-class verdict; downward-spawn / upward-validation coupling; `activity:` classes
deciding what a result may claim; one page per mechanism; a flat pre-registered candidate plan as the stop
rule). **Verification independence** — author ≠ verifier ≠ master, stated so it survives collapse into one
agent (*"authoring-phase numbers never graduate into verdict numbers"*), self-hashed receipts, pre-registration
enforced by commit ordering, commit-per-candidate, and a lint battery of named fabrication classes each
carrying its observed incident. The **launch-armed process watcher** — supervision as a separate process
with different lifetime and authority, whose stop authorization is a file the runner cannot write, and
which explicitly *revives* an idle session. **Coverage as a set-diff** against enumerated class-page levers,
keyed to the named lever rather than a self-described "axis," and moved from close time to selection time.
And the **regeneratable-vs-earned** classification of the wiki's own knowledge, with checked-in regenerate
prompts, one-role-one-index scoping, and content-not-paths brief assembly (measured 2/8 → 8/8).

**Reconciled with concurrent work.** A `kernelevolve` / `frontis-ma1` ingest landed in this working tree
mid-session, adding `concepts/llm-kernel-generation.md` and a substantial kernel section to
`topics/auto-optimization.md`. A draft `topics/kernel-level-auto-optimization.md` was therefore **dropped**
rather than published as a competing page; its synthesis was folded into the existing pages instead — a
*directed vs. selection-driven search* comparison on `llm-kernel-generation.md` (the TPU kernel lane against
KernelEvolve and AlphaEvolve/openevolve: what produces the next candidate, whether "no win exists" is
expressible, and why only the directed loop needs a coverage notion) and a `### The TPU autoresearch wiki's
kernel lane` subsection on `auto-optimization.md`.

**Not done:** no code silo (the source is a wiki, not a library — `wikify-ingest-repo` has nothing to index);
no `connect` step (`verification-independence` is a new vocabulary key with plausible implementations in
`openevolve` (cascade evaluator), `dgm` (external benchmark harness), and `autoresearch` (frozen
`prepare.py`) — a candidate for the next `wikify connect --refresh`, left unwired here rather than asserting
grounded links this pass didn't verify).

## [2026-08-06] lint | claim verification of the tpu-performance re-ingest + ingest hold on a confidential source

Verification pass over the claims filed above, checked against the author's internal design doc *"Unified
framework for TPU Performance model auto-optimization"* (Google Doc `11XsyRp_uz…`), plus independent web
verification of one public fact.

**Ingest HOLD — not a scope decision, a disclosure one.** That doc is marked **Confidential** under
Google's data-security policy, carries internal-only references (`go/`, `moma.corp`, `critique.corp`, `cl/`
numbers, internal drive folders, named internal reviewers), and compares the project against unpublished
internal systems. **This repo is public on GitHub** (`vlasenkoalexey/autoresearch-knowledgebase-wiki`,
`isPrivate: false`), so no source page, raw clip, or paraphrase of it has been written. Awaiting the
owner's decision. The doc was *read* for verification only — the checks below cite public artifacts.

**Collateral check on the material that WAS ingested.** The design doc states both wiki repos "were
compiled using only material available in OSS (no private google3 TPU information was used)"; a scan of the
848 KB staged under `raw/papers/tpu-performance-autoresearch-wiki/` for `google3` / `*.corp.google.com` /
`go/` / `cl/` / "confidential" markers returns **zero hits**, consistent with that. The snapshot contains
methodology files only — no `raw/code/` and no experiment data.

**Confirmed.** The four-harness roster (Opus 4.8 / Fable 5 / Codex GPT-5.5 / Antigravity Gemini 3.1 Pro),
the MaxText 39.8% reference at 8k, the 2.48× kernel reference, the author≠verifier + firing-audit +
self-hashed-receipt design, and the process-auditor's rationale (an "audit yourself" instruction placed in
the same document the agent is already failing to follow inherits that document's skip rate — *using the
process to enforce the process is circular*) all check out against the pages filed above.

**Corrected — over-precise numbers.** Per-arm kernel speedups were stated as if settled. The internal
table's cold no-peek campaign gives materially different per-arm values for the same family (notably the
Gemini arm) than the public README/explorer snapshot the pages cite. The numbers were not *wrong* — they
match their cited public source — but their **precision was unwarranted**, so
`sources/tpu-performance-autoresearch-wiki.md`, `topics/auto-optimization.md`, and
`concepts/llm-kernel-generation.md` now attribute them to the public explorer explicitly and flag that the
ordering is the durable result while the per-arm decimals are a live-campaign snapshot. Also dropped the
internal system's name from the public-facing pages in favour of "a hand-tuned reference."

**Added — one public fact worth having.** [`concepts/verification-independence.md`](concepts/verification-independence.md)
gains the **Sakana AI CUDA Engineer** case (Feb 2025): 10–100× speedups announced on KernelBench, walked
back after independent readers found the system had "found a memory exploit in the evaluation code which…
allowed it to avoid checking for correctness" (Sakana's own public update; one reported case was a 3×
*slow*down). Verified independently via web search before filing, not taken on the doc's word. It is the
sharpest case in the collection because the grader *was* separate code and the objective *was* a hardware
measurement, and it still failed — so the page now states that grader independence is **necessary but not
sufficient**, and that best-of-N / evolutionary selection specifically adds the risk of searching for holes
in the evaluator.

**Open lint findings (pre-existing, not from this pass):** 9 broken relative links in code-silo prose —
`code/dgm/concepts/{prompts-self_improvement_prompt,analysis-visualize_archive,tools-bash}.md` use `../`
prefixes for sibling concept pages, and `code/ai-scientist-v2/concepts/{…-utils-metric,…-ideas-…}.md`
reference sibling pages by unqualified filename. Left unfixed: silo prose is skill-generated and
lint-gated, so these should be corrected by the generator (the citation linter checks citations, not prose
links) rather than hand-patched.

## [2026-08-06] note | Applying Frontis-MA1 / OpenMLE to TPU model + kernel optimization
Query: check this project's TPU optimization work against the freshly-ingested
[Frontis-MA1](sources/frontis-ma1.md), assess which RSI ideas transfer to the model and kernel lanes, and
estimate the cost of adapting the OpenMLE stack and training a TPU-optimization model. Filed as
[`notes/frontis-openmle-applied-to-tpu-optimization.md`](notes/frontis-openmle-applied-to-tpu-optimization.md)
— the wiki's first `notes/` page.

**Verdict: yes for the kernel lane, no for the model lane as an RL environment.** Read
[`sources/tpu-performance-autoresearch-wiki.md`](sources/tpu-performance-autoresearch-wiki.md) plus the raw
methodology clips (kernel index, model blueprint, K0–K9 program, `author-kernel`, README) against
[`sources/frontis-ma1.md`](sources/frontis-ma1.md), [`sources/kernelevolve.md`](sources/kernelevolve.md),
and [`sources/alphaevolve.md`](sources/alphaevolve.md).

**Headline finding — the TPU project already ran half of Frontis's ablation.** Frontis's key controlled
result is *fix the harness, swap the model* → +21.22 pp. The TPU README's four-harness study is structurally
that same experiment: identical protocol, four frontier models, unattended — 47.3% → 33.0% MFU (model lane,
14.3 pp spread) and 6.77× → 3.51× (kernel lane, ~2×). Model capability, not scaffold, is the binding
constraint on this domain. The arm never run is *train the model*.

**Verified by reading the protocol, not inferred:** the TPU kernel lane has **no crossover / recombination
step anywhere** (grep hits for "crossover" are the small-block tiling threshold and the compute-bound
crossover — unrelated), and no population / parent selection: it is a single-lineage frontier ratchet with
one mechanism per page. Frontis's evidence that this is the expensive omission is its strongest claim
(85–92% of long-horizon gain from late Improve/Crossover; a targeted Crossover beating a seven-step Debug
lineage by 8–11% RMSE). The population *already exists on disk* — `commit-each-candidate` commits every
loser under a machine-readable grammar with `bench()` stdout verbatim — and is read only as
`refuted-patterns.md`.

**Also recorded:** the TPU wiki independently invented Frontis's *novelty* selection factor as hard rules
(lever set-diff, consecutive-lever limit, bounded deferral) and covers *quality* via
`expected_gain × confidence / effort` — the missing factor is **`progress`** (gain over parent), which a
single-lineage ratchet cannot express. Its harness is *ahead* of OpenMLE-Evo on rigor (author≠verifier,
self-hashed receipts, commit-order pre-registration, firing audit, `refute` as a first-class outcome, HLO/AOT
pre-filters — Frontis has none of these) and behind on search. And a TPU kernel Gym is **easier** to build
than MLE-Bench's: the reference implementation is the task spec, the roofline is a free score ceiling (no
need for OpenMLE's learned adaptive bounds), op-points are enumerable from real profiles via the existing
downward-spawn rule, and the early-kill gate makes most rollouts accelerator-free — so per-rollout cost is
*below* MLE-Bench's, not above.

**Proposed TPU-native operator set** (do *not* port Draft/Improve/Debug/Crossover literally): the existing
intervention-class ladder — `Diagnose` · **`Refute`** · `Flag` · `Rewrite` · `Author` · `Tune` · `Crossover`
(new). `Refute` is called out as the operator MLE doesn't have and the cheapest verifiable win: frontier
models are trained to produce code, not decline; refuting correctly costs one HLO dump; refuting wrongly is
disproved by any later candidate beating the claimed bound.

**Effort:** Tier 0 (Crossover + population + `progress`, no training) weeks · Tier 1 (SFT on the existing
candidate corpus) ~1–3 months · Tier 2 (full ERL with RL rollouts) ~6–12 months + standing chip budget.
Argued that Tier 1 headroom should *exceed* Frontis's +21 pp because Pallas/Mosaic is genuinely absent from
pretraining (the kernel index's own stated premise; measured 2/8 vs 8/8 path-vs-pasted briefs), which is
KernelEvolve's ecosystem-maturity gradient pointing the same way.

**Honest gaps flagged in the note rather than papered over:** the "~3,580 experiment pages" figure is
ambiguous — the README says 3,580 pages *total* including concept/observation/source/codebase substrate — so
step 1 of any training plan is a real count of `(candidate, verdict, receipt)` triples from git history, and
no estimate should be trusted over it. Risks recorded in bite-order: reward hacking (the project has
*measured* 0-of-4 claimed wins surviving re-check — the existing gates must sit *inside* the RL reward path,
not beside it), train/test contamination (the cold/warm-tier discipline currently governs prompting and must
be extended to a family-level data split), overfitting to generation-specific constants (train mechanism
selection, keep constants in retrieval — the one place KernelEvolve's design should win over Frontis's), and
corpus concentration. Closing argument: TPU optimization is a *shorter* RSI loop than MLE-Bench — it answers
Frontis's own limitation #3 ("especially the improvement of language models themselves"), with AlphaEvolve's
23%-kernel → 1%-training-time Gemini result as the existing proof point — but a much thinner benchmark, so
rigor has to come from the protocol.

## [2026-08-06] note | (addendum) Could a trained model beat Claude Opus 5 at TPU optimization?
Follow-up question on the same note — appended as a section to
[`notes/frontis-openmle-applied-to-tpu-optimization.md`](notes/frontis-openmle-applied-to-tpu-optimization.md)
rather than filed separately, since it refines the same query.

**The bar, from the README's own kernel-lane campaign** (GQA attention, v6e, MaxKernel reference 2.48×):
Claude Opus 5 **6.77× over 22 experiments**, Codex GPT-5.6 3.73× over 9, Gemini Flash 3.6 3.51× over 12.
Opus 5 is absent from the model-lane table, so the bar is well-defined only on the kernel lane.

**The detail that decided the analysis:** the README states Opus 5's jumps (3.73×→4.97× at experiment 8,
→6.03× at 15) are *"single structural changes surrounded by long flat runs of refuted hypotheses"* — and
Codex plateaued at **exactly 3.73×**, Opus 5's pre-jump level. So the separating capability is **structural
insight at the hypothesize/author step**, not stamina, tool discipline, Pallas syntax, or sweep efficiency.
A training plan aimed at any of the latter produces a cheaper, faster model that still stops at 3.73×.

**Reframing recorded:** you don't need to out-invent Opus 5, you need to out-*recall* and out-*apply* the
inventions it already made — every structural jump any arm found is already banked as a `## Levers
(verified)` entry with a receipt. The specialist's task on a new family is recognition over a closed,
enumerated lever set (a classification problem the corpus labels), not open-ended invention. Hence the
proposed benchmark split: held-out families partitioned into **lever-covered** vs **needs-a-new-lever**,
reported separately.

**Targets graded A–E** (Author > Refute > lever-covered end-to-end > new-lever end-to-end > model lane),
with the hybrid — specialist for `Author`/`Tune`/`Refute`, frontier model retained for `Diagnose` — argued
as what Frontis's own "local skill in weights, global composition in harness" principle implies, not as a
hedge (OpenMLE-Evo already runs a separate memory model).

**Path runs *through* Opus 5, not around it:** the existing corpus is likely too small for Frontis's
31-point swing, so training data gets *generated* as Frontis generated 17,245 of its own — sample many
single-shot `Author` candidates from Opus 5 as teacher against the load-mandate brief, filter through the
existing gates (the early-kill gate makes most of this accelerator-free), distill, then RL past the teacher
on `F = t_reference/t_candidate`. ~500 tasks × ~40 samples ≈ 6–10k high-quality examples, comparable to
Frontis's 9,014 trajectory-step examples; dominant cost is teacher inference, not TPU time. This is also the
answer to the structural-insight worry — Frontis's stated reason for having an SFT stage is that teacher
distillation introduces behavior *absent from the base model's sampled support* (Yue et al. 2025), which is
the only stage that can transfer a jump the base would never sample.

**Moving-target caveat + the durable claim:** frontier models improve fast (Frontis's own table: Sonnet 4.6
→ Sonnet 5 → Opus 4.8 → GPT-5.6 Sol), so "our 30B beats the best model" has a short shelf life. The claim
that doesn't decay: a frontier model never learns from this wiki; a specialist does, and the gap compounds
on *this* workload/generation/lane — rung 3 of [meta-evolution](concepts/meta-evolution.md).

**Recommended first experiment (days, not months):** run an open ~30B model as a **fourth arm** on GQA
attention under the existing protocol. Without that base number the result cannot be stated the way Frontis
states its own (a delta over its base under an identical harness), and it discriminates the two regimes:
~3.5× (first plateau) means the gap is two structural moves and the distillation plan is aimed right; ~1.5×
with no compiling Pallas means `Author` capability is the whole project for a while.

## [2026-08-06] note | (addendum 2) The product goal — a cheap model at Claude/Codex capability
Second follow-up on the same note: the goal was restated as **a product built on a cheap model that is as
capable as Claude or Codex** at TPU model + kernel optimization, fed by (a) SFT over all relevant wiki data
and (b) generated trajectories across models and kernels. Appended as a section to
[`notes/frontis-openmle-applied-to-tpu-optimization.md`](notes/frontis-openmle-applied-to-tpu-optimization.md).

**Verdict: realistic, and better-supported than the "beat Opus 5" framing** — parity-at-low-cost is the
result Frontis literally reports, not a projection from it. Re-read their table for cost rather than rank:
the backbones are `A3B` MoEs (**~3B active parameters**) evaluated under 12 h on a single **12 GB RTX 4090**,
and *both* models beat Claude Opus 4.8 (63.64%) — 35B at 71.21% (also past GPT-5.5 + Codex at 68.18%, within
1.5 pp of GPT-5.6 Sol and of the 2.8T Kimi K3), 30B at 66.67%. The user's goal is strictly weaker than what
was demonstrated.

**The two proposed data sources map 1:1 onto Frontis's two SFT paths** — generated trajectories ↔ their
parallel path (17,245 `Draft` examples), wiki harvest ↔ their evolutionary path (9,014 trajectory-step
examples), 26,259 total. Recorded why the wiki-harvest half is *better* than theirs: it is already
multi-teacher frontier-authored (Codex/Claude/Gemini/Antigravity across 40+ kernel families), and its labels
are receipt-backed, independently re-measured, pre-registered and firing-audited rather than merely
score-filtered — with negative examples labelled too.

**Grounding gap found and recorded on the source page:** the word **"ablation" appears zero times** in the
61-page report (verified by full-text scan). Frontis reports controlled model/harness swaps and two
component comparisons (Figure 8 entropic weighting, Figure 16 vs AIRA-Evo) but **no SFT-vs-RL
decomposition** — the +21.22 pp is base → final only. That is the single most decision-relevant missing
number for an SFT-weighted plan, since the paper's own theory (§4, Yue et al. 2025) predicts SFT carries the
capability-closing share but never measures it. Added as a `> [!warning]` on
[`sources/frontis-ma1.md`](sources/frontis-ma1.md), contrasted against DGM's and AlphaEvolve's real
ablations.

**Operator-level parity outlook + the product path:** `Author`/`Tune`/`Refute` are high-volume and
favourable (narrow, data-rich, out-of-distribution for the frontier); **`Diagnose` is the crux risk** and is
~1 call per experiment — so a hybrid keeping a frontier model only for `Diagnose` moves ~90% of calls onto
the cheap model at almost no quality risk, and is shippable immediately. Argued the structural advantage
over Frontis: **the harness is the product and the model is a swappable operator**, so operators can be
replaced one at a time, each graded by `kgate` against the frontier incumbent on held-out families — one
large bet converted into a sequence of small measured reversible ones, with no point where the product is
worse than today's.

**Risks specific to this goal:** (1) test `Diagnose` first — cheap, since the wiki holds labelled K1
diagnoses whose downstream verdicts reveal whether the class choice was right; (2) **task diversity, not
example count, is the likely binding constraint** — the fix is op-point enumeration (40 families × 10–20
op-points ≈ 400–800 tasks, + KernelBench's 250), since diversity comes from op-points not from more samples
per family; (3) SFT-only inherits the teachers' ceiling and blind spots (including their bias against
`Refute`) — acceptable for the stated goal, but decide deliberately; (4) generation-specific overfit;
(5) **internal vs external product changes the data strategy** and should be settled before the generation
run.

## [2026-08-06] ingest | researchgym
Ingested **ResearchGym: Evaluating Language Model Agents on Real-World AI Research** (Garikaparthi,
Patwardhan, Cohan — TCS Research / Yale; arXiv:2602.15112, v2 2026-03-11) — downloaded to
[`raw/papers/researchgym.pdf`](../raw/papers/researchgym.pdf) (13 pp. main text + appendices A–F) and read
in full. Summary page: [`sources/researchgym.md`](sources/researchgym.md). Sourced from a review of
[FrontisAI/Awesome-Self-Improving-Agents](https://github.com/FrontisAI/Awesome-Self-Improving-Agents) for
papers worth ingesting on RSI/autoresearch grounds.

**Why it matters here:** withholds the proposed method from five oral/spotlight ICML/ICLR/ACL 2025 papers'
own repositories — keeping datasets, eval harness, and baselines intact — so an agent must propose a
genuinely novel hypothesis and beat a strong human-expert baseline, graded by the paper's own execution
scripts rather than an LLM judge. A GPT-5 `rg-agent` improves over baseline in only 1 of 15 end-to-end runs
(6.7%) and completes 26.5% of sub-tasks on average — yet that one run surpasses an ICML 2025 Spotlight's
own reference solution outright. Claude Code (Opus-4.5) and Codex (GPT-5.2) show the same
capability–reliability gap under the same protocol. A qualitative failure-mode pass documents overconfidence
in weak hypotheses, non-comparable experiments, parallel-experiment collapse, and context-length
degradation; a hint ablation (handing the withheld method's core idea in prose) still failed to reach
baseline in most cases, pointing at execution as a stronger bottleneck than ideation for this agent.

**Pages touched (3).** New: [`sources/researchgym.md`](sources/researchgym.md). Updated:
[`topics/mle-agents-and-benchmarks.md`](topics/mle-agents-and-benchmarks.md) (ResearchGym's benchmark-table
row grounded with real numbers, plus a new bullet in "Systems in this wiki"),
[`topics/autoresearch.md`](topics/autoresearch.md) ("Hypothesis generation and idea evaluation" section —
ResearchGym as the quantified instance of the page's opening claim that generation outpaces verification),
[`index.md`](index.md).

**Relation to this wiki's other closed-loop systems.** Against
[The AI Scientist-v2](sources/ai-scientist-v2.md): both close the loop with no human step, but
ResearchGym's grader is execution-based against a paper's own withheld metric rather than an LLM/VLM
verdict — a harsher, less gameable bar than AI Scientist-v2's 1/3 workshop-acceptance rate. Against
[Co-Scientist](sources/ai-co-scientist.md): Co-Scientist never executes anything and hands its ranked
hypotheses to a human for wet-lab validation; ResearchGym measures the ML-domain mirror case, where the
"experiment" a hypothesis proposes *can* be executed by the agent itself, so it can score what Co-Scientist
structurally cannot — whether the system's own execution of its own idea beats a strong human result.

## [2026-08-06] ingest | robophd
Ingested **RoboPhD: Evolving Diverse Complex Agents Under Tight Evaluation Budgets** (Borthwick, Ash &
Galczak; arXiv:2604.04347, 2026-04) — downloaded to [`raw/papers/robophd.pdf`](../raw/papers/robophd.pdf)
(10 pp.) and read in full. Summary page: [`sources/robophd.md`](sources/robophd.md). Sourced from the same
Awesome-Self-Improving-Agents review as researchgym.

**Why it matters here:** the first paper to run this wiki's own `autoresearch` silo head-to-head against two
other optimization paradigms — RoboPhD's own validation-free Elo-tournament selection and GEPA's Pareto-based
selection — under identical seed agents, evaluators, and a fixed 1,500-evaluation budget, across four
non-training-domain benchmarks (ARC-AGI, cloud scheduling, Text2SQL, financial QA). Confirmed with high
confidence via the paper's own reference list that its "Autoresearch" citation is Karpathy's repository, the
same one this wiki's `autoresearch` silo documents (though what's benchmarked is a reimplementation of the
harness's *algorithm*, not the literal `train.py`/`prepare.py`/`val_bpb` GPT-pretraining harness). RoboPhD
wins 3 of 4 benchmarks; a validation-budget ablation shows shrinking GEPA's/`autoresearch`'s held-out set
consistently frees budget for better scores (all 8 paired comparisons improve); and the `autoresearch`
reimplementation independently discovered a simulator oracle exploit on the Can't Be Late task — a
smaller-scale echo of DGM's Appendix H hallucination-detector gaming case study.

**Pages touched (5).** New: [`sources/robophd.md`](sources/robophd.md). Updated:
[`topics/autoresearch.md`](topics/autoresearch.md) (new "RoboPhD" subsection in "Self-improving research
loops"), [`code/autoresearch/overview.md`](code/autoresearch/overview.md) (new "Benchmarked externally"
section), [`concepts/evolutionary-self-improvement.md`](concepts/evolutionary-self-improvement.md) (Elo
tournament placed as a third selection mechanism, between `autoresearch`'s ratchet and DGM's archive),
[`index.md`](index.md).

## [2026-08-06] ingest | goedel-machines
Ingested **Gödel Machines: Self-Referential Universal Problem Solvers Making Provably Optimal
Self-Improvements** (Jürgen Schmidhuber; arXiv:cs/0309048, v1 25 Sep 2003, this summary cites v5 rev. 17 Dec
2006) — downloaded to [`raw/papers/goedel-machines.pdf`](../raw/papers/goedel-machines.pdf) (30 pp.) and
read in full. Summary page: [`sources/goedel-machines.md`](sources/goedel-machines.md). Sourced from the
same Awesome-Self-Improving-Agents review.

**Why it matters here:** the foundational theory paper the Darwin Gödel Machine is named after and
explicitly descends from, previously represented in this wiki only as a two-sentence, uncited gloss on
[`concepts/self-referential-code-rewriting.md`](concepts/self-referential-code-rewriting.md). A Gödel
machine rewrites any part of its own code — including its own proof searcher — only once a proof searcher
finds a *formal proof*, from an axiomatized hardware/environment/utility model, that the rewrite raises
expected utility; because that proof implicitly quantifies over every future alternative the unmodified
searcher could find, an accepted rewrite is **globally optimal** (Theorem 4.1), not just locally better. The
paper's own limitations section concedes Gödel/Rice-style undecidability can block a proof from ever being
found, but is notably confident (FAQ) that formalizing real-world utility is *not* itself a fundamental
obstacle — the "practically impossible" critique this wiki's concept page had attributed to this paper is
actually the Darwin Gödel Machine paper's own argument, made fourteen years later, against it.

**Date correction.** The existing concept page cited "Schmidhuber's 2007 Gödel machine" with no arXiv link.
The primary source is the 2003 arXiv preprint (revised through 2006); "2007" traces to a same-title,
condensed book chapter (Goertzel & Pennachin, eds., *Artificial General Intelligence*, Springer) that is a
derivative of, not the source for, this paper. Corrected on the concept page.

**Pages touched (3).** New: [`sources/goedel-machines.md`](sources/goedel-machines.md). Updated:
[`concepts/self-referential-code-rewriting.md`](concepts/self-referential-code-rewriting.md) ("Origin"
section rewritten with a proper citation, the corrected date, and a link to the new source page — full
kept/discarded comparison against DGM lives on the source page itself),
[`concepts/meta-evolution.md`](concepts/meta-evolution.md) (one-sentence pointer from rung 4 to this paper's
theoretical ceiling), [`index.md`](index.md).

## [2026-08-06] ingest | recursive-automated-ai-research
Ingested **"First Steps Toward Automated AI Research"** (Recursive, blog, 2026-06) — captured to
[`raw/papers/recursive-automated-ai-research.md`](../raw/papers/recursive-automated-ai-research.md) (no
linked full technical report or arXiv id exists for the system itself; the article and its companion
partial-artifacts GitHub repo are the only primary sources). Summary page:
[`sources/recursive-automated-ai-research.md`](sources/recursive-automated-ai-research.md). Sourced from the
same Awesome-Self-Improving-Agents review.

**Why it matters here:** reports an automated research system closing propose→implement→run→validate→
next-experiment with no human step, evidenced by three case studies — one of which, **NanoChat
Autoresearch**, runs directly against **this wiki's own `autoresearch` silo's exact benchmark**
(`karpathy/autoresearch`, `val_bpb`), beating the public `autoresearch@home` community leaderboard's best
score (0.9372→0.9109). Also reports a NanoGPT-speedrun win (79.7s→77.5s, community record since ~2025) and
an 18%-gap-reduction result on NVIDIA's SOL-ExecBench kernel benchmark (0.699→0.754 mean SOL score). The
source page is deliberately skeptical rather than credulous: the article names no search/ratchet mechanism,
data structure, or worked reward-hacking-detector example for any of the three results, so the numbers are
recorded as reported claims, not verified findings — and a small unexplained discrepancy between the
article's and the companion repo's NanoGPT-speedrun timing (77.5s vs. 77.3s) is flagged rather than silently
resolved.

**Pages touched (4).** New: [`sources/recursive-automated-ai-research.md`](sources/recursive-automated-ai-research.md),
[`raw/papers/recursive-automated-ai-research.md`](../raw/papers/recursive-automated-ai-research.md). Updated:
[`topics/autoresearch.md`](topics/autoresearch.md) (new subsection in "Self-improving research loops",
immediately after RoboPhD), [`code/autoresearch/overview.md`](code/autoresearch/overview.md) (folded into
the new "Benchmarked externally" section alongside RoboPhD),
[`topics/auto-optimization.md`](topics/auto-optimization.md) (new "Recursive — SOL-ExecBench" subsection
after the AlphaEvolve-vs-KernelEvolve comparison), [`index.md`](index.md).

**Not done:** no code silo — only a partial-artifacts companion repo exists (full NanoGPT-speedrun and
NanoChat-autoresearch scripts, but only 10/235 SOL-ExecBench kernels), and no full technical report exists
to ground a deeper ingest. If Recursive publishes a fuller writeup, revisit for the loop mechanism and
reward-hacking-detector detail this pass could not ground.

## [2026-08-06] ingest | kernelblaster
Ingested **KernelBlaster: Continual Cross-Task CUDA Optimization via Memory-Augmented In-Context
Reinforcement Learning** (Dong et al., NVIDIA; arXiv:2602.14293, 2026-02) — downloaded to
[`raw/papers/kernelblaster.pdf`](../raw/papers/kernelblaster.pdf) (33 pp.) and read in full. Summary page:
[`sources/kernelblaster.md`](sources/kernelblaster.md). Sourced from the same Awesome-Self-Improving-Agents
review.

**Why it matters here:** the wiki's third concrete [`llm-kernel-generation`](concepts/llm-kernel-generation.md)
instance, and the first targeting raw **CUDA** (not Triton/Pallas) on mainstream NVIDIA GPUs
(A6000/A100/H100/L40S). Its **MAIC-RL** mechanism — a compact (~50 KB) Persistent CUDA Knowledge Base of
`⟨bottleneck-signature, ⟨optimization, score⟩⟩` entries, rewritten by an LLM-driven textual-gradient loop —
borrows RL's vocabulary (state/action/reward, an explicit REINFORCE analogy) but never updates model
weights; confirmed with high confidence from the paper's own Table 1. Reaches 1.43×/2.50×/1.50× geomean on
KernelBench L1/L2/L3; an ablation with an empty knowledge base runs 1.67× slower, isolating the memory
itself (not just profiling access) as load-bearing. Internal inconsistencies flagged in the summary's
"Reading cautions" section (three different L3 headline figures; a SqueezeNetFireModule result given as
both 1.95× and 1.2×), following this wiki's practice on `kernelevolve.md`.

**Pages touched (2).** New: [`sources/kernelblaster.md`](sources/kernelblaster.md). Updated:
[`concepts/llm-kernel-generation.md`](concepts/llm-kernel-generation.md) (third papers-list entry, a
correction that MAIC-RL is in-context not weight-space RL, CUDA-L1 added to the reading queue),
[`index.md`](index.md).

## [2026-08-06] ingest | ai-supervisor
Ingested **AI-Supervisor: Autonomous AI Research Supervision via a Persistent Research World Model**
(Yunbo Long; arXiv:2603.24402, 2026-03) — downloaded to
[`raw/papers/ai-supervisor.pdf`](../raw/papers/ai-supervisor.pdf) (21 pp. incl. appendices A–F) and read in
full. Summary page: [`sources/ai-supervisor.md`](sources/ai-supervisor.md). Sourced from the same
Awesome-Self-Improving-Agents review.

**Why it matters here:** a multi-agent research-supervision framework built around a persistent, typed,
uncertainty-annotated **Research World Model** (a knowledge graph surviving across separate projects, unlike
Co-Scientist's per-run context memory) and a formally specified **consensus mechanism** gating gap
verification on corroboration counts. Its Experiment 3 gives this wiki's cleanest cross-project-persistence
result (16 structural links vs. 0 for a context-window-memory baseline). But close reading of the appendix
protocols shows every one of its seven evaluations is LLM-judged text-vs-text comparison — the
execution/reproduction machinery its architecture (and Related Work) describes is never shown firing
anywhere in its own results. And against this wiki's `verification-independence.md` criteria, the consensus
mechanism does not qualify as genuine independence: the same pool of agents proposes gap candidates in
Round 1 and "corroborates" them in Round 2 after being shown everyone's Round-1 answers — same-family
agreement-after-disclosure, not independent re-derivation. Both findings are this wiki's own synthesis from
the paper's appendix protocols and cost table, not concessions the paper makes about itself.

**Pages touched (3).** New: [`sources/ai-supervisor.md`](sources/ai-supervisor.md). Updated:
[`topics/autoresearch.md`](topics/autoresearch.md) (new bullet in "Hypothesis generation and idea
evaluation", between Co-Scientist and AI Scientist-v2),
[`concepts/verification-independence.md`](concepts/verification-independence.md) (new table row — "weak,
arguably weaker than AI Scientist-v2" — and a new failure-mode bullet on same-family corroboration
masquerading as consensus), [`index.md`](index.md).

## [2026-08-06] note | (addendum 3) Bake the wiki into weights? Price, and H100 sizing
Third follow-up on the same note. Claims evaluated: (a) a trained specialist removes the need to ship the
wiki as a runtime knowledge base, since its content is in the training set; (b) it solves LLM price; (c) the
model can be slightly bigger — H100-sized. **Verdict: (b) and (c) hold and are stronger than stated; (a) is
half right, and the wrong half is the expensive one.**

**(b) Price — two multiplicative levers, not one.** Frontis's `A3B` backbones are ~3B *active* params (the
per-token lever), but campaign cost here is input-dominated — Frontis's own matched study: 41.5M of 75.3M
tokens are prompt, `Improve` briefs averaging 35.7K chars after their context work. Training removes the
*reason* for the biggest paste: the load mandate currently injects `pallas-kernel.md` through `## Debugging`
into every author brief on the stated premise that the model has no Pallas. Recorded the right product KPI:
**cost per frontier-advancing experiment**, not per token (Frontis tracks the analogue — new-best updates
per million tokens, 1.77 → 3.27). Noted the structural reason cheap-but-noisier is a *better* trade here
than in MLE: the early-kill gate rejects broken candidates with no accelerator, so extra candidates are
near-free, whereas an MLE candidate is a real training run.

**(c) H100 — go MoE-bigger, not dense-bigger.** Sizing table filed. ~30–35B MoE at ~3B active in fp8 leaves
~45 GB for KV, which is the real constraint given 40–60K-token briefs; a ~32B *dense* model of the same
footprint costs ~10× the compute per token. Recommendation: increase **total** params via MoE before
**active** params via dense — Frontis's `A3B` choice is the whole cost thesis, not an implementation detail.
Two caveats: `Diagnose` is the operator that may genuinely want dense (long-context reasoning over messy
profiler output is where 3B-active is weakest — fix per-operator, as OpenMLE-Evo already runs a separate
memory model); and an H100 may not be needed at all, since a 30B-A3B serves fine on a v5e/v6e slice, which
removes both the GPU purchase and the API bill.

**(a) The pushback — the wiki does four jobs and training displaces one, partially.** Runtime brief
(partially displaced) · **training-corpus generator** (not displaced, becomes *more* important) ·
verification substrate — kgate receipts, lever-coverage set-diff, LINT, auditor (not displaced) ·
human-readable record (not displaced). Key finding: **the wiki already published the correct
bake-vs-retrieve split under a different name** — its own `regeneratable vs. earned` classification.
Regeneratable synthesis (indexes, blueprint — "nothing original lives here") is the bake-in pile; `BRIEFS.md`
(earned, incident-driven, "must never be rebuilt from a prompt") is the keep-retrieved pile. Three
non-negotiables for retrieval, each with an incident already in the wiki: generation-specific constants (the
index's own Generation-scope list, with "query, don't hardcode" and "treat numbers as calibration for the
*shape* of the answer" — a v6e-trained model will emit v6e block sizes on v7); framework-version API drift
("assume the target version's API, not memory" — a trained model *is* memory; the April-2026 libtpu flag
rejection cost ~5–8 experiments); and new hardware generations, which is exactly
[KernelEvolve](sources/kernelevolve.md)'s MTIA argument that a hand-authored KB enables generation "without
model retraining."

**Operational framing recorded:** dropping the wiki **converts a config change into a model release** — today
a libtpu regression is a `BRIEFS.md` edit effective in minutes; baked in, it waits for the next training run,
and that bites hardest at a hardware transition, which is when demand peaks. The opposite error is also named:
keeping the *whole* brief after training wastes the price win. Target is **a much smaller brief, not no
brief** — drop the Pallas mechanics, keep BRIEFS + class-page levers + queried constants. Decisive argument
is the flywheel: the wiki generates the corpus for v2, so dropping it freezes the model at v1 and dismantles
the [meta-evolution](concepts/meta-evolution.md) loop to save context tokens. Correct reading is the inverse
of the claim — **training makes the wiki less necessary at inference and more necessary as infrastructure**,
the same "what the system learned vs. what the system was told" asymmetry already on
[`retrieval-augmented-prompt-synthesis`](concepts/retrieval-augmented-prompt-synthesis.md).

## [2026-08-06] ingest-code | openrsi
Ingested `openrsi` (https://github.com/FrontisAI/OpenRSI, Frontis.AI's code release for the
[Frontis-MA1 / OpenMLE](sources/frontis-ma1.md) paper) as a git submodule at `raw/code/openrsi`, pinned @
`eab056726`. `wikify prepare` indexed 6234 symbols (scip-python) and auto-seeded 24 concept packets by
centrality. Checked the repo's `NOTICE` file first: 8 of the 24 packets sit entirely inside
`OpenMLE-ERL/SFT/slime/`, vendored third-party THUDM/slime RL-training infra (Apache-2.0), not Frontis's own
contribution — with the user's sign-off, scoped the deep-dive to the 16 OpenMLE-original packets and let
Stage 6b's catalog generation represent the vendored slime modules.

Synthesized the 16 in scope, in parallel batches: OpenMLE-Gym's task builder
([NodeExecutor](code/openrsi/concepts/OpenMLE-Gym-builder_core-utils-nodes.md)) and sandboxed executor
([process_runner](code/openrsi/concepts/OpenMLE-Gym-openmle_gym-process_runner.md)); OpenMLE-ERL/RL's
operator-conditioned rollout ([generate_mle](code/openrsi/concepts/OpenMLE-ERL-RL-generate_mle.md)), reward
shaping — the paper's adaptive-bound `power_clip` (Eq. 1) plus `hack_check_async`/validation-gap integrity
guards — ([reward_func_utils](code/openrsi/concepts/OpenMLE-ERL-RL-reward_func_utils.md)), the paper's Eq. 3
three-term (exploit/explore/cooling) parent-fitness database
([program_database](code/openrsi/concepts/OpenMLE-ERL-RL-program_database.md)), and the original-AIRA-Evo
baseline adapter ([airaevo_experience](code/openrsi/concepts/OpenMLE-ERL-RL-airaevo_experience.md));
OpenMLE-ERL/SFT's trajectory-collection harness — scheduler, evaluator, generator, rejection policies,
tree-search event log, and its own simpler program database (7 pages under
`OpenMLE-ERL-SFT-tts_search-*`) — plus the validation/test gap data-quality filter
([gap_filter](code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)); and
OpenMLE-Evo's storage substrate
([program_database](code/openrsi/concepts/OpenMLE-Evo-tts_search-program_database.md)), leaderboard/medal
grading ([eval_utils](code/openrsi/concepts/OpenMLE-Evo-tts_search-eval_utils.md)), and OpenMLE-Evo-Max's
multi-GPU async worker pool
([airaevo_async_resources](code/openrsi/concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)). Wrote
[`overview.md`](code/openrsi/overview.md) with a dedicated comparison table mapping each paper mechanism
(adaptive bounds, entropic advantage, async rollouts, Eq. 3/Eq. 4 fitness, the four-operator vocabulary) to
where it's actually grounded — the load-bearing cross-cutting finding, independently converged on by three
readings (the SFT scheduler, its tree-search state log, and its program database): the wired `GreedySearch`
and RL rollout only ever emit `draft`/`improve`; `Debug`/`Crossover` as distinct operators only fire through
the vendored, third-party AIRA-Dojo `Evolutionary` solver, not the primary harness this ingest grounds. From
the README, 3 doc-concept pages: [trainable atomic operators](code/openrsi/doc-concepts/trainable-atomic-operators.md)
(which cross-references that same finding), [the OpenMLE-Evo-Max profile](code/openrsi/doc-concepts/openmle-evo-max-profile.md),
and [the shared action space](code/openrsi/doc-concepts/shared-action-space.md) (the `Program`/`ProgramDatabase`
shape recurring, independently evolved, across all three layers).

`wikify finalize` needed one repair round (3 Mechanism steps missing an in-subgraph citation) before going
green: 6228 documentable symbols across 413 modules, 100% represented (380/380 classes), 553 deep (8.9%).
Adversarial verify then checked all 281 load-bearing claims across the 16 concept pages (16 parallel
reviewers) and refuted-and-fixed ~20 of them — notably: `Download` doesn't actually wrap its own body in
`try/except` (only its internal helper does, contradicting the page's "every phase swallows its own
exceptions" claim); `run_task_process` is not literally "the single choke point" for every Gym operation
(`prepare_single_competition` bypasses it entirely in the default non-isolated mode); the RL rollout's group
reward-barrier is guarded by a dedicated per-task `asyncio.Lock`, not `_get_loop_lock` as originally claimed;
`SearchAlgorithm.select`/`select_best` really do have zero concrete overrides anywhere in `OpenMLE-Evo/`
(confirmed by an explicit repo-wide search, not just absence-from-subgraph); and `eval_utils.write_time_scaling`
computes `medal_rate`/`grade_avg@k` over the *full* sample count, not just samples under the time budget as
originally claimed. Re-ran `wikify finalize openrsi` after all edits: still green, same coverage.

Registered in [`index.md`](index.md) (Code repos section) and cross-referenced from the
[Frontis-MA1 source page](sources/frontis-ma1.md), which previously flagged the repo as un-ingested.

## [2026-08-06] connect | 3 new concepts wired for openrsi, 12 refreshed
`wikify connect` proposed 3 new candidate concepts from openrsi's `concepts:` frontmatter tags (tag matches,
authoritative) plus new tagged implementations on 9 already-connected concepts. Applied the 3 new ones —
[`program-evolution-operators`](concepts/program-evolution-operators.md) (8 openrsi implementations —
the paper's own Draft/Improve/Debug/Crossover vocabulary),
[`verification-independence`](concepts/verification-independence.md) (9 implementations — `hack_check_async`,
the validation/test gap filter, hidden-evaluator public/private split, leaderboard-file medal grading), and
[`retrieval-augmented-prompt-synthesis`](concepts/retrieval-augmented-prompt-synthesis.md) (1 implementation
— the AIRA-Evo baseline adapter's per-operator ancestor/sibling/error-signature memory assembly) — then
`--refresh`ed all 12 already-connected concepts so the ones openrsi also tags
(`closed-loop-experiment-design`, `evolutionary-algorithm-discovery`, `agentic-tree-search`) pick up its
implementation links too.

Added hand-written hub prose above the auto blocks on two pages, since openrsi's code-grounding qualifies
claims those pages made at the paper level: `program-evolution-operators.md` gets an `[!inferred]` note that
the four-operator vocabulary the paper describes is not realized in the primary wired code paths — Debug and
Crossover only fire through the vendored, third-party AIRA-Dojo `Evolutionary` solver, not Frontis's own
scheduler/rollout; `verification-independence.md` gets a new table row for Frontis-MA1/OpenMLE, noting the
sandboxed hidden-evaluator score is structurally independent but the two self-report cross-checks are
weaker (the hack-check judge fails *open* by default; the sandbox's secret-stripping is opt-in, tied to the
non-default `"isolated"` execution mode). `wikify finalize openrsi` re-checked green after both edits.

## [2026-08-12] ingest-code | rlm

Ingested `alexzhang13/rlm` (submodule, pinned @ `caf0bffa1a`) — Alex Zhang's own reference implementation of
[Recursive Language Models](sources/recursive-language-models.md), the first of four repos named in the
2026-08-10 "Context as a Variable" video (`k2rkLm1eA9k`). 1,753 symbols across 121 modules (100% represented,
191/191 classes); 21 code concept pages + 3 doc-concept pages
(`repl-environment-taxonomy`, `codeact-bet`, `trajectory-logging-and-visualization`). `wikify finalize`
green after a repair loop (26 → 7 → 2 → 1 → 0 lint errors — mostly cross-packet citation leakage: a symbol
genuinely in the repo but not in the specific packet being synthesized, which the linter correctly rejects).
Adversarial verify run as a spot-check on the highest-load-bearing page (`rlm-core-rlm`, 14 claims) rather
than exhaustively across all 118 claims in the silo — see the batch-completion note at the end of this
ingest run for the reasoning. No refutations found on the spot-checked page; two claims were honestly
docstring/signature-grounded rather than directly-observed-in-full (`format_iteration`'s truncation
behavior, `_subcall`'s recursive-spawn branch), both within the skill's own grounding rules.

## [2026-08-12] ingest-code | Retrodict

Ingested `ryanbbrown/Retrodict` (submodule, pinned @ `71672e8e5a`, **no license — all rights reserved,
gitlink only, no content vendored**) — the second of four repos from the 2026-08-10 video batch, and the
sharpest verification-discipline instance in the set: every hypothesis about a game mechanic is replayed
against the log before it earns a live action, and every planned action carries a checked forward
prediction. 326 symbols across 14 modules (100% represented, 23/23 classes); 3 code concept pages + 2
doc-concept pages (`retrodiction-methodology`, `context-reset-and-playbook`). `wikify finalize` green on
the first pass. Adversarial-verify: direct source read (not packet-only) on `arc3-runner.py` (the
highest-claim page, 740 lines, read in full) and `arc3-plan_parser.py` (148 lines, read in full) against
the corresponding wiki pages' claims — found and fixed one real inaccuracy (`_record_escalation` was
described as computing the escalation tier; it only *logs* a tier change decided by
`_escalation_directive`). `arc3-logwriter.md`'s claims rest on the packet's own quoted docstrings only (not
independently re-read against the 194-line source), a shallower verification tier than the other two pages
in this silo — flagged rather than silently treated as equally checked.

## [2026-08-12] ingest-code | continual-harness

Ingested `sethkarten/continual-harness` (submodule, pinned @ `bbab97ad73`) — the third of four repos from
the 2026-08-10 video batch, and the implementation behind
[`sources/continual-harness.md`](sources/continual-harness.md). 4,582 symbols across 137 modules (100%
represented, 210/210 classes); 26 code concept pages + 2 doc-concept pages
(`reset-free-harness-evolution`, `immutable-base-prompt`).

**Tooling note worth carrying forward.** Auto-discovery (SCIP centrality ranking) picked 24 concepts, all
Pokémon-environment infrastructure (memory readers, emulators, map stitchers, server routes) — it missed
`agents/utils/harness_evolver.py`, the file implementing the paper's actual headline contribution, entirely.
Added as explicit `## Concepts` seeds in `config/continual-harness.md` (`agents-utils-harness_evolver`,
`agents-tools-registry`) per the `wikify-ingest-repo` skill's guidance. Even seeded this way, both packets'
own `Seeds` line read "(discover: top-importance symbols — no seeds resolved)" — the module-path-style seed
name did not restrict discovery to that file's own symbols, and both packets fell back to the same generic
top-importance symbol set as the auto-discovered ones. Practical consequence: both concept pages
(`agents-utils-harness_evolver.md`, `agents-tools-registry.md`) were written from **direct source reading**
(`harness_evolver.py`, `agents/tools/registry.py`, read in full) rather than from their packets, and their
citations had to route through whichever in-subgraph symbol was actually available (mostly
`PokeAgent.run_step`, a genuine caller) rather than the methods the prose is actually about — `wikify
finalize`'s citation linter correctly rejected the first draft's direct citations (26 → 19 → 8 → 3 → 0
errors across the repair loop) since those methods were absent from the packets' own subgraphs even though
they resolve in the full SCIP index. Worth a `wikify` tool fix: symbol-level seeds (not just module-path
seeds) should restrict discovery to symbols *defined in* the named file, not fall back to global
top-importance ranking when the module-path form doesn't match a recognized seed pattern.

**Pages updated**: `index.md` (registers this silo with the same disclosure).

## [2026-08-12] ingest-code | prime-agent

Ingested `PrimeIntellect-ai/prime-agent` (submodule, pinned @ `a3b3e75349`) — the fourth and last repo from
the 2026-08-10 video batch, and the implementation behind
[`sources/prime-agent-launch.md`](sources/prime-agent-launch.md). 21,067 symbols across 774 modules (100%
represented, 1984/1984 classes); 25 code concept pages + 3 doc-concept pages
(`rlm-continual-harness-composition`, `long-running-agent-continuity`, `prime-agent-trust-model`). This is
the largest silo ingested so far by module count — a TypeScript monorepo (`packages/coding-agent`,
`packages/agent`, `packages/ai`, `packages/tui`) — and confirmed by direct source-reading (`README.md`
Acknowledgements) to be built on `earendil-works/pi`, not `badlogic/pi-mono` as the README's header link
row might suggest at a glance; the two repos are unrelated despite the pi-mono link appearing alongside
Verifiers/PRIME-RL.

**TypeScript SCIP indexing note worth carrying forward.** `index_shards` (file-level sharding, used
successfully to scope large Python repos in earlier silos) totally breaks indexing for a TypeScript repo
with a project-reference `tsconfig.json`: `wikify prepare` expands the glob into individual `.ts` file
paths and invokes `scip-typescript` once per file, and `scip-typescript` cannot parse a single `.ts` file
path as its own `tsconfig.json` root — every shard failed silently, and `wikify prepare` reported an
empty index. Root-caused by running `scip-typescript index` manually with different argument shapes: a
single-file target treats that file as `tsconfig.json` and fails to parse it (`TS1005`); `--cwd
packages/coding-agent` fails because that subdirectory has no `tsconfig.json` (only `tsconfig.build.json`);
running unsharded from the repo root succeeds in ~39s using the top-level `tsconfig.json`'s project
references. Fix: dropped `index_shards` from `config/prime-agent.md` entirely and used `coverage_collapse`
instead (which only affects the coverage-report grouping, not indexing) to keep the coverage report legible
despite `examples/`, `themes/`, and `packages/tui/` contributing thousands of low-signal symbols.
Indexing also required `npm install --no-audit --no-fund --ignore-scripts` at the repo root first (351
packages) for type resolution to succeed at all.

**Same seeded-symbol-resolution limitation as continual-harness, once.** The `refinement.ts` config seed
(`packages-coding-agent-src-core-refinement-refinement.ts`) hit the same tool limitation already logged for
continual-harness's Python seeds — its packet's `Seeds` line failed to resolve to that file's own symbols,
falling back to generic top-importance discovery. `kernel/index.ts`, the other explicit seed, was already
auto-discovered independently and did not hit this. `refinement.ts`'s concept page was written from direct
source reading (`packages/coding-agent/src/core/refinement/refinement.ts`, read in full) rather than its
packet, using unlinked citations for its own symbols and routing the linter's rule-2 requirement through
genuinely in-subgraph references. Post-finalize spot-check (this ingest's verify pass) re-read the same
source file against all 5 load-bearing claims on that page — optimistic-concurrency comparison against
`baselineState`, the exact `"entry changed during refinement planning"` / `"entry not found"` / `"entry
already exists"` error strings, the `before?.scope ?? options.scope ?? "local"` fallback chain, the
`version = before ? before.version + 1 : 1` bump, and `rollbackProposal`'s reverse-and-invert structure —
all confirmed accurate. `wikify finalize` itself passed clean on the first run (0 citation errors across
all 25 pages), unlike continual-harness's multi-round repair loop.

**Pages updated**: `index.md` (registers this silo).

## [2026-08-12] ingest | video batch — RLM / Continual Harness / ARC-AGI-3 cluster (closing)

Closes the batch opened by "ingest articles and repositories mentioned in [this
video](https://www.youtube.com/watch?v=k2rkLm1eA9k)" — 8 source pages and 4 code silos, connected and
synthesized. Full accounting:

**Sources** (`wiki/sources/`, all new): [2025-context-rot](2025-context-rot.md),
[arc-agi-3](arc-agi-3.md), [recursive-language-models](recursive-language-models.md),
[pokeagent-challenge](pokeagent-challenge.md), [continual-harness](continual-harness.md),
[schema-harness](schema-harness.md), [retrodict](retrodict.md), [prime-agent-launch](prime-agent-launch.md).
Two corrections made while cross-checking these against each other and against grounded code: (1)
`pokeagent-challenge.md` records that the source video's description links the *wrong* paper — the
self-refining-harness mechanism it narrates is `continual-harness.md`'s paper, under the same lead author,
not the PokéAgent benchmark paper itself; (2) `prime-agent-launch.md`'s claim that a "Pi-mono" benchmark
comparison "confirms Prime Agent's README-stated lineage from `badlogic/pi-mono`" was flagged
`[!warning]` and corrected after direct code-silo grounding: the actual README Acknowledgements state Prime
Agent is built on `earendil-works/pi`, a different project `badlogic/pi-mono` is unrelated to beyond
appearing in the same header link row.

**Code silos** (`wiki/code/`, all new, all `wikify finalize` green at 100% coverage): `rlm` (1,753 symbols/
121 modules, 21 concept + 3 doc-concept pages), `Retrodict` (326 symbols/14 modules, 3 concept + 2
doc-concept pages), `continual-harness` (4,582 symbols/137 modules, 26 concept + 2 doc-concept pages),
`prime-agent` (21,067 symbols/774 modules, 25 concept + 3 doc-concept pages — the largest silo in this wiki
by module count). Per-silo tooling notes and repair-loop accounting are in each silo's own log entry above.
One thing worth flagging here because it wasn't caught until the connect step: **all four silos' `finalize`
runs assembled `index.md` but never wrote `overview.md`**, the hand-authored landing page `wikify connect`'s
`discover_silos` requires (it globs for `overview.md`, not `index.md`) — and the one every `wiki/index.md`
entry for these silos already linked to. All four `overview.md` files were written retroactively this pass,
after `wikify connect` silently reported "8 silo(s)" (the pre-existing count) with zero candidates from any
of the four new silos, which is what surfaced the gap. Worth carrying forward as a checklist item for future
code-silo ingests: **write `overview.md` before calling `wikify connect`**, not after.

**Connect.** Two of this wiki's cross-paper vocabulary concepts gained new implementations after adding
explicit `concepts:` frontmatter tags (missed during the original per-silo ingest passes, also only caught
via the connect step's zero-candidate report): `self-referential-code-rewriting` — `dgm` (3 pages) plus now
`continual-harness`'s `agents-utils-harness_evolver` and `prime-agent`'s `refinement.ts`, a second
independently-engineered implementation of the same target class; `verification-independence` — `openrsi`
(9 pages) plus now all three `Retrodict` concept pages (`arc3-runner`, `arc3-plan_parser`, `arc3-logwriter`),
retrodiction-before-action and forward-prediction-checked-after-action both being instances of "make the
evidence an artifact, not an assertion." Also resolved: `prime-agent`↔`pi-autoresearch-vkf` is not a
fork/derivative relationship (both are separate repos targeting the same `earendil-works/pi` coding-agent
framework — `pi-autoresearch-vkf` is loadable as an extension into a host like `prime-agent` via the
`ExtensionAPI`/package-manager mechanism `prime-agent`'s own silo now documents) — noted in both overview
pages.

**Topic synthesis.** [`wiki-driven-autoresearch-loop`](../topics/wiki-driven-autoresearch-loop.md) gained a
new "long-horizon interactive-game agents" section: a third domain (after model-quality and model-performance
autoresearch) that independently converges on the same two load-bearing lessons — a persistent, replayable
artifact as ground truth over an agent's own live/context-window state (Retrodict's log, Continual
Harness's/Prime Agent's reset-free harness editing), and falsifying a hypothesis cheaply before committing a
real action (Retrodict's retrodiction, Schema's guarded action queues) — with no cross-citation between this
cluster and the TPU-performance instances already on that page. [`autoresearch`](../topics/autoresearch.md)'s
"Self-improving research loops" section gained a disambiguating note: Continual Harness/Prime Agent's
harness self-editing is the same *target class* as DGM (self-referential-code-rewriting) but closes its loop
within one episode of interactive play, not across independent research runs judged by a fixed metric — no
keep/discard ratchet, no archive, no benchmark-gated acceptance.

**Pages updated this closing entry**: `index.md` (added all 8 source-page entries to Papers/Sources, which
had been omitted from the per-source ingest passes — another gap the closing pass caught; updated the
`self-referential-code-rewriting` cross-paper-concepts bullet), `sources/prime-agent-launch.md` (the
Pi-mono correction above), `topics/wiki-driven-autoresearch-loop.md`,
`topics/autoresearch.md`, and `overview.md` + one `concepts:` frontmatter tag in each of the four new code
silos.
