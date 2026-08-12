# Recursive Language Models

Alex L. Zhang, Tim Kraska, Omar Khattab (MIT CSAIL) — [arXiv:2512.24601](https://arxiv.org/abs/2512.24601),
v1 2025-12-31, v3 2026-05-11, **published to no conference**. The paradigm this whole ingest batch turns
on: instead of pasting a long input into a model's context window, store it as a variable in a live Python
REPL and let the model **write code against a handle to it** — including code that recursively calls
itself (or a cheaper sub-model) over slices of that variable. Ingested 2026-08-12 alongside
[Prime Agent](prime-agent-launch.md), the product built on this idea plus
[Continual Harness](continual-harness.md).

## Overview

An RLM initializes with the long prompt bound to a variable in a persistent REPL; the root model receives
only metadata about it (length, a short prefix, access methods) — never the content itself. It generates
Python that inspects, filters, and decomposes that variable, and can invoke `rlm.completion(...)` as an
ordinary function call — a sub-RLM with its own empty context — over any slice. Only bounded-size stdout
(a prefix + length) returns to the root model's own history, so the root's context stays small regardless
of input size; recursion terminates when the model sets a designated `Final` variable. The paper frames
this explicitly as a bet against JSON tool-calling and for CodeAct-style code environments, with
sub-model calls and long inputs both treated as *objects in code* rather than *tokens in a prompt*.

## Key claims

- **The premise is [Chroma's context-rot finding](2025-context-rot.md), cited directly**: quality
  degrades well before a window fills, so the fix is not a bigger window but keeping the long input out of
  the window in the first place.
- **On OOLONG (131K-token linear-aggregation benchmark), RLM(GPT-5, depth=1) scores 56.0 against a 44.0
  base-GPT-5 baseline** — a 12-point gap the paper itself states as **+28.4% relative** (Qwen3-Coder-480B:
  48.0 vs. 36.0 base, **+33.3%** relative). On the quadratic-complexity OOLONG-Pairs variant, both base
  models score ≤0.1 F1 while their depth=1 RLM counterparts reach 58.0 (GPT-5) and 23.1 (Qwen3-Coder) —
  the paper's clearest case for recursion mattering, not just context-offloading.
- **Depth=0 (context-as-variable, no recursive sub-calls) already captures most of the win on some
  tasks**; recursive sub-calling adds the rest specifically on information-dense tasks (OOLONG,
  OOLONG-Pairs), where the paper reports the no-sub-call ablation falls back to keyword heuristics instead
  of the semantic transformation recursion enables. This is the paper's stated Observation 2.
- **On BrowseComp-Plus (6M–11M input tokens)**, RLM(GPT-5, depth=1) reaches 91.3% against a compaction
  baseline's 70.5% and a 0% base-model score (the base model exceeds its context window outright), at an
  average cost of $0.99/query versus a linearly-extrapolated $1.50–$2.75 for feeding that much text to
  GPT-5-mini directly.
- **Depth generally helps but with diminishing and sometimes negative returns**: on OOLONG-Pairs, GPT-5
  RLM improves monotonically from depth=0 (43.9) through depth=3 (76.0); on Qwen3-Coder's OOLONG run,
  depth=1 (48.0) beats depth=2 (26.0) and depth=3 (32.0) — the paper does not claim depth is a free lever.
- **A fine-tuned 8B model narrows most of the gap to a much larger one.** RLM-Qwen3-8B — Qwen3-8B
  fine-tuned on 1,000 filtered RLM(Qwen3-Coder-480B) trajectories from an unrelated task set — beats its
  own un-tuned base by a **median of 28.3%** across four evaluation tasks and, on three of them,
  approaches vanilla GPT-5's score, while running >3× faster than the larger teacher.
- **The Claude Code comparison the video cites is real but asymmetric on cost.** Table 1 reports Claude
  Code (Claude Opus 4.1, context-offloading variant) scoring competitively on several tasks (e.g. 84.0 on
  BrowseComp-Plus) but at far higher per-query cost than the RLM rows on the same tasks — the paper's own
  average-cost columns put several Claude Code cells multiple dollars per query above the corresponding
  RLM row.

## Key data points

| Benchmark (task length) | Base model | RLM (depth=1) | Gap |
|---|--:|--:|---|
| OOLONG (131K), GPT-5 root | 44.0 | 56.0 | +12 pts (paper states +28.4% relative) |
| OOLONG (131K), Qwen3-Coder-480B | 36.0 | 48.0 | +12 pts (paper states +33.3% relative) |
| OOLONG-Pairs (32K), GPT-5 root | 0.1 F1 | 58.0 F1 | — |
| BrowseComp-Plus (6–11M), GPT-5 root | 0.0 (context-limit) | 91.3 | — |
| RLM-Qwen3-8B vs. its own un-tuned base | — | +28.3% median (4 tasks) | approaches vanilla GPT-5 on 3/4 |

## Techniques referenced
REPL-mediated context offloading; `Final`-variable-gated recursion termination; recursion-depth ablation
(0–3); rejection fine-tuning on distilled RLM trajectories; RLVR length generalization on MRCRv2.

## Gaps & caveats
- **The video's "34 points at 132K tokens / 15 points at 263K"** framing does not match Table 1's
  directly-stated OOLONG numbers verified above (a 12-point / 28.4%-relative gap at 131K, stated in text).
  The paper's Figure 1 does plot a growing GPT-5-vs-RLM gap as context length increases on a log scale, and
  a reader could plausibly read larger point-gaps off that chart at specific lengths — but I could not
  independently confirm 34 and 15 as the paper's own stated values at exactly those two lengths from the
  extracted text, so this ingest cites only the table-stated numbers above and flags the video's figures as
  unverified.
- **This is a preprint with no peer review, revised twice and still unpublished to any venue** as of the
  version ingested. Treat headline percentages as the authors' own reported numbers, not an independently
  refereed result.
- The paper's own honest caveat: RLM cost can spike on trajectories where the model "struggles to find an
  answer" — average cost, not median cost, is where RLM sometimes loses its cost advantage over baselines.
- **Provenance**: the idea originates in an October 2025 blog post by Zhang, then a first-year MIT PhD
  student about six weeks into the program — the same "give a model task A, give it task B, give it both
  and it does worse than either alone" framing this paper formalizes. By the last day of 2025 that post was
  an arXiv preprint with his two co-authors (his advisors); it was independently developed into a product
  ([Prime Agent](prime-agent-launch.md)) by Prime Intellect over the following months, and Zhang is now a
  research fellow there.

## Connections
- [Context Rot (Chroma, 2025)](2025-context-rot.md) — the measured problem this paper's design responds to.
- [Prime Agent launch post](prime-agent-launch.md) — the shipped product implementing RLM (context as a
  variable, `rlm(...)` subagent calls) as one of its two core abstractions.
- [Continual Harness](continual-harness.md) — the other core abstraction Prime Agent is built on; a
  distinct paper about *rewriting the harness itself* rather than about context handling.
- [`concepts/evolutionary-algorithm-discovery.md`](../concepts/evolutionary-algorithm-discovery.md) — a
  different but related move in this wiki's vocabulary: RLM keeps the *model* fixed and changes what enters
  its context programmatically; the evolutionary systems keep the harness fixed and evolve the *artifact*.
  Both replace "paste everything into one call" with "structure the search over what one call sees."

## Sources
- [Recursive Language Models](https://arxiv.org/abs/2512.24601), Zhang, Kraska, Khattab — arXiv:2512.24601, v3 2026-05-11
- [alexzhang13.github.io/blog/2025/rlm/](https://alexzhang13.github.io/blog/2025/rlm/) — the October 2025
  origin post
- Code: [alexzhang13/rlm](https://github.com/alexzhang13/rlm) (see the code-silo ingest at
  [`code/rlm/overview.md`](../code/rlm/overview.md) once grounded)
