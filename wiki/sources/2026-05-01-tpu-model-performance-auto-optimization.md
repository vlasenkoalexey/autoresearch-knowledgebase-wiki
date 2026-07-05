# TPU Model Performance Auto-optimization (blog, 2026-05-01)

The author's own introduction to [tpu_performance_autoresearch_wiki](tpu-performance-autoresearch-wiki.md),
stating the four ingredients the project claims are sufficient for an autonomous agent to drive any
`(model, hardware)` pair to state-of-the-art performance, and reporting the first real case-study results.

## Overview
The post frames the four components as exactly what a new human hire would also need to optimize a model
they'd never seen: **tools** (a profiler), a **knowledge base** (TPU optimization know-how), a **codebase**
to work on, and, as a bonus, a **reference-optimized codebase** to compare against
([raw](../../raw/papers/2026-05-01-tpu-model-performance-auto-optimization.md)). It positions the work
against Anthropic's [recursive self-improvement](https://www.anthropic.com/institute/recursive-self-improvement)
piece — the claim there is about agents eventually building/training models themselves; this post's claim
is narrower and already demonstrated: for *model performance optimization* specifically, autonomous
agent-driven optimization already works, at least partially.

## Key claims

1. **Autoresearch generalizes past "optimize for loss."** [Karpathy's autoresearch](../code/autoresearch/overview.md)
   loop — propose ranked hypotheses, run experiments, evaluate, revise priors — is domain-agnostic; the
   post repurposes it to optimize **TPS** (tokens/sec) and **MFU** (Model FLOPs Utilization) instead of
   validation loss.
2. **Performance optimization is more measurable than quality optimization.** Unlike convergence — which
   improves for reasons that are often hard to predict — performance is "highly predictable and
   measurable," which is why a profiler-as-observer works so well here specifically.
3. **XProf-as-MCP is the bridge that makes profiling agent-usable.** XProf itself is a human-facing tool;
   wrapping it as an MCP server ([xprof-mcp](https://github.com/vlasenkoalexey/xprof-mcp)) gives the agent
   programmatic access to bucket-level attribution *and* to HLO dumps (both optimized and original HLO),
   letting it trace a profile finding back to the exact line of model code that produced it.
4. **The wiki is a lighter-weight alternative to RAG for this domain**, not just a convenience — contrasted
   explicitly against [MaxCode/MaxKernel](https://github.com/AI-Hypercomputer/accelerator-agents), which
   solve the same "give the LLM TPU-specific knowledge" problem via a vector-database RAG pipeline. The
   wiki claims comparable payoff (the agent doesn't need to rediscover known Pallas kernels) with far less
   infrastructure.
5. **Write access to the model code is what distinguishes this from "LLM as smart reader."** The agent
   edits real code on real per-experiment branches — auditable, revertible, tied back to the experiment
   page, the profile, and the verdict that accepted or rejected it.
6. **A reference-optimized codebase narrows search dramatically.** Ingesting a fast reference (MaxText,
   MaxDiffusion, vLLM, SGLang) reframes the problem from "explore the space of optimizations" to "explain
   why the reference is fast and close the gap" — many "what next" decisions collapse into "do what the
   reference already does, and measure."

## Key data points

**Llama 3 8B case study (single harness, Claude Code + Opus 4.7, TPU v6e-8):**

| Stack | tok/s/chip | MFU | vs MaxText |
|---|---:|---:|---:|
| JAX (Flax NNX) | ~7,700 (peak 7,768) | ~43.3% (peak 43.6%) | +8.9% (peak +9.9%) |
| MaxText reference | 7,069 | 44.6% non-causal / ≈39.6% causal-adjusted | — (anchor) |
| torchax (PyTorch-on-JAX) | 6,559 | 36.8% | −7.2% |
| torchax (baseline) | 4,591 | 22.9% @ seq=1024 | — |

The model was built from scratch by the agent in two stages: convert HuggingFace Llama 3 to torchax and
optimize (~70 iterations), then rewrite in JAX from a local maximum and optimize again (~70 iterations).
The agent reached state-of-the-art for this model over a single weekend, unattended.

**Qwen3 8B case study (four agent + harness stacks, same TPU v6e-8, no steering beyond pointing at
MaxText as a reference):**

| Agent + harness | Best MFU @ seq 8192 | vs MaxText |
|---|---:|---:|
| Codex (GPT-5.5) | 43.2% | +8.5% |
| Claude Code (Fable 5) | 39.9% | +0.3% |
| MaxText reference (causal-adjusted) | 39.8% | — (anchor) |
| Claude Code (Opus 4.8) | 34.8% | −12.6% |
| Antigravity (Gemini 3.1 pro) | 30.6% | −23.1% |

Two of four harnesses autonomously beat the optimized MaxText reference. The author's read: Codex won
mainly because it kept pushing more experiments rather than declaring the search exhausted — the spread
between harnesses is itself a measurement of agent persistence, not just capability.

## Gaps & caveats
- At time of writing, the loop only worked reliably on Claude Code — Codex and Gemini CLI struggled to
  follow it (later addressed; see
  [Making TPU auto-optimization work with other agents](2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md)).
- The author had to babysit the loop — it stopped often, claiming exhaustion (later addressed; see
  [Making Karpathy's autoresearch production-ready](2026-06-05-making-karpathy-autoresearch-production-ready.md)).
- Auto-optimization "doesn't work as well for more complex models yet."

## Connections
- [karpathy/autoresearch — overview](../code/autoresearch/overview.md) — the seed loop this post specializes.
- [tpu_performance_autoresearch_wiki — methodology summary](tpu-performance-autoresearch-wiki.md) — the
  repo this post introduces.
- [Wiki-driven autoresearch loop](../topics/wiki-driven-autoresearch-loop.md) — synthesis topic page.

## Sources
- [`raw/papers/2026-05-01-tpu-model-performance-auto-optimization.md`](../../raw/papers/2026-05-01-tpu-model-performance-auto-optimization.md)
- Original: https://vlasenkoalexey.github.io (post dated 2026-05-01)
