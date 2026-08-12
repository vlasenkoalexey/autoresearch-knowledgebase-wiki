# The PokéAgent Challenge

Seth Karten et al. (31 authors, Princeton-led; NeurIPS 2025 Competition Track) —
[arXiv:2603.15563](https://arxiv.org/abs/2603.15563). A competitive-benchmark paper, not a system paper —
the predecessor this wiki ingests specifically because the reference framework it shipped later grew,
under the same lead author, into [Continual Harness](continual-harness.md). Ingested 2026-08-12 to record
that lineage accurately: the video's description links *this* paper while narrating the harness paper it
became.

## Overview

PokéAgent uses Pokémon's battle system and RPG world as a testbed combining three properties the authors
argue no existing benchmark suite captures simultaneously: **partial observability** (an opponent's team
and item choices are hidden), **game-theoretic reasoning** (competitive battling is adversarial, not
solitaire), and **long-horizon planning** (an RPG run is thousands of sequential decisions with sparse,
delayed feedback). Two tracks split the two halves of that claim.

## Key claims

- **Battling track** — strategic reasoning under partial observability in competitive Pokémon battles,
  backed by a dataset of **20M+ battle trajectories** and heuristic / RL / LLM baseline implementations.
- **Speedrunning track** — long-horizon planning and sequential decision-making across a full Pokémon RPG
  playthrough; the paper positions this as the **first standardized RPG-speedrunning evaluation
  framework**, with a modular multi-agent orchestration baseline.
- **Competition scale**: NeurIPS 2025 Competition Track, over 100 participating teams across both tracks, a
  living leaderboard maintained post-competition at pokeagentchallenge.com.
- **Positioning**: the authors frame Pokémon explicitly as *"an unsolved benchmark"* precisely because it
  forces partial observability, adversarial reasoning, and long-horizon planning into one environment
  rather than isolating them.

## Techniques referenced
Heuristic / reinforcement-learning / LLM baseline agents for competitive battling; multi-agent
orchestration for RPG speedrunning; a public leaderboard as a living (non-static) evaluation resource.

## Gaps & caveats
- This is a **benchmark and competition-design** paper — it does not itself contain the self-refining
  harness mechanism ([Continual Harness](continual-harness.md)) that later work built on top of it. Citing
  this paper alone for "the self-refining Pokémon harness" (as the video's description link does) is a
  category error the two source pages here are meant to resolve, not repeat.
- The reference repository originally published for this paper (`sethkarten/pokeagent-speedrun`) was later
  **renamed and generalized** into `sethkarten/continual-harness`; GitHub auto-redirects the old URL, and
  the hand-engineered PokéAgent harness this paper describes survives inside that repo as one scaffold
  (`H_expert`) among several, no longer the headline contribution. See
  [Continual Harness](continual-harness.md) for what superseded it.

## Connections
- [Continual Harness](continual-harness.md) — the same lead author's follow-up paper, using this paper's
  benchmark infrastructure (and the same, later-renamed repository) as its evaluation substrate; the
  self-refining `/refine` mechanism that made Prime Agent's Pokémon result possible lives there, not here.
- [Prime Agent launch post](prime-agent-launch.md) — cites Continual Harness, not this paper, as the
  self-improvement mechanism it ships.

## Sources
- [The PokéAgent Challenge: Competitive and Long-Context Learning at Scale](https://arxiv.org/abs/2603.15563),
  Karten et al. — arXiv:2603.15563, NeurIPS 2025 Competition Track
- [pokeagentchallenge.com](https://pokeagentchallenge.com)
- Code (now `continual-harness`): [sethkarten/continual-harness](https://github.com/sethkarten/continual-harness)
