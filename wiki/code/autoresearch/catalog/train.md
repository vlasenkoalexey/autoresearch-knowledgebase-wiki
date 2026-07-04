---
title: 'Module: train.py'
type: catalog
provenance: extracted
module: train.py
status: fresh
symbol_base: scip-python python autoresearch 0.0.0 train/
symbols:
  build_model_config: build_model_config().
  CausalSelfAttention.forward: CausalSelfAttention#forward().
  remaining: remaining.
  peak_vram_mb: peak_vram_mb.
  model: model.
  GPT.forward: GPT#forward().
  group: group.
  optimizer: optimizer.
  GPT.init_weights: GPT#init_weights().
  GPT.setup_optimizer: GPT#setup_optimizer().
  MuonAdamW._step_adamw: MuonAdamW#_step_adamw().
  dt: dt.
  fa3: fa3.
  GPT.estimate_flops: GPT#estimate_flops().
  train_loss: train_loss.
  CausalSelfAttention.head_dim: CausalSelfAttention#head_dim.
  GPT.transformer: GPT#transformer.
  GPT.num_scaling_params: GPT#num_scaling_params().
  MuonAdamW._step_muon: MuonAdamW#_step_muon().
  steady_state_mfu: steady_state_mfu.
  tokens_per_fwdbwd: tokens_per_fwdbwd.
  train_loader: train_loader.
  loss: loss.
  step: step.
  mfu: mfu.
  total_tokens: total_tokens.
  val_bpb: val_bpb.
  num_flops_per_token: num_flops_per_token.
  ema_beta: ema_beta.
  GPT.value_embeds: GPT#value_embeds.
  vocab_size: vocab_size.
  config: config.
  epoch: epoch.
  CausalSelfAttention.c_q: CausalSelfAttention#c_q.
  CausalSelfAttention.c_k: CausalSelfAttention#c_k.
  CausalSelfAttention.c_v: CausalSelfAttention#c_v.
  CausalSelfAttention.ve_gate: CausalSelfAttention#ve_gate.
  get_lr_multiplier: get_lr_multiplier().
  debiased_smooth_loss: debiased_smooth_loss.
  value: value.
  CausalSelfAttention.n_kv_head: CausalSelfAttention#n_kv_head.
  GPT.config: GPT#config.
  tokenizer: tokenizer.
  grad_accum_steps: grad_accum_steps.
  progress: progress.
  train_loss_f: train_loss_f.
  Block.forward: Block#forward().
  CausalSelfAttention.n_embd: CausalSelfAttention#n_embd.
  GPT.rotary_seq_len: GPT#rotary_seq_len.
  param_counts: param_counts.
  total_training_time: total_training_time.
  lrm: lrm.
  norm: norm().
  CausalSelfAttention.n_head: CausalSelfAttention#n_head.
  GPT.sin: GPT#sin.
  MuonAdamW.step: MuonAdamW#step().
  TOTAL_BATCH_SIZE: TOTAL_BATCH_SIZE.
  muon_momentum: muon_momentum.
  muon_weight_decay: muon_weight_decay.
  tok_per_sec: tok_per_sec.
  MLP.forward: MLP#forward().
  GPT.resid_lambdas: GPT#resid_lambdas.
  GPT.x0_lambdas: GPT#x0_lambdas.
  startup_time: startup_time.
  micro_step: micro_step.
  GPT.window_sizes: GPT#window_sizes.
  GPT._precompute_rotary_embeddings: GPT#_precompute_rotary_embeddings().
  GPT.lm_head: GPT#lm_head.
  HEAD_DIM: HEAD_DIM.
  repo: repo.
  CausalSelfAttention.c_proj: CausalSelfAttention#c_proj.
  Block.attn: Block#attn.
  Block.mlp: Block#mlp.
  muon_step_fused: muon_step_fused().
  num_params: num_params.
  get_weight_decay: get_weight_decay().
  pct_done: pct_done.
  WARMUP_RATIO: WARMUP_RATIO.
  DEVICE_BATCH_SIZE: DEVICE_BATCH_SIZE.
  smooth_train_loss: smooth_train_loss.
  has_ve: has_ve().
  apply_rotary_emb: apply_rotary_emb().
  CausalSelfAttention.ve_gate_channels: CausalSelfAttention#ve_gate_channels.
  GPT.cos: GPT#cos.
  polar_express_coeffs: polar_express_coeffs.
  MuonAdamW._adamw_step_t: MuonAdamW#_adamw_step_t.
  MuonAdamW._adamw_lr_t: MuonAdamW#_adamw_lr_t.
  MuonAdamW._adamw_beta1_t: MuonAdamW#_adamw_beta1_t.
  MuonAdamW._adamw_beta2_t: MuonAdamW#_adamw_beta2_t.
  MuonAdamW._adamw_eps_t: MuonAdamW#_adamw_eps_t.
  MuonAdamW._adamw_wd_t: MuonAdamW#_adamw_wd_t.
  MuonAdamW._muon_momentum_t: MuonAdamW#_muon_momentum_t.
  MuonAdamW._muon_lr_t: MuonAdamW#_muon_lr_t.
  MuonAdamW._muon_wd_t: MuonAdamW#_muon_wd_t.
  MuonAdamW._muon_beta2_t: MuonAdamW#_muon_beta2_t.
  WEIGHT_DECAY: WEIGHT_DECAY.
  WARMDOWN_RATIO: WARMDOWN_RATIO.
  DEPTH: DEPTH.
  t_start: t_start.
  autocast_ctx: autocast_ctx.
  H100_BF16_PEAK_FLOPS: H100_BF16_PEAK_FLOPS.
  x: x.
  y: y.
  cap: cap.
  GPTConfig: GPTConfig#
  GPTConfig.sequence_len: GPTConfig#sequence_len.
  GPTConfig.vocab_size: GPTConfig#vocab_size.
  GPTConfig.n_layer: GPTConfig#n_layer.
  GPTConfig.n_head: GPTConfig#n_head.
  GPTConfig.n_kv_head: GPTConfig#n_kv_head.
  GPTConfig.n_embd: GPTConfig#n_embd.
  GPTConfig.window_pattern: GPTConfig#window_pattern.
  CausalSelfAttention: CausalSelfAttention#
  MLP: MLP#
  MLP.c_fc: MLP#c_fc.
  MLP.c_proj: MLP#c_proj.
  Block: Block#
  GPT: GPT#
  GPT._compute_window_sizes: GPT#_compute_window_sizes().
  adamw_step_fused: adamw_step_fused().
  ASPECT_RATIO: ASPECT_RATIO.
  WINDOW_PATTERN: WINDOW_PATTERN.
  EMBEDDING_LR: EMBEDDING_LR.
  UNEMBEDDING_LR: UNEMBEDDING_LR.
  MATRIX_LR: MATRIX_LR.
  SCALAR_LR: SCALAR_LR.
  ADAM_BETAS: ADAM_BETAS.
  FINAL_LR_FRAC: FINAL_LR_FRAC.
  device: device.
  get_muon_momentum: get_muon_momentum().
  t_start_training: t_start_training.
  t0: t0.
  t1: t1.
  t_end: t_end.
  MuonAdamW: MuonAdamW#
  key: key.
  CausalSelfAttention.__init__: CausalSelfAttention#__init__().
  MLP.__init__: MLP#__init__().
  Block.__init__: Block#__init__().
  GPT.__init__: GPT#__init__().
  MuonAdamW.__init__: MuonAdamW#__init__().
---
# Module: [`train.py`](../../../../raw/code/autoresearch/train.py)

## Classes
### `Block`
- def: [`train.py:112`](../../../../raw/code/autoresearch/train.py#L112)
- signature: `class Block(nn.Module):`
- members:
  - `forward(self, x, ve, cos_sin, window_size)` — [`L118`](../../../../raw/code/autoresearch/train.py#L118)
  - `attn` — [`L115`](../../../../raw/code/autoresearch/train.py#L115)
  - `mlp` — [`L116`](../../../../raw/code/autoresearch/train.py#L116)
- protocol/private: `__init__`[`L113`](../../../../raw/code/autoresearch/train.py#L113)
- uses (calls/refs, reference-scoped): [`norm`](train.md#norm), [`CausalSelfAttention`](train.md#CausalSelfAttention), [`MLP`](train.md#MLP)
- used by: [`transformer`](train.md#GPT.transformer)

### `CausalSelfAttention`
- def: [`train.py:61`](../../../../raw/code/autoresearch/train.py#L61)
- signature: `class CausalSelfAttention(nn.Module):`
- members:
  - `forward(self, x, ve, cos_sin, window_size)` — [`L77`](../../../../raw/code/autoresearch/train.py#L77) — documented in [train](../concepts/train.md)
  - `c_k` — [`L71`](../../../../raw/code/autoresearch/train.py#L71) — documented in [train](../concepts/train.md)
  - `c_proj` — [`L73`](../../../../raw/code/autoresearch/train.py#L73)
  - `c_q` — [`L70`](../../../../raw/code/autoresearch/train.py#L70) — documented in [train](../concepts/train.md)
  - `c_v` — [`L72`](../../../../raw/code/autoresearch/train.py#L72) — documented in [train](../concepts/train.md)
  - `head_dim` — [`L67`](../../../../raw/code/autoresearch/train.py#L67) — documented in [train](../concepts/train.md)
  - `n_embd` — [`L66`](../../../../raw/code/autoresearch/train.py#L66)
  - `n_head` — [`L64`](../../../../raw/code/autoresearch/train.py#L64) — documented in [train](../concepts/train.md)
  - `n_kv_head` — [`L65`](../../../../raw/code/autoresearch/train.py#L65) — documented in [train](../concepts/train.md)
  - `ve_gate` — [`L75`](../../../../raw/code/autoresearch/train.py#L75) — documented in [train](../concepts/train.md)
  - `ve_gate_channels` — [`L74`](../../../../raw/code/autoresearch/train.py#L74)
- protocol/private: `__init__`[`L62`](../../../../raw/code/autoresearch/train.py#L62)
- uses (calls/refs, reference-scoped): [`fa3`](train.md#fa3), [`norm`](train.md#norm), [`apply_rotary_emb`](train.md#apply_rotary_emb), [`has_ve`](train.md#has_ve)
- used by: [`attn`](train.md#Block.attn)

### `GPT`
- def: [`train.py:124`](../../../../raw/code/autoresearch/train.py#L124)
- signature: `class GPT(nn.Module):`
- members:
  - `estimate_flops(self)` — [`L208`](../../../../raw/code/autoresearch/train.py#L208) — Estimated FLOPs per token (forward + backward). — documented in [train](../concepts/train.md)
  - `forward(self, idx, targets=None, reduction='mean')` — [`L268`](../../../../raw/code/autoresearch/train.py#L268)
  - `init_weights(self)` — [`L150`](../../../../raw/code/autoresearch/train.py#L150) — documented in [train](../concepts/train.md)
  - `num_scaling_params(self)` — [`L224`](../../../../raw/code/autoresearch/train.py#L224) — documented in [train](../concepts/train.md)
  - `setup_optimizer(self, unembedding_lr=0.004, embedding_lr=0.2, matrix_lr=0.02, weight_decay=0, adam_betas=(0.8, 0.95), scalar_lr=0.5)` — [`L236`](../../../../raw/code/autoresearch/train.py#L236)
  - `config` — [`L127`](../../../../raw/code/autoresearch/train.py#L127)
  - `cos` — [`L177`](../../../../raw/code/autoresearch/train.py#L177)
  - `lm_head` — [`L133`](../../../../raw/code/autoresearch/train.py#L133)
  - `resid_lambdas` — [`L134`](../../../../raw/code/autoresearch/train.py#L134)
  - `rotary_seq_len` — [`L144`](../../../../raw/code/autoresearch/train.py#L144)
  - `sin` — [`L177`](../../../../raw/code/autoresearch/train.py#L177)
  - `transformer` — [`L129`](../../../../raw/code/autoresearch/train.py#L129) — documented in [train](../concepts/train.md)
  - `value_embeds` — [`L139`](../../../../raw/code/autoresearch/train.py#L139)
  - `window_sizes` — [`L128`](../../../../raw/code/autoresearch/train.py#L128)
  - `x0_lambdas` — [`L135`](../../../../raw/code/autoresearch/train.py#L135)
- protocol/private: `__init__`[`L125`](../../../../raw/code/autoresearch/train.py#L125), `_compute_window_sizes`[`L195`](../../../../raw/code/autoresearch/train.py#L195), `_precompute_rotary_embeddings`[`L183`](../../../../raw/code/autoresearch/train.py#L183)
- uses (calls/refs, reference-scoped): [`norm`](train.md#norm), [`has_ve`](train.md#has_ve), [`Block`](train.md#Block), [`MuonAdamW`](train.md#MuonAdamW)
- used by: [`model`](train.md#model), [`optimizer`](train.md#optimizer), [`num_flops_per_token`](train.md#num_flops_per_token), [`param_counts`](train.md#param_counts)

### `GPTConfig`
- def: [`train.py:33`](../../../../raw/code/autoresearch/train.py#L33)
- signature: `class GPTConfig:`
- members:
  - `n_embd` — [`L39`](../../../../raw/code/autoresearch/train.py#L39)
  - `n_head` — [`L37`](../../../../raw/code/autoresearch/train.py#L37)
  - `n_kv_head` — [`L38`](../../../../raw/code/autoresearch/train.py#L38)
  - `n_layer` — [`L36`](../../../../raw/code/autoresearch/train.py#L36)
  - `sequence_len` — [`L34`](../../../../raw/code/autoresearch/train.py#L34)
  - `vocab_size` — [`L35`](../../../../raw/code/autoresearch/train.py#L35)
  - `window_pattern` — [`L40`](../../../../raw/code/autoresearch/train.py#L40)
- used by: [`build_model_config`](train.md#build_model_config)

### `MLP`
- def: [`train.py:99`](../../../../raw/code/autoresearch/train.py#L99)
- signature: `class MLP(nn.Module):`
- members:
  - `forward(self, x)` — [`L105`](../../../../raw/code/autoresearch/train.py#L105)
  - `c_fc` — [`L102`](../../../../raw/code/autoresearch/train.py#L102)
  - `c_proj` — [`L103`](../../../../raw/code/autoresearch/train.py#L103)
- protocol/private: `__init__`[`L100`](../../../../raw/code/autoresearch/train.py#L100)
- used by: [`mlp`](train.md#Block.mlp)

### `MuonAdamW`
- def: [`train.py:356`](../../../../raw/code/autoresearch/train.py#L356)
- members:
  - `step(self)` — [`L421`](../../../../raw/code/autoresearch/train.py#L421)
- protocol/private: `__init__`[`L359`](../../../../raw/code/autoresearch/train.py#L359), `_adamw_beta1_t`[`L364`](../../../../raw/code/autoresearch/train.py#L364), `_adamw_beta2_t`[`L365`](../../../../raw/code/autoresearch/train.py#L365), `_adamw_eps_t`[`L366`](../../../../raw/code/autoresearch/train.py#L366), `_adamw_lr_t`[`L363`](../../../../raw/code/autoresearch/train.py#L363), `_adamw_step_t`[`L362`](../../../../raw/code/autoresearch/train.py#L362), `_adamw_wd_t`[`L367`](../../../../raw/code/autoresearch/train.py#L367), `_muon_beta2_t`[`L371`](../../../../raw/code/autoresearch/train.py#L371), `_muon_lr_t`[`L369`](../../../../raw/code/autoresearch/train.py#L369), `_muon_momentum_t`[`L368`](../../../../raw/code/autoresearch/train.py#L368), `_muon_wd_t`[`L370`](../../../../raw/code/autoresearch/train.py#L370), `_step_adamw`[`L373`](../../../../raw/code/autoresearch/train.py#L373), `_step_muon`[`L394`](../../../../raw/code/autoresearch/train.py#L394)
- uses (calls/refs, reference-scoped): [`muon_step_fused`](train.md#muon_step_fused), [`adamw_step_fused`](train.md#adamw_step_fused)
- used by: [`group`](train.md#group), [`setup_optimizer`](train.md#GPT.setup_optimizer)

## Functions
- `adamw_step_fused(p, grad, exp_avg, exp_avg_sq, step_t, lr_t, beta1_t, beta2_t, eps_t, wd_t)` — [`L306`](../../../../raw/code/autoresearch/train.py#L306)
- `apply_rotary_emb(x, cos, sin)` — [`L52`](../../../../raw/code/autoresearch/train.py#L52)
- `build_model_config(depth)` — [`L469`](../../../../raw/code/autoresearch/train.py#L469) — documented in [train](../concepts/train.md)
- `get_lr_multiplier(progress)` — [`L518`](../../../../raw/code/autoresearch/train.py#L518) — documented in [train](../concepts/train.md)
- `get_muon_momentum(step)` — [`L527`](../../../../raw/code/autoresearch/train.py#L527)
- `get_weight_decay(progress)` — [`L531`](../../../../raw/code/autoresearch/train.py#L531)
- `has_ve(layer_idx, n_layer)` — [`L47`](../../../../raw/code/autoresearch/train.py#L47) — Returns True if layer should have Value Embedding (alternating, last always included).
- `muon_step_fused(stacked_grads, stacked_params, momentum_buffer, second_momentum_buffer, momentum_t, lr_t, wd_t, beta2_t, ns_steps, red_dim)` — [`L317`](../../../../raw/code/autoresearch/train.py#L317)
- `norm(x)` — [`L43`](../../../../raw/code/autoresearch/train.py#L43) — documented in [train](../concepts/train.md)

## Module values
- `ADAM_BETAS` — [`L444`](../../../../raw/code/autoresearch/train.py#L444)
- `ASPECT_RATIO` — [`L433`](../../../../raw/code/autoresearch/train.py#L433)
- `DEPTH` — [`L450`](../../../../raw/code/autoresearch/train.py#L450)
- `DEVICE_BATCH_SIZE` — [`L451`](../../../../raw/code/autoresearch/train.py#L451)
- `EMBEDDING_LR` — [`L439`](../../../../raw/code/autoresearch/train.py#L439)
- `FINAL_LR_FRAC` — [`L447`](../../../../raw/code/autoresearch/train.py#L447)
- `H100_BF16_PEAK_FLOPS` — [`L463`](../../../../raw/code/autoresearch/train.py#L463)
- `HEAD_DIM` — [`L434`](../../../../raw/code/autoresearch/train.py#L434) — documented in [train](../concepts/train.md)
- `MATRIX_LR` — [`L441`](../../../../raw/code/autoresearch/train.py#L441)
- `SCALAR_LR` — [`L442`](../../../../raw/code/autoresearch/train.py#L442)
- `TOTAL_BATCH_SIZE` — [`L438`](../../../../raw/code/autoresearch/train.py#L438) — documented in [train](../concepts/train.md)
- `UNEMBEDDING_LR` — [`L440`](../../../../raw/code/autoresearch/train.py#L440)
- `WARMDOWN_RATIO` — [`L446`](../../../../raw/code/autoresearch/train.py#L446)
- `WARMUP_RATIO` — [`L445`](../../../../raw/code/autoresearch/train.py#L445)
- `WEIGHT_DECAY` — [`L443`](../../../../raw/code/autoresearch/train.py#L443)
- `WINDOW_PATTERN` — [`L435`](../../../../raw/code/autoresearch/train.py#L435)
- `autocast_ctx` — [`L462`](../../../../raw/code/autoresearch/train.py#L462)
- `cap` — [`L21`](../../../../raw/code/autoresearch/train.py#L21)
- `config` — [`L479`](../../../../raw/code/autoresearch/train.py#L479) — documented in [train](../concepts/train.md)
- `debiased_smooth_loss` — [`L584`](../../../../raw/code/autoresearch/train.py#L584) — documented in [train](../concepts/train.md)
- `device` — [`L461`](../../../../raw/code/autoresearch/train.py#L461)
- `dt` — [`L576`](../../../../raw/code/autoresearch/train.py#L576) — documented in [train](../concepts/train.md)
- `ema_beta` — [`L582`](../../../../raw/code/autoresearch/train.py#L582) — documented in [train](../concepts/train.md)
- `epoch` — [`L511`](../../../../raw/code/autoresearch/train.py#L511)
- `fa3` — [`L24`](../../../../raw/code/autoresearch/train.py#L24) — documented in [train](../concepts/train.md)
- `grad_accum_steps` — [`L497`](../../../../raw/code/autoresearch/train.py#L497) — documented in [train](../concepts/train.md)
- `group` — [`L559`](../../../../raw/code/autoresearch/train.py#L559)
- `key` — [`L489`](../../../../raw/code/autoresearch/train.py#L489)
- `loss` — [`L548`](../../../../raw/code/autoresearch/train.py#L548)
- `lrm` — [`L556`](../../../../raw/code/autoresearch/train.py#L556) — documented in [train](../concepts/train.md)
- `mfu` — [`L587`](../../../../raw/code/autoresearch/train.py#L587) — documented in [train](../concepts/train.md)
- `micro_step` — [`L546`](../../../../raw/code/autoresearch/train.py#L546)
- `model` — [`L483`](../../../../raw/code/autoresearch/train.py#L483)
- `muon_momentum` — [`L557`](../../../../raw/code/autoresearch/train.py#L557)
- `muon_weight_decay` — [`L558`](../../../../raw/code/autoresearch/train.py#L558)
- `num_flops_per_token` — [`L492`](../../../../raw/code/autoresearch/train.py#L492)
- `num_params` — [`L491`](../../../../raw/code/autoresearch/train.py#L491)
- `optimizer` — [`L499`](../../../../raw/code/autoresearch/train.py#L499)
- `param_counts` — [`L487`](../../../../raw/code/autoresearch/train.py#L487)
- `pct_done` — [`L585`](../../../../raw/code/autoresearch/train.py#L585)
- `peak_vram_mb` — [`L619`](../../../../raw/code/autoresearch/train.py#L619) — documented in [train](../concepts/train.md)
- `polar_express_coeffs` — [`L297`](../../../../raw/code/autoresearch/train.py#L297)
- `progress` — [`L555`](../../../../raw/code/autoresearch/train.py#L555) — documented in [train](../concepts/train.md)
- `remaining` — [`L588`](../../../../raw/code/autoresearch/train.py#L588)
- `repo` — [`L23`](../../../../raw/code/autoresearch/train.py#L23)
- `smooth_train_loss` — [`L539`](../../../../raw/code/autoresearch/train.py#L539)
- `startup_time` — [`L617`](../../../../raw/code/autoresearch/train.py#L617)
- `steady_state_mfu` — [`L618`](../../../../raw/code/autoresearch/train.py#L618) — documented in [train](../concepts/train.md)
- `step` — [`L541`](../../../../raw/code/autoresearch/train.py#L541)
- `t0` — [`L545`](../../../../raw/code/autoresearch/train.py#L545)
- `t1` — [`L575`](../../../../raw/code/autoresearch/train.py#L575)
- `t_end` — [`L616`](../../../../raw/code/autoresearch/train.py#L616)
- `t_start` — [`L457`](../../../../raw/code/autoresearch/train.py#L457)
- `t_start_training` — [`L538`](../../../../raw/code/autoresearch/train.py#L538)
- `tok_per_sec` — [`L586`](../../../../raw/code/autoresearch/train.py#L586) — documented in [train](../concepts/train.md)
- `tokenizer` — [`L465`](../../../../raw/code/autoresearch/train.py#L465)
- `tokens_per_fwdbwd` — [`L495`](../../../../raw/code/autoresearch/train.py#L495) — documented in [train](../concepts/train.md)
- `total_tokens` — [`L608`](../../../../raw/code/autoresearch/train.py#L608) — documented in [train](../concepts/train.md)
- `total_training_time` — [`L540`](../../../../raw/code/autoresearch/train.py#L540) — documented in [train](../concepts/train.md)
- `train_loader` — [`L510`](../../../../raw/code/autoresearch/train.py#L510) — documented in [train](../concepts/train.md)
- `train_loss` — [`L549`](../../../../raw/code/autoresearch/train.py#L549)
- `train_loss_f` — [`L567`](../../../../raw/code/autoresearch/train.py#L567) — documented in [train](../concepts/train.md)
- `val_bpb` — [`L613`](../../../../raw/code/autoresearch/train.py#L613) — documented in [prepare](../concepts/prepare.md)
- `value` — [`L489`](../../../../raw/code/autoresearch/train.py#L489)
- `vocab_size` — [`L466`](../../../../raw/code/autoresearch/train.py#L466)
- `x` — [`L511`](../../../../raw/code/autoresearch/train.py#L511)
- `y` — [`L511`](../../../../raw/code/autoresearch/train.py#L511)

