---
title: 'Module: OpenMLE-Gym/builder_core/utils/nodes.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/builder_core/utils/nodes.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.builder_core.utils.nodes`/NodeExecutor#
symbols:
  NodeExecutor.todo: todo.
  NodeExecutor.structure: structure.
  NodeExecutor.prepare_single_competition: prepare_single_competition().
  NodeExecutor.Copy: Copy().
  NodeExecutor.Metric: Metric().
  NodeExecutor.Perceive: Perceive().
  NodeExecutor.Prepare: Prepare().
  NodeExecutor.Describe: Describe().
  NodeExecutor.Next: Next().
  NodeExecutor.Download: Download().
  NodeExecutor: ''
  NodeExecutor._cleanup_failed_competition: _cleanup_failed_competition().
  NodeExecutor.Scrape: Scrape().
  NodeExecutor.extract: extract().
  NodeExecutor.get_prepare_function: get_prepare_function().
  NodeExecutor.prepare_validation: prepare_validation().
  NodeExecutor.llm_provider_tools: llm_provider_tools.
  NodeExecutor._generate_tree: _generate_tree().
  NodeExecutor.download: download().
  NodeExecutor.get_directory_tree: get_directory_tree().
  NodeExecutor.prepare_implement: prepare_implement().
  NodeExecutor.Router1: Router1().
  NodeExecutor.Router2: Router2().
  NodeExecutor.Router3: Router3().
  NodeExecutor.Router4: Router4().
  NodeExecutor.Router5: Router5().
  NodeExecutor.Router6: Router6().
  NodeExecutor.tools: tools.
  NodeExecutor.llm_provider: llm_provider.
  NodeExecutor._load_sample_file: _load_sample_file().
  NodeExecutor.tree: tree.
  NodeExecutor.csvinfo: csvinfo.
  NodeExecutor.max_tool_call: max_tool_call.
  NodeExecutor._is_compressed: _is_compressed().
  NodeExecutor.__init__: __init__().
  NodeExecutor.delete_raw: delete_raw.
  NodeExecutor.validate_member: validate_member().
  NodeExecutor._clean_code_output: _clean_code_output().
  NodeExecutor.COMPRESSED_EXTENSIONS: COMPRESSED_EXTENSIONS.
  NodeExecutor.KAGGLE_DATA_URL: KAGGLE_DATA_URL.
  NodeExecutor.info_csv: info_csv.
  NodeExecutor.sample_dir: sample_dir.
  NodeExecutor.code_execution_mode: code_execution_mode.
  NodeExecutor.code_timeout: code_timeout.
  NodeExecutor._load_kaggle_auth: _load_kaggle_auth().
  NodeExecutor._load_module: _load_module().
---
# Module: [`OpenMLE-Gym/builder_core/utils/nodes.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py)

## Classes
### `NodeExecutor`
- def: [`OpenMLE-Gym/builder_core/utils/nodes.py:39`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L39)
- doc: Orchestrates downloading, processing, and preparing Kaggle competition data.
- signature: `class NodeExecutor:`
- members:
  - `Copy(self, state: AgentState)` — [`L630`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L630) — Prepare data for a single competition by copying and extracting. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Describe(self, state: AgentState)` — [`L812`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L812) — Generate description for a single competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Download(self, state: AgentState)` — [`L593`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L593) — Download a single competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Metric(self, state: AgentState)` — [`L988`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L988) — Generate metric script for a single competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Next(self, state: AgentState)` — [`L1063`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1063) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Perceive(self, state: AgentState)` — [`L744`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L744) — Run optional file inventory. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Prepare(self, state: AgentState)` — [`L884`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L884) — Generate prepare script for a single competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Router1(self, state: AgentState)` — [`L1121`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1121) — Route based on download status. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Router2(self, state: AgentState)` — [`L1125`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1125) — Route based on copy status. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Router3(self, state: AgentState)` — [`L1129`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1129) — Route based on web info status. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Router4(self, state: AgentState)` — [`L1133`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1133) — Route based on file info status.
  - `Router5(self, state: AgentState)` — [`L1137`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1137) — Route based on describe status. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Router6(self, state: AgentState)` — [`L1141`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L1141) — Route based on prepare status. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `Scrape(self, state: AgentState)` — [`L700`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L700) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `__init__(self, base_dir: str, batch_name: str, api_key: Optional[str] = None, base_url: Optional[str] = None, model: Optional[str] = None, todo: Task = None, tools: List[Any] = None, info_csv: Optional[Path] = None, sample_dir: Optional[Path] = None, delete_raw: bool = False, code_execution_mode: str = "process", code_timeout: float = 600)` — [`L46`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L46) — Initialize the NodeExecutor.
  - `_clean_code_output(self, message: str)` — [`L355`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L355) — Clean code output from LLM (remove markdown formatting).
  - `_cleanup_failed_competition(self, comp_id: str)` — [`L571`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L571) — Clean up directories for a failed competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `_is_compressed(self, file_path: Path)` — [`L111`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L111) — Check if a file is compressed based on its extension.
  - `_load_kaggle_auth(self)` — [`L122`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L122) — Load Kaggle username/key auth from env or KAGGLE_CONFIG_DIR/kaggle.json.
  - `_load_module(self, module_name: str, file_path: Path)` — [`L394`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L394) — Dynamically load a Python module from a file.
  - `_load_sample_file(self, filename: str)` — [`L340`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L340) — Load a sample file from the samples directory. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `download(self, comp_id: str, target_dir: Path)` — [`L152`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L152) — Download a Kaggle competition dataset using Kaggle CLI.
  - `extract(self, compressed_path: Path, dst: Path, recursive: bool = True, already_extracted: Optional[Set[Path]] = None)` — [`L201`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L201) — Extract compressed files with optional recursive extraction.
  - `get_directory_tree(self, start_path: Path, max_depth: int = 6)` — [`L322`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L322) — Get tree representation of a directory.
  - `get_prepare_function(self, comp_id: str)` — [`L426`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L426) — Get the prepare function from prepare.py. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `prepare_implement(self, comp_id: str)` — [`L552`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L552) — Wrapper for prepare_single_competition with logging. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `prepare_single_competition(self, comp_id: str)` — [`L468`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L468) — Prepare data for a single competition. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `prepare_validation(self, comp_id: str)` — [`L445`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L445) — Check if required files and directories exist. — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `validate_member(name: str)` — [`L230`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L230)
  - `COMPRESSED_EXTENSIONS` — [`L43`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L43)
  - `KAGGLE_DATA_URL` — [`L44`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L44)
  - `code_execution_mode` — [`L79`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L79)
  - `code_timeout` — [`L80`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L80)
  - `csvinfo` — [`L81`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L81)
  - `delete_raw` — [`L78`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L78)
  - `info_csv` — [`L76`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L76)
  - `llm_provider` — [`L92`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L92)
  - `llm_provider_tools` — [`L98`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L98)
  - `max_tool_call` — [`L90`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L90)
  - `sample_dir` — [`L77`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L77)
  - `structure` — [`L74`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L74) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `todo` — [`L105`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L105) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `tools` — [`L84`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L84)
  - `tree` — [`L75`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L75)
- protocol/private: `_generate_tree`[`L277`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/nodes.py#L277)
- uses (calls/refs, reference-scoped): [`run_task_process`](../../openmle_gym/process_runner.md#run_task_process), [`AgentState`](state.md#AgentState), [`ok`](../../openmle_gym/process_runner.md#TaskProcessOutcome.ok), [`comp_id_dir`](struct.md#Structure.comp_id_dir), [`error`](../../openmle_gym/process_runner.md#TaskProcessOutcome.error), [`stderr`](../../openmle_gym/process_runner.md#TaskProcessOutcome.stderr), [`stdout`](../../openmle_gym/process_runner.md#TaskProcessOutcome.stdout), [`public_dir`](struct.md#Structure.public_dir), [`query`](chat.md#OpenAILLMProvider.query), [`atomic_write_text`](../../openmle_gym/common.md#atomic_write_text), [`raw_dir`](struct.md#Structure.raw_dir), [`private_dir`](struct.md#Structure.private_dir), [`data_dir`](struct.md#Structure.data_dir), [`utils_dir`](struct.md#Structure.utils_dir), [`data_comp_id_dir`](struct.md#Structure.data_comp_id_dir), [`Task`](task.md#Task), [`DOWNLOAD_DIR`](struct.md#Structure.DOWNLOAD_DIR), [`Structure`](struct.md#Structure), [`gen_perceiver`](prompts.md#gen_perceiver), [`OpenAILLMProvider`](chat.md#OpenAILLMProvider), [`description_info`](prompts.md#description_info), [`gen_description`](prompts.md#gen_description), [`gen_metric_script`](prompts.md#gen_metric_script), [`gen_prepare_script`](prompts.md#gen_prepare_script), [`metric_info`](prompts.md#metric_info)
- used by: [`Graph`](../design.md#Graph)  (10 test-only)

