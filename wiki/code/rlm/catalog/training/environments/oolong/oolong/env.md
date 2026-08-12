---
title: 'Module: training/environments/oolong/oolong/env.py'
type: catalog
provenance: extracted
module: training/environments/oolong/oolong/env.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.environments.oolong.oolong.env`/
symbols:
  _synth_score: _synth_score().
  _build_dataset: _build_dataset().
  load_environment: load_environment().
  _find_comparison_phrase: _find_comparison_phrase().
  _attempt_answer_parse: _attempt_answer_parse().
  _score: _score().
  COMPARISON_PHRASES: COMPARISON_PHRASES.
  _build_dataset._keep: _build_dataset()._keep().
  _QUESTION_INSTRUCTION: _QUESTION_INSTRUCTION.
  __all__: __all__.
---
# Module: [`training/environments/oolong/oolong/env.py`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py)

## Functions
- `_attempt_answer_parse(answer: str)` — [`L25`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L25)
- `_build_dataset(*, dataset_name: str, min_ctx: int, max_ctx: int, num_examples: int, seed: int, exclude_numeric: bool)` — [`L91`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L91)
- `_find_comparison_phrase(output: str)` — [`L19`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L19)
- `_keep(ex)` — [`L100`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L100)
- `_score(info, state: vf.State, **_kw: Any)` — [`L76`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L76)
- `_synth_score(datapoint: dict, output: str)` — [`L39`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L39)
- `load_environment(*, dataset_name: str = "trec_coarse", min_ctx: int = 1024, max_ctx: int = 4096, num_examples: int = -1, seed: int = 42, exclude_numeric: bool = False, max_iterations: int = 12, sub_max_tokens: int = 4096, min_iterations: int = 2, min_subcall: int = 1, **kwargs: Any)` — [`L149`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L149)

## Module values
- `COMPARISON_PHRASES` — [`L16`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L16)
- `_QUESTION_INSTRUCTION` — [`L82`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L82)
- `__all__` — [`L186`](../../../../../../../../raw/code/rlm/training/environments/oolong/oolong/env.py#L186)

