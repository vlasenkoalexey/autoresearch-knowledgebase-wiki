---
title: 'Module: ai_scientist/ideas/i_cant_believe_its_not_better.py'
type: catalog
provenance: extracted
module: ai_scientist/ideas/i_cant_believe_its_not_better.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.ideas.i_cant_believe_its_not_better`/
symbols:
  test_accuracy: test_accuracy.
  checkpoint_path: checkpoint_path.
  loss: loss.
  model: model.
  val_accuracy: val_accuracy.
  final_checkpoint_path: final_checkpoint_path.
  labels: labels.
  seconds: seconds.
  train_accuracy: train_accuracy.
  train_loader: train_loader.
  optimizer: optimizer.
  outputs: outputs.
  metrics: metrics.
  scheduler: scheduler.
  checkpoint_dir: checkpoint_dir.
  device: device.
  train_dataset: train_dataset.
  val_dataset: val_dataset.
  test_dataset: test_dataset.
  val_loader: val_loader.
  test_loader: test_loader.
  epoch_time: epoch_time.
  log_file: log_file.
  avg_loss: avg_loss.
  perf_string: perf_string.
  similarity_score: similarity_score.
  epoch: epoch.
  pipe: pipe.
  transform: transform.
  total_time: total_time.
  embed: embed.
  HuggingFaceImageNet.__getitem__: HuggingFaceImageNet#__getitem__().
  step: step.
  start_time: start_time.
  NUM_EPOCHS: NUM_EPOCHS.
  image_real: image_real.
  image_gen: image_gen.
  weights: weights.
  train_dataset_hf: train_dataset_hf.
  val_dataset_hf: val_dataset_hf.
  test_dataset_hf: test_dataset_hf.
  elapsed: elapsed.
  epoch_elapsed: epoch_elapsed.
  hours: hours.
  minutes: minutes.
  e: e.
  BATCH_SIZE: BATCH_SIZE.
  NUM_WORKERS: NUM_WORKERS.
  NUM_TEST_BATCHES: NUM_TEST_BATCHES.
  DATASET: DATASET.
  WARMUP_EPOCHS: WARMUP_EPOCHS.
  HuggingFaceImageNet: HuggingFaceImageNet#
  calculate_accuracy: calculate_accuracy().
  epoch_start_time: epoch_start_time.
  running_loss: running_loss.
  images: images.
  HuggingFaceImageNet.__len__: HuggingFaceImageNet#__len__().
  img_urls: img_urls.
  IMAGE_SIZE: IMAGE_SIZE.
  DATASET_NAME: DATASET_NAME.
  STEPS_TO_LOG: STEPS_TO_LOG.
  HuggingFaceImageNet.hf_dataset: HuggingFaceImageNet#hf_dataset.
  HuggingFaceImageNet.transform: HuggingFaceImageNet#transform.
  timestamp: timestamp.
  best_val_accuracy: best_val_accuracy.
  feature_extractor: feature_extractor.
  text: text.
  WEIGHT_DECAY: WEIGHT_DECAY.
  criterion: criterion.
  GRAD_CLIP_NORM: GRAD_CLIP_NORM.
  medmnist: medmnist.
  eurosat: eurosat.
  mnist: mnist.
  fashion_mnist: fashion_mnist.
  cifar: cifar.
  imdb: imdb.
  amazon_polarity: amazon_polarity.
  emotion: emotion.
  silicone: silicone.
  math_examples: math_examples.
  LEARNING_RATE: LEARNING_RATE.
  HuggingFaceImageNet.__init__: HuggingFaceImageNet#__init__().
---
# Module: [`ai_scientist/ideas/i_cant_believe_its_not_better.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py)

## Classes
### `HuggingFaceImageNet`
- def: [`ai_scientist/ideas/i_cant_believe_its_not_better.py:175`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L175) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- signature: `class HuggingFaceImageNet(torch.utils.data.Dataset):`
- members:
  - `hf_dataset` — [`L177`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L177)
  - `transform` — [`L178`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L178)
- protocol/private: `__getitem__`[`L183`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L183), `__init__`[`L176`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L176), `__len__`[`L180`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L180)
- used by: [`test_dataset`](i_cant_believe_its_not_better.md#test_dataset), [`train_dataset`](i_cant_believe_its_not_better.md#train_dataset), [`val_dataset`](i_cant_believe_its_not_better.md#val_dataset)

## Functions
- `calculate_accuracy(model, data_loader, device, max_batches=None)` — [`L267`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L267) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)

## Module values
- `BATCH_SIZE` — [`L129`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L129) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `DATASET` — [`L138`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L138) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `DATASET_NAME` — [`L134`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L134) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `GRAD_CLIP_NORM` — [`L263`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L263) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `IMAGE_SIZE` — [`L132`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L132) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `LEARNING_RATE` — [`L130`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L130)
- `NUM_EPOCHS` — [`L135`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L135) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `NUM_TEST_BATCHES` — [`L137`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L137) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `NUM_WORKERS` — [`L133`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L133) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `STEPS_TO_LOG` — [`L136`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L136) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `WARMUP_EPOCHS` — [`L139`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L139) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `WEIGHT_DECAY` — [`L131`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L131) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `amazon_polarity` — [`L54`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L54)
- `avg_loss` — [`L327`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L327) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `best_val_accuracy` — [`L301`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L301) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `checkpoint_dir` — [`L286`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L286) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `checkpoint_path` — [`L367`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L367) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `cifar` — [`L44`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L44)
- `criterion` — [`L234`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L234) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `device` — [`L83`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L83) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `e` — [`L231`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L231)
- `elapsed` — [`L325`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L325) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `embed` — [`L121`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L121)
- `emotion` — [`L59`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L59)
- `epoch` — [`L302`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L302) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `epoch_elapsed` — [`L326`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L326) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `epoch_start_time` — [`L303`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L303)
- `epoch_time` — [`L388`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L388)
- `eurosat` — [`L29`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L29)
- `fashion_mnist` — [`L39`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L39)
- `feature_extractor` — [`L116`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L116)
- `final_checkpoint_path` — [`L403`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L403) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `hours` — [`L394`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L394)
- `image_gen` — [`L95`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L95) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `image_real` — [`L94`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L94) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `images` — [`L306`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L306) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `imdb` — [`L49`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L49)
- `img_urls` — [`L90`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L90) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `labels` — [`L306`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L306) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `log_file` — [`L285`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L285) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `loss` — [`L312`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L312) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `math_examples` — [`L69`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L69)
- `medmnist` — [`L24`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L24)
- `metrics` — [`L290`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L290) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `minutes` — [`L395`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L395)
- `mnist` — [`L34`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L34)
- `model` — [`L223`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L223) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `optimizer` — [`L237`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L237) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `outputs` — [`L96`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L96) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `perf_string` — [`L365`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L365) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `pipe` — [`L84`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L84) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `running_loss` — [`L304`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L304) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `scheduler` — [`L247`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L247) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `seconds` — [`L396`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L396)
- `silicone` — [`L64`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L64)
- `similarity_score` — [`L97`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L97)
- `start_time` — [`L226`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L226)
- `step` — [`L306`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L306) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `test_accuracy` — [`L335`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L335) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `test_dataset` — [`L195`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L195) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `test_dataset_hf` — [`L167`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L167) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `test_loader` — [`L214`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L214) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `text` — [`L119`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L119)
- `timestamp` — [`L284`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L284) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `total_time` — [`L393`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L393)
- `train_accuracy` — [`L329`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L329) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `train_dataset` — [`L193`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L193) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `train_dataset_hf` — [`L155`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L155) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `train_loader` — [`L198`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L198) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `transform` — [`L141`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L141) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `val_accuracy` — [`L332`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L332) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `val_dataset` — [`L194`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L194) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `val_dataset_hf` — [`L161`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L161) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `val_loader` — [`L206`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L206) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)
- `weights` — [`L149`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_better.py#L149) — documented in [ai_scientist-ideas-i_cant_believe_its_not_better](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md)

