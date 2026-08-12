---
title: 'Module: OpenMLE-Evo/tts_search/program_database.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/program_database.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.program_database`/
symbols:
  ProgramDatabase.add: ProgramDatabase#add().
  Program.to_dict: Program#to_dict().
  Program: Program#
  ProgramDatabase._get_connection: ProgramDatabase#_get_connection().
  Program.__post_init__: Program#__post_init__().
  Program.code: Program#code.
  Program.feedback: Program#feedback.
  ProgramDatabase._local: ProgramDatabase#_local.
  Program.from_dict: Program#from_dict().
  ProgramDatabase.get_by_id: ProgramDatabase#get_by_id().
  ProgramDatabase.get_best: ProgramDatabase#get_best().
  ProgramDatabase.get_random_by_fitness: ProgramDatabase#get_random_by_fitness().
  ProgramDatabase.get_top_k: ProgramDatabase#get_top_k().
  ProgramDatabase.list_by_task: ProgramDatabase#list_by_task().
  Program.task_name: Program#task_name.
  ProgramDatabase.clear: ProgramDatabase#clear().
  SearchAlgorithm.select: SearchAlgorithm#select().
  SearchAlgorithm.select_best: SearchAlgorithm#select_best().
  ProgramDatabase._lock: ProgramDatabase#_lock.
  Program.fitness: Program#fitness.
  ProgramDatabase._init_db: ProgramDatabase#_init_db().
  Program.reward: Program#reward.
  Program.run_log: Program#run_log.
  Program.metadata: Program#metadata.
  ProgramDatabase.max_per_task: ProgramDatabase#max_per_task.
  ProgramDatabase.is_empty: ProgramDatabase#is_empty().
  ProgramDatabase.size: ProgramDatabase#size().
  ProgramDatabase.count_by_generation_mode: ProgramDatabase#count_by_generation_mode().
  ProgramDatabase.close: ProgramDatabase#close().
  Program.task_id: Program#task_id.
  Program.score: Program#score.
  Program.base_reward: Program#base_reward.
  Program.parent_id: Program#parent_id.
  Program.parent_code: Program#parent_code.
  Program.generation_mode: Program#generation_mode.
  Program.raw_text: Program#raw_text.
  ProgramDatabase: ProgramDatabase#
  Program.id: Program#id.
  ProgramDatabase.db_path: ProgramDatabase#db_path.
  DatabaseLifecycle: DatabaseLifecycle#
  DatabaseLifecycle.ROLLOUT: DatabaseLifecycle#ROLLOUT.
  DatabaseLifecycle.STEP: DatabaseLifecycle#STEP.
  DatabaseLifecycle.TASK: DatabaseLifecycle#TASK.
  ProgramDatabase.__init__: ProgramDatabase#__init__().
  SearchAlgorithm: SearchAlgorithm#
---
# Module: [`OpenMLE-Evo/tts_search/program_database.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py)

## Classes
### `DatabaseLifecycle`  ·  implements/extends Enum
- def: [`OpenMLE-Evo/tts_search/program_database.py:15`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L15)
- doc: Lifecycle modes for Program Database.
- signature: `class DatabaseLifecycle(Enum):`
- members:
  - `ROLLOUT` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L17)
  - `STEP` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L18)
  - `TASK` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L19)

### `Program`
- def: [`OpenMLE-Evo/tts_search/program_database.py:23`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L23) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- doc: Represents a program in the database.
- signature: `class Program:`
- members:
  - `from_dict(cls, data: dict[str, Any])` — [`L69`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L69) — Create program from dictionary. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `to_dict(self)` — [`L48`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L48) — Convert program to dictionary for storage. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `base_reward` — [`L32`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L32) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `code` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L28) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `feedback` — [`L34`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L34) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `fitness` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L31) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `generation_mode` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L37) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `id` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L25)
  - `metadata` — [`L39`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L39) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `parent_code` — [`L36`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L36) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `parent_id` — [`L35`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L35) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `raw_text` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L38) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `reward` — [`L30`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L30) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `run_log` — [`L33`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L33) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `score` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L29) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `task_id` — [`L26`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L26) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `task_name` — [`L27`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L27) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- protocol/private: `__post_init__`[`L41`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L41)
- used by: [`add`](program_database.md#ProgramDatabase.add), [`build_prompt`](prompt_builder.md#build_prompt), [`build_crossover_prompt`](prompt_builder.md#build_crossover_prompt), [`build_debug_prompt`](prompt_builder.md#build_debug_prompt), [`build_improve_prompt`](prompt_builder.md#build_improve_prompt), [`get_best`](program_database.md#ProgramDatabase.get_best), [`get_by_id`](program_database.md#ProgramDatabase.get_by_id), [`get_random_by_fitness`](program_database.md#ProgramDatabase.get_random_by_fitness), [`get_top_k`](program_database.md#ProgramDatabase.get_top_k), [`list_by_task`](program_database.md#ProgramDatabase.list_by_task), [`select`](program_database.md#SearchAlgorithm.select), [`select_best`](program_database.md#SearchAlgorithm.select_best)

### `ProgramDatabase`
- def: [`OpenMLE-Evo/tts_search/program_database.py:99`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L99)
- doc: Database for storing and managing programs during rollout.
- signature: `class ProgramDatabase:`
- members:
  - `__init__(self, db_path: str = "program_database.db", max_per_task: int | None = 10)` — [`L106`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L106) — Initialize Program Database.
  - `_get_connection(self)` — [`L129`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L129) — Get thread-local database connection. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `_init_db(self)` — [`L136`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L136) — Initialize database schema. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `add(self, program: Program)` — [`L219`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L219) — Add a program to the database, maintaining top k per task by fitness. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `clear(self, task_name: str | None = None)` — [`L314`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L314) — Clear programs from the database. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `close(self)` — [`L332`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L332) — Close database connection.
  - `count_by_generation_mode(self, task_name: str, generation_mode: str)` — [`L304`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L304) — Count programs for a task by generation mode. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `get_best(self, task_name: str)` — [`L338`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L338) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `get_by_id(self, program_id: int)` — [`L275`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L275) — Get a program by its ID. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `get_random_by_fitness(self, task_name: str, fitness: float)` — [`L353`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L353) — Randomly sample a program by fitness. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `get_top_k(self, task_name: str, k: int)` — [`L371`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L371) — Return top-k programs by fitness (descending). — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `is_empty(self, task_name: str)` — [`L287`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L287) — Check if database is empty for a task.
  - `list_by_task(self, task_name: str)` — [`L387`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L387) — List programs for a task in creation order. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `size(self, task_name: str)` — [`L296`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L296) — Get the number of programs for a task.
  - `db_path` — [`L117`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L117) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `max_per_task` — [`L118`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L118) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- protocol/private: `_local`[`L120`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L120), `_lock`[`L121`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L121)
- uses (calls/refs, reference-scoped): [`Program`](program_database.md#Program), [`code`](program_database.md#Program.code), [`feedback`](program_database.md#Program.feedback), [`from_dict`](program_database.md#Program.from_dict), [`task_name`](program_database.md#Program.task_name), [`fitness`](program_database.md#Program.fitness), [`metadata`](program_database.md#Program.metadata), [`reward`](program_database.md#Program.reward), [`run_log`](program_database.md#Program.run_log), [`base_reward`](program_database.md#Program.base_reward), [`generation_mode`](program_database.md#Program.generation_mode), [`parent_code`](program_database.md#Program.parent_code), [`parent_id`](program_database.md#Program.parent_id), [`raw_text`](program_database.md#Program.raw_text), [`score`](program_database.md#Program.score), [`task_id`](program_database.md#Program.task_id)
- used by: [`select`](program_database.md#SearchAlgorithm.select), [`select_best`](program_database.md#SearchAlgorithm.select_best)

### `SearchAlgorithm`  ·  implements/extends ABC
- def: [`OpenMLE-Evo/tts_search/program_database.py:403`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L403)
- doc: Abstract base class for search algorithms to select programs from database.
- signature: `class SearchAlgorithm(ABC):`
- members:
  - `select(self, database: ProgramDatabase, task_name: str, task_description: str, data_description: str, public_system_prompt: str, public_user_prompt: str, data_dir: str, max_steps: int = 1)` — [`L407`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L407) — Select a program and build prompt. — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
  - `select_best(self, database: ProgramDatabase, task_name: str)` — [`L445`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/program_database.py#L445) — documented in [OpenMLE-Evo-tts_search-program_database](../../../concepts/OpenMLE-Evo-tts_search-program_database.md)
- uses (calls/refs, reference-scoped): [`Program`](program_database.md#Program), [`ProgramDatabase`](program_database.md#ProgramDatabase)

