---
title: 'Module: rdagent/scenarios/rl/autorl_bench/test/test_fixes.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/test/test_fixes.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.test.test_fixes`/
symbols:
  report: report().
  test_b2b3_lock_and_cache: test_b2b3_lock_and_cache().
  main: main().
  test_b4_error_passthrough: test_b4_error_passthrough().
  test_b1_lora_detection: test_b1_lora_detection().
  test_baseline_integrity: test_baseline_integrity().
  test_alfworld_prompt_truncation: test_alfworld_prompt_truncation().
  test_b2b3_lock_and_cache.submit_wrapper: test_b2b3_lock_and_cache().submit_wrapper().
  FAIL: FAIL.
  PASS: PASS.
  test_alfworld_prompt_truncation.ToyTokenizer: test_alfworld_prompt_truncation().ToyTokenizer#
  test_b2b3_lock_and_cache.mock_run_eval: test_b2b3_lock_and_cache().mock_run_eval().
  test_b2b3_lock_and_cache.mock_fail_eval: test_b2b3_lock_and_cache().mock_fail_eval().
  test_b4_error_passthrough.mock_error_eval: test_b4_error_passthrough().mock_error_eval().
  test_alfworld_prompt_truncation.ToyTokenizer.encode: test_alfworld_prompt_truncation().ToyTokenizer#encode().
  test_alfworld_prompt_truncation.ToyTokenizer.decode: test_alfworld_prompt_truncation().ToyTokenizer#decode().
---
# Module: [`rdagent/scenarios/rl/autorl_bench/test/test_fixes.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py)

## Classes
### `ToyTokenizer`
- def: [`rdagent/scenarios/rl/autorl_bench/test/test_fixes.py:215`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L215)
- signature: `class ToyTokenizer:`
- members:
  - `decode(self, token_ids)` — [`L219`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L219)
  - `encode(self, text)` — [`L216`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L216)
- used by: (1 test-only callers)

## Functions
- `main()` — [`L369`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L369)
- `mock_error_eval(**kwargs)` — [`L323`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L323)
- `mock_fail_eval(**kwargs)` — [`L297`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L297)
- `mock_run_eval(**kwargs)` — [`L246`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L246)
- `report(name: str, ok: bool, detail: str = "")` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L25)
- `submit_wrapper(mp)` — [`L268`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L268)
- `test_alfworld_prompt_truncation()` — [`L209`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L209)
- `test_b1_lora_detection()` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L38)
- `test_b2b3_lock_and_cache()` — [`L231`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L231)
- `test_b4_error_passthrough()` — [`L316`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L316)
- `test_baseline_integrity()` — [`L160`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L160)

## Module values
- `FAIL` — [`L22`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L22)
- `PASS` — [`L21`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/test/test_fixes.py#L21)

