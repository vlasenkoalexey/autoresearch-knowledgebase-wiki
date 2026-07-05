---
title: 'Module: examples/mlx_metal_kernel_opt/evaluator.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.evaluator`/
symbols:
  BulletproofMetalEvaluator.evaluate: BulletproofMetalEvaluator#evaluate().
  BulletproofMetalEvaluator._command_buffer_protected_benchmark: BulletproofMetalEvaluator#_command_buffer_protected_benchmark().
  BulletproofMetalEvaluator._gpu_protected_measure_baseline: BulletproofMetalEvaluator#_gpu_protected_measure_baseline().
  BulletproofMetalEvaluator._analyze_performance_with_safety_metrics: BulletproofMetalEvaluator#_analyze_performance_with_safety_metrics().
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.max_position_embeddings: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#max_position_embeddings.
  BulletproofMetalEvaluator.total_metal_errors: BulletproofMetalEvaluator#total_metal_errors.
  BulletproofMetalEvaluator._get_comprehensive_error_statistics: BulletproofMetalEvaluator#_get_comprehensive_error_statistics().
  BulletproofMetalEvaluator._result_to_dict: BulletproofMetalEvaluator#_result_to_dict().
  BulletproofMetalEvaluator._reset_error_counters: BulletproofMetalEvaluator#_reset_error_counters().
  BulletproofMetalEvaluator._bulletproof_execute_with_gpu_protection: BulletproofMetalEvaluator#_bulletproof_execute_with_gpu_protection().
  BulletproofMetalEvaluator._store_enhanced_baseline_metrics: BulletproofMetalEvaluator#_store_enhanced_baseline_metrics().
  BulletproofMetalEvaluator._calculate_safety_score: BulletproofMetalEvaluator#_calculate_safety_score().
  BulletproofMetalEvaluator._bulletproof_extract_custom_attention: BulletproofMetalEvaluator#_bulletproof_extract_custom_attention().
  BulletproofMetalEvaluator._test_single_sequence_memory_safe: BulletproofMetalEvaluator#_test_single_sequence_memory_safe().
  BulletproofMetalEvaluator._get_safe_benchmark_configs: BulletproofMetalEvaluator#_get_safe_benchmark_configs().
  BulletproofMetalEvaluator.benchmark_suite: BulletproofMetalEvaluator#benchmark_suite.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.max_position_embeddings: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#max_position_embeddings.
  BulletproofMetalEvaluator.max_retry_attempts: BulletproofMetalEvaluator#max_retry_attempts.
  BulletproofMetalEvaluator._generate_comprehensive_summary: BulletproofMetalEvaluator#_generate_comprehensive_summary().
  BulletproofMetalEvaluator._create_comprehensive_failure_result: BulletproofMetalEvaluator#_create_comprehensive_failure_result().
  BulletproofMetalEvaluator.retry_base_delay: BulletproofMetalEvaluator#retry_base_delay.
  BulletproofMetalEvaluator.metal_compilation_errors: BulletproofMetalEvaluator#metal_compilation_errors.
  BulletproofMetalEvaluator.baseline_metrics: BulletproofMetalEvaluator#baseline_metrics.
  BulletproofMetalEvaluator.metal_command_buffer_errors: BulletproofMetalEvaluator#metal_command_buffer_errors.
  BulletproofMetalEvaluator.metal_memory_violations: BulletproofMetalEvaluator#metal_memory_violations.
  BulletproofMetalEvaluator._gpu_protected_apply_hook: BulletproofMetalEvaluator#_gpu_protected_apply_hook().
  BulletproofMetalEvaluator._gpu_protected_remove_hook: BulletproofMetalEvaluator#_gpu_protected_remove_hook().
  evaluate: evaluate().
  BulletproofMetalEvaluator.gpu_resource_errors: BulletproofMetalEvaluator#gpu_resource_errors.
  BulletproofMetalEvaluator._ensure_clean_gpu_state: BulletproofMetalEvaluator#_ensure_clean_gpu_state().
  BulletproofMetalEvaluator._safe_calculate_improvement: BulletproofMetalEvaluator#_safe_calculate_improvement().
  BulletproofMetalEvaluator._calculate_safety_adjusted_score: BulletproofMetalEvaluator#_calculate_safety_adjusted_score().
  BulletproofMetalEvaluator._print_bulletproof_evaluation_results: BulletproofMetalEvaluator#_print_bulletproof_evaluation_results().
  test_bulletproof_evaluator: test_bulletproof_evaluator().
  MetalKernelSafetyError: MetalKernelSafetyError#
  BulletproofMetalEvaluator.retry_attempts_used: BulletproofMetalEvaluator#retry_attempts_used.
  BulletproofMetalEvaluator.model_path: BulletproofMetalEvaluator#model_path.
  BulletproofMetalEvaluator.successful_fallbacks: BulletproofMetalEvaluator#successful_fallbacks.
  BulletproofMetalEvaluator.max_sequence_length_safe: BulletproofMetalEvaluator#max_sequence_length_safe.
  BulletproofMetalEvaluator.max_batch_size_safe: BulletproofMetalEvaluator#max_batch_size_safe.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.num_attention_heads: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#num_attention_heads.
  GPUCommandBufferError: GPUCommandBufferError#
  BulletproofMetalEvaluator: BulletproofMetalEvaluator#
  BulletproofMetalEvaluator.kernel_validation_timeout: BulletproofMetalEvaluator#kernel_validation_timeout.
  BulletproofMetalEvaluator.baseline_results: BulletproofMetalEvaluator#baseline_results.
  BulletproofMetalEvaluator._static_validate_metal_kernel_syntax: BulletproofMetalEvaluator#_static_validate_metal_kernel_syntax().
  BulletproofMetalEvaluator._validate_custom_attention_class: BulletproofMetalEvaluator#_validate_custom_attention_class().
  BulletproofMetalEvaluator._validate_metal_kernel_safety: BulletproofMetalEvaluator#_validate_metal_kernel_safety().
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.num_key_value_heads: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#num_key_value_heads.
  BulletproofMetalEvaluator._memory_safe_correctness_test: BulletproofMetalEvaluator#_memory_safe_correctness_test().
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#
  BulletproofMetalEvaluator._apply_attention_hook_safely: BulletproofMetalEvaluator#_apply_attention_hook_safely().
  BulletproofMetalEvaluator._remove_attention_hook_safely: BulletproofMetalEvaluator#_remove_attention_hook_safely().
  BulletproofMetalEvaluator._create_bulletproof_execution_environment: BulletproofMetalEvaluator#_create_bulletproof_execution_environment().
  BulletproofMetalEvaluator._ensure_standard_attention: BulletproofMetalEvaluator#_ensure_standard_attention().
  MetalMemoryViolationError: MetalMemoryViolationError#
  BulletproofMetalEvaluator.__init__: BulletproofMetalEvaluator#__init__().
  BulletproofMetalEvaluator.max_head_dimension_safe: BulletproofMetalEvaluator#max_head_dimension_safe.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.hidden_size: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#hidden_size.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.head_dim: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#head_dim.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.rms_norm_eps: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#rms_norm_eps.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.rope_theta: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#rope_theta.
  BulletproofMetalEvaluator._validate_metal_kernel_safety.MockArgs.rope_scaling: BulletproofMetalEvaluator#_validate_metal_kernel_safety().MockArgs#rope_scaling.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.hidden_size: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#hidden_size.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.num_attention_heads: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#num_attention_heads.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.num_key_value_heads: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#num_key_value_heads.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.head_dim: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#head_dim.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.rms_norm_eps: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#rms_norm_eps.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.rope_theta: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#rope_theta.
  BulletproofMetalEvaluator._memory_safe_correctness_test.MockArgs.rope_scaling: BulletproofMetalEvaluator#_memory_safe_correctness_test().MockArgs#rope_scaling.
---
# Module: [`examples/mlx_metal_kernel_opt/evaluator.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py)

## Classes
### `BulletproofMetalEvaluator`
- def: [`examples/mlx_metal_kernel_opt/evaluator.py:66`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L66)
- doc: Bulletproof evaluator that NEVER crashes from Metal kernel failures
- signature: `class BulletproofMetalEvaluator:`
- members:
  - `_analyze_performance_with_safety_metrics(self, baseline_results: List[BenchmarkResult], custom_results: List[BenchmarkResult])` — [`L1073`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1073) — Analyze performance with enhanced safety metrics
  - `_apply_attention_hook_safely(self, custom_attention_class: Any)` — [`L939`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L939) — Safely apply attention hook
  - `_bulletproof_execute_with_gpu_protection(self, func)` — [`L426`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L426) — Execute function with maximum GPU and Metal kernel protection
  - `_bulletproof_extract_custom_attention(self, program_text: str)` — [`L231`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L231) — Bulletproof extraction with comprehensive Metal kernel validation
  - `_calculate_safety_adjusted_score(self, performance_analysis: Dict[str, Any], correctness: float)` — [`L1234`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1234) — Calculate final score adjusted for safety
  - `_calculate_safety_score(self)` — [`L1219`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1219) — Calculate overall safety score based on error statistics
  - `_command_buffer_protected_benchmark(self, program_text: str, custom_attention_class: Any)` — [`L780`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L780) — Command-buffer-protected benchmarking with maximum safety
  - `_create_bulletproof_execution_environment(self)` — [`L978`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L978) — Create bulletproof execution environment with enhanced imports
  - `_create_comprehensive_failure_result(self, error_message: str)` — [`L1406`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1406) — Create comprehensive failure result with full error statistics
  - `_ensure_clean_gpu_state(self)` — [`L911`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L911) — Ensure clean GPU state before operations
  - `_ensure_standard_attention(self)` — [`L1036`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1036) — Ensure standard attention is active
  - `_generate_comprehensive_summary(self, performance_analysis: Dict[str, Any], correctness: float)` — [`L1279`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1279) — Generate comprehensive evaluation summary with safety info
  - `_get_comprehensive_error_statistics(self)` — [`L1321`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1321) — Get comprehensive error statistics
  - `_get_safe_benchmark_configs(self)` — [`L1008`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1008) — Get safer benchmark configurations for GPU protection
  - `_gpu_protected_apply_hook(self, custom_attention_class: Any)` — [`L924`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L924) — GPU-protected application of custom attention hook
  - `_gpu_protected_measure_baseline(self)` — [`L467`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L467) — GPU-protected baseline measurement with enhanced error handling
  - `_gpu_protected_remove_hook(self, original_attention: Any)` — [`L958`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L958) — GPU-protected removal of custom attention hook
  - `_memory_safe_correctness_test(self, custom_attention_class: Any)` — [`L544`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L544) — Memory-safe correctness testing with GPU protection
  - `_print_bulletproof_evaluation_results(self, result: Dict[str, Any])` — [`L1350`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1350) — Print comprehensive bulletproof evaluation results
  - `_remove_attention_hook_safely(self, original_attention: Any)` — [`L971`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L971) — Safely remove attention hook
  - `_reset_error_counters(self)` — [`L221`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L221) — Reset all error tracking counters
  - `_result_to_dict(self, result: BenchmarkResult)` — [`L1420`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1420) — Convert BenchmarkResult to dictionary
  - `_safe_calculate_improvement(self, new_value: float, old_value: float)` — [`L1209`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1209) — Safely calculate percentage improvement with bounds
  - `_static_validate_metal_kernel_syntax(self, program_text: str)` — [`L313`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L313) — Static analysis of Metal kernel syntax for common safety issues
  - `_store_enhanced_baseline_metrics(self, baseline_results: List[BenchmarkResult])` — [`L1047`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1047) — Store enhanced baseline metrics
  - `_test_single_sequence_memory_safe(self, custom_attention_class: Any, args: Any, x: Any, mask: Any)` — [`L686`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L686) — Test single sequence with enhanced memory safety
  - `_validate_custom_attention_class(self, custom_class: Any)` — [`L350`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L350) — Comprehensive validation of custom attention class
  - `_validate_metal_kernel_safety(self, custom_attention_class: Any)` — [`L373`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L373) — Pre-execution validation of Metal kernel safety
  - `evaluate(self, program_text: str)` — [`L105`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L105) — BULLETPROOF evaluation that handles ALL Metal kernel failures:
  - `baseline_metrics` — [`L92`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L92)
  - `baseline_results` — [`L93`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L93)
  - `benchmark_suite` — [`L96`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L96)
  - `gpu_resource_errors` — [`L81`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L81)
  - `kernel_validation_timeout` — [`L75`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L75)
  - `max_batch_size_safe` — [`L88`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L88)
  - `max_head_dimension_safe` — [`L89`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L89)
  - `max_retry_attempts` — [`L73`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L73)
  - `max_sequence_length_safe` — [`L87`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L87)
  - `metal_command_buffer_errors` — [`L78`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L78)
  - `metal_compilation_errors` — [`L80`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L80)
  - `metal_memory_violations` — [`L79`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L79)
  - `model_path` — [`L70`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L70)
  - `retry_attempts_used` — [`L84`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L84)
  - `retry_base_delay` — [`L74`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L74)
  - `successful_fallbacks` — [`L83`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L83)
  - `total_metal_errors` — [`L82`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L82)
- protocol/private: `__init__`[`L69`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L69)
- uses (calls/refs, reference-scoped): (16 test-only callers)
- used by: (3 test-only callers)

### `GPUCommandBufferError`  ·  implements/extends Exception
- def: [`examples/mlx_metal_kernel_opt/evaluator.py:54`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L54)
- doc: GPU command buffer execution error
- signature: `class GPUCommandBufferError(Exception):`
- used by: (1 test-only callers)

### `MetalKernelSafetyError`  ·  implements/extends Exception
- def: [`examples/mlx_metal_kernel_opt/evaluator.py:48`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L48)
- doc: Metal kernel safety violation
- signature: `class MetalKernelSafetyError(Exception):`
- used by: (1 test-only callers)

### `MetalMemoryViolationError`  ·  implements/extends Exception
- def: [`examples/mlx_metal_kernel_opt/evaluator.py:60`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L60)
- doc: Metal kernel memory access violation
- signature: `class MetalMemoryViolationError(Exception):`

### `MockArgs`
- def: [`examples/mlx_metal_kernel_opt/evaluator.py:550`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L550)
- signature: `class MockArgs:`
- members:
  - `head_dim` — [`L385`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L385)
  - `head_dim` — [`L555`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L555)
  - `hidden_size` — [`L382`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L382)
  - `hidden_size` — [`L552`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L552)
  - `max_position_embeddings` — [`L389`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L389)
  - `max_position_embeddings` — [`L559`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L559)
  - `num_attention_heads` — [`L383`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L383)
  - `num_attention_heads` — [`L553`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L553)
  - `num_key_value_heads` — [`L384`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L384)
  - `num_key_value_heads` — [`L554`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L554)
  - `rms_norm_eps` — [`L386`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L386)
  - `rms_norm_eps` — [`L556`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L556)
  - `rope_scaling` — [`L388`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L388)
  - `rope_scaling` — [`L558`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L558)
  - `rope_theta` — [`L387`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L387)
  - `rope_theta` — [`L557`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L557)
- uses (calls/refs, reference-scoped): (10 test-only callers)

## Functions
- `evaluate(program_text: str)` — [`L1432`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1432) — 🛡️ BULLETPROOF evaluation function called by OpenEvolve
- `test_bulletproof_evaluator()` — [`L1438`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/evaluator.py#L1438) — Test the bulletproof Metal kernel evaluator

