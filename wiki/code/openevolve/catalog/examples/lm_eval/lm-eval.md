---
title: 'Module: examples/lm_eval/lm-eval.py'
type: catalog
provenance: extracted
module: examples/lm_eval/lm-eval.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.lm_eval.lm-eval`/
symbols:
  OpenEvolve.generate: OpenEvolve#generate().
  val: val.
  args: args.
  value: value.
  p: p.
  results: results.
  results_path: results_path.
  lm_obj: lm_obj.
  f: f.
  task_dict: task_dict.
  metrics: metrics.
  task: task.
  OpenEvolve.generate_until: OpenEvolve#generate_until().
  OpenEvolve.base_system_message: OpenEvolve#base_system_message.
  short: short.
  PIPELINE_CMD: PIPELINE_CMD.
  OpenEvolve: OpenEvolve#
  OpenEvolve.init_file: OpenEvolve#init_file.
  OpenEvolve.evaluator_file: OpenEvolve#evaluator_file.
  OpenEvolve.iterations: OpenEvolve#iterations.
  OpenEvolve.extra_param: OpenEvolve#extra_param.
  OpenEvolve.config_file: OpenEvolve#config_file.
  OpenEvolve.prompt_path: OpenEvolve#prompt_path.
  OpenEvolve.evaluator_prompt_path: OpenEvolve#evaluator_prompt_path.
  OpenEvolve.best_path: OpenEvolve#best_path.
  timestamp: timestamp.
  key: key.
  name: name.
  OpenEvolve.__init__: OpenEvolve#__init__().
  OpenEvolve.loglikelihood: OpenEvolve#loglikelihood().
  OpenEvolve.loglikelihood_rolling: OpenEvolve#loglikelihood_rolling().
---
# Module: [`examples/lm_eval/lm-eval.py`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py)

## Classes
### `OpenEvolve`
- def: [`examples/lm_eval/lm-eval.py:28`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L28)
- signature: `class OpenEvolve(LM):`
- members:
  - `generate(self, prompts: List[str], max_gen_toks: int = None, stop=None, **kwargs)` — [`L51`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L51)
  - `generate_until(self, requests: Iterable[Any], **kw)` — [`L103`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L103)
  - `loglikelihood(self, requests: Iterable[Tuple[str, str]], **kw)` — [`L95`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L95)
  - `loglikelihood_rolling(self, requests: Iterable[str], **kw)` — [`L99`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L99)
  - `base_system_message` — [`L49`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L49)
  - `best_path` — [`L48`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L48)
  - `config_file` — [`L43`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L43)
  - `evaluator_file` — [`L40`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L40)
  - `evaluator_prompt_path` — [`L47`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L47)
  - `extra_param` — [`L42`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L42)
  - `init_file` — [`L39`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L39)
  - `iterations` — [`L41`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L41)
  - `prompt_path` — [`L46`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L46)
- protocol/private: `__init__`[`L29`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L29)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Module values
- `PIPELINE_CMD` — [`L24`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L24)
- `args` — [`L162`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L162)
- `f` — [`L192`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L192)
- `key` — [`L199`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L199)
- `lm_obj` — [`L164`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L164)
- `metrics` — [`L197`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L197)
- `name` — [`L206`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L206)
- `p` — [`L140`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L140)
- `results` — [`L173`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L173)
- `results_path` — [`L185`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L185)
- `short` — [`L196`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L196)
- `task` — [`L197`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L197)
- `task_dict` — [`L171`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L171)
- `timestamp` — [`L184`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L184)
- `val` — [`L199`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L199)
- `value` — [`L206`](../../../../../../raw/code/openevolve/examples/lm_eval/lm-eval.py#L206)

