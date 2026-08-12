---
title: 'Module: OpenMLE-ERL/SFT/tts_search/greedy.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/greedy.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.greedy`/
symbols:
  GreedySearch.select: GreedySearch#select().
  GreedySearch._draft_prob: GreedySearch#_draft_prob.
  GreedySearch.select_best: GreedySearch#select_best().
  GreedySearch: GreedySearch#
  logger: logger.
  AlgoConfig.debug_prob: AlgoConfig#debug_prob.
  AlgoConfig: AlgoConfig#
  GreedySearch._config: GreedySearch#_config.
  GreedySearch.__init__: GreedySearch#__init__().
  AlgoConfig.num_drafts: AlgoConfig#num_drafts.
  AlgoConfig.draft_prob: AlgoConfig#draft_prob.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/greedy.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py)

## Classes
### `AlgoConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/greedy.py:14`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L14)
- signature: `class AlgoConfig:`
- members:
  - `debug_prob` — [`L16`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L16)
  - `draft_prob` — [`L17`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L17)
  - `num_drafts` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L15)
- used by: [`_HAS_MATPLOTLIB`](services/scheduler.md#_HAS_MATPLOTLIB), [`_search_algorithm`](services/scheduler.md#Scheduler._search_algorithm), [`select`](greedy.md#GreedySearch.select), [`_draft_prob`](greedy.md#GreedySearch._draft_prob), [`__init__`](greedy.md#GreedySearch.__init__)

### `GreedySearch`  ·  implements/extends SearchAlgorithm
- def: [`OpenMLE-ERL/SFT/tts_search/greedy.py:20`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L20)
- signature: `class GreedySearch(SearchAlgorithm):`
- members:
  - `select(self, database: ProgramDatabase, task_name: str, description: str, data_dir: str, max_steps: int = 1)` — [`L26`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L26) — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
  - `select_best(self, database: ProgramDatabase, task_name: str)` — [`L99`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L99) — documented in [OpenMLE-ERL-SFT-tts_search-program_database](../../../../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md)
- protocol/private: `__init__`[`L21`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L21), `_config`[`L22`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L22), `_draft_prob`[`L23`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L23)
- uses (calls/refs, reference-scoped): [`Program`](program_database.md#Program), [`fitness`](program_database.md#Program.fitness), [`build_prompt`](prompt_builder.md#build_prompt), [`get_best`](program_database.md#ProgramDatabase.get_best), [`get_random_by_fitness`](program_database.md#ProgramDatabase.get_random_by_fitness), [`ProgramDatabase`](program_database.md#ProgramDatabase), [`id`](program_database.md#Program.id), [`SearchAlgorithm`](program_database.md#SearchAlgorithm), [`debug_prob`](greedy.md#AlgoConfig.debug_prob), [`logger`](greedy.md#logger), [`count_by_generation_mode`](program_database.md#ProgramDatabase.count_by_generation_mode), [`is_empty`](program_database.md#ProgramDatabase.is_empty), [`AlgoConfig`](greedy.md#AlgoConfig), [`draft_prob`](greedy.md#AlgoConfig.draft_prob), [`num_drafts`](greedy.md#AlgoConfig.num_drafts)
- used by: [`_create_requests`](services/scheduler.md#Scheduler._create_requests), [`_HAS_MATPLOTLIB`](services/scheduler.md#_HAS_MATPLOTLIB), [`_search_algorithm`](services/scheduler.md#Scheduler._search_algorithm), [`select`](program_database.md#SearchAlgorithm.select), [`select_best`](program_database.md#SearchAlgorithm.select_best), [`SearchAlgorithm`](program_database.md#SearchAlgorithm)

## Module values
- `logger` — [`L10`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/greedy.py#L10)

