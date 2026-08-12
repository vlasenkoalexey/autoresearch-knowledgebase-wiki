---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.sglang_rollout`/
symbols:
  generate: generate().
  eval_rollout_single_dataset: eval_rollout_single_dataset().
  generate_rollout_async: generate_rollout_async().
  generate_and_rm: generate_and_rm().
  generate_and_rm_group: generate_and_rm_group().
  abort: abort().
  GenerateState.submit_generate_tasks: GenerateState#submit_generate_tasks().
  generate_rollout: generate_rollout().
  eval_rollout: eval_rollout().
  GenerateState: GenerateState#
  GenerateState.dp_rank_context: GenerateState#dp_rank_context().
  GenerateState.pendings: GenerateState#pendings.
  logger: logger.
  GenerateState.dp_counts: GenerateState#dp_counts.
  GenerateState.aborted: GenerateState#aborted.
  GenerateState.processor: GenerateState#processor.
  EVAL_PROMPT_DATASET: EVAL_PROMPT_DATASET.
  GenerateState.tokenizer: GenerateState#tokenizer.
  GenerateState.dp_rank: GenerateState#dp_rank.
  GenerateState.remaining_batch_size: GenerateState#remaining_batch_size.
  GenerateState.reset: GenerateState#reset().
  GenerateState.args: GenerateState#args.
  GenerateState.semaphore: GenerateState#semaphore.
  GenerateState.sampling_params: GenerateState#sampling_params.
  GenerateState.group_sampling_seeds: GenerateState#group_sampling_seeds.
  __all__: __all__.
  GenerateState.__init__: GenerateState#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py)

## Classes
### `GenerateState`
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py:39`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L39)
- doc: The global state for the generation process.
- signature: `class GenerateState(metaclass=SingletonMeta):`
- members:
  - `dp_rank_context(self)` — [`L76`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L76)
  - `reset(self)` — [`L87`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L87)
  - `submit_generate_tasks(self, samples: list[list[Sample]])` — [`L92`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L92)
  - `aborted` — [`L90`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L90)
  - `args` — [`L46`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L46)
  - `dp_counts` — [`L70`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L70)
  - `dp_rank` — [`L71`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L71)
  - `group_sampling_seeds` — [`L67`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L67)
  - `pendings` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L89)
  - `processor` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L48)
  - `remaining_batch_size` — [`L88`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L88)
  - `sampling_params` — [`L53`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L53)
  - `semaphore` — [`L50`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L50)
  - `tokenizer` — [`L47`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L47)
- protocol/private: `__init__`[`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L44)
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample), [`generate_and_rm_group`](sglang_rollout.md#generate_and_rm_group), [`load_processor`](../utils/processing_utils.md#load_processor), [`load_tokenizer`](../utils/processing_utils.md#load_tokenizer), [`SingletonMeta`](../utils/misc.md#SingletonMeta)
- used by: [`generate`](sglang_rollout.md#generate), [`generate_rollout_async`](sglang_rollout.md#generate_rollout_async), [`generate_and_rm`](sglang_rollout.md#generate_and_rm), [`generate_and_rm_group`](sglang_rollout.md#generate_and_rm_group), [`abort`](sglang_rollout.md#abort)

## Functions
- `abort(args: Namespace, rollout_id: int)` — [`L332`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L332)
- `eval_rollout(args: Namespace, rollout_id: int)` — [`L469`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L469)
- `eval_rollout_single_dataset(args: Namespace, rollout_id: int, dataset_cfg: EvalDatasetConfig)` — [`L482`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L482) — An example to implement the eval_rollout function for an rule based rm rollout generation.
- `generate(args: Namespace, sample: Sample, sampling_params: dict[str, Any])` — [`L108`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L108) — Generate using traditional SGLang router with token-based workflow
- `generate_and_rm(args: Namespace, sample: Sample | list[Sample], sampling_params: dict[str, Any], evaluation: bool = False)` — [`L208`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L208)
- `generate_and_rm_group(args: Namespace, group: list[Sample], sampling_params: dict[str, Any], evaluation: bool = False)` — [`L273`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L273)
- `generate_rollout(args: Namespace, rollout_id: int, data_source: Any, evaluation: bool = False)` — [`L584`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L584) — An example to implement the generate_rollout function for an rule based rm rollout generation.
- `generate_rollout_async(args: Namespace, rollout_id: int, data_source: Callable[[int], list[list[Sample]]])` — [`L372`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L372) — An example to implement the generate_rollout function for an rule based rm rollout generation.

## Module values
- `EVAL_PROMPT_DATASET` — [`L466`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L466)
- `__all__` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L34)
- `logger` — [`L36`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/sglang_rollout.py#L36)

