---
title: 'Module: ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py'
type: catalog
provenance: extracted
module: ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.ideas.i_cant_believe_its_not_betterrealworld`/
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
  LEARNING_RATE: LEARNING_RATE.
  HuggingFaceImageNet.__init__: HuggingFaceImageNet#__init__().
---
# Module: [`ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py)

## Classes
### `HuggingFaceImageNet`
- def: [`ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py:143`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L143) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- signature: `class HuggingFaceImageNet(torch.utils.data.Dataset):`
- members:
  - `hf_dataset` — [`L145`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L145)
  - `transform` — [`L146`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L146)
- protocol/private: `__getitem__`[`L151`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L151), `__init__`[`L144`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L144), `__len__`[`L148`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L148)
- used by: [`test_dataset`](i_cant_believe_its_not_betterrealworld.md#test_dataset), [`train_dataset`](i_cant_believe_its_not_betterrealworld.md#train_dataset), [`val_dataset`](i_cant_believe_its_not_betterrealworld.md#val_dataset)

## Functions
- `calculate_accuracy(model, data_loader, device, max_batches=None)` — [`L235`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L235) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)

## Module values
- `BATCH_SIZE` — [`L97`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L97)
- `DATASET` — [`L106`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L106) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `DATASET_NAME` — [`L102`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L102) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `GRAD_CLIP_NORM` — [`L231`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L231)
- `IMAGE_SIZE` — [`L100`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L100) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `LEARNING_RATE` — [`L98`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L98)
- `NUM_EPOCHS` — [`L103`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L103)
- `NUM_TEST_BATCHES` — [`L105`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L105)
- `NUM_WORKERS` — [`L101`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L101)
- `STEPS_TO_LOG` — [`L104`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L104)
- `WARMUP_EPOCHS` — [`L107`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L107)
- `WEIGHT_DECAY` — [`L99`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L99)
- `avg_loss` — [`L295`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L295)
- `best_val_accuracy` — [`L269`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L269) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `checkpoint_dir` — [`L254`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L254)
- `checkpoint_path` — [`L335`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L335) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `criterion` — [`L202`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L202)
- `device` — [`L51`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L51)
- `e` — [`L199`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L199)
- `elapsed` — [`L293`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L293)
- `embed` — [`L89`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L89)
- `epoch` — [`L270`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L270)
- `epoch_elapsed` — [`L294`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L294)
- `epoch_start_time` — [`L271`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L271)
- `epoch_time` — [`L356`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L356)
- `feature_extractor` — [`L84`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L84)
- `final_checkpoint_path` — [`L371`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L371) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `hours` — [`L362`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L362)
- `image_gen` — [`L63`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L63)
- `image_real` — [`L62`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L62)
- `images` — [`L274`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L274)
- `img_urls` — [`L58`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L58)
- `labels` — [`L274`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L274)
- `log_file` — [`L253`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L253)
- `loss` — [`L280`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L280) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `metrics` — [`L258`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L258) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `minutes` — [`L363`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L363)
- `model` — [`L191`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L191) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `optimizer` — [`L205`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L205) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `outputs` — [`L64`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L64) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `perf_string` — [`L333`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L333)
- `pipe` — [`L52`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L52) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `running_loss` — [`L272`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L272)
- `scheduler` — [`L215`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L215) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `seconds` — [`L364`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L364)
- `similarity_score` — [`L65`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L65)
- `start_time` — [`L194`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L194)
- `step` — [`L274`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L274)
- `test_accuracy` — [`L303`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L303) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `test_dataset` — [`L163`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L163)
- `test_dataset_hf` — [`L135`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L135) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `test_loader` — [`L182`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L182)
- `text` — [`L87`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L87)
- `timestamp` — [`L252`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L252)
- `total_time` — [`L361`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L361)
- `train_accuracy` — [`L297`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L297) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `train_dataset` — [`L161`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L161) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `train_dataset_hf` — [`L123`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L123) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `train_loader` — [`L166`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L166)
- `transform` — [`L109`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L109)
- `val_accuracy` — [`L300`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L300) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `val_dataset` — [`L162`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L162)
- `val_dataset_hf` — [`L129`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L129) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)
- `val_loader` — [`L174`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L174)
- `weights` — [`L117`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/ideas/i_cant_believe_its_not_betterrealworld.py#L117) — documented in [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](../../../concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md)

