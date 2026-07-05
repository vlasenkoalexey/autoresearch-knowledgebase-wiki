---
title: 'Module: test/notebook/testfiles/main2.py'
type: catalog
provenance: extracted
module: test/notebook/testfiles/main2.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.notebook.testfiles.main2`/
symbols:
  DEBUG: DEBUG.
  main.CactusDataset.__getitem__: main().CactusDataset#__getitem__().
  main: main().
  main.EfficientNetB0_4ch.forward: main().EfficientNetB0_4ch#forward().
  parser: parser.
  main.set_requires_grad: main().set_requires_grad().
  args: args.
  main.load_img_as_numpy_with_mask: main().load_img_as_numpy_with_mask().
  main.get_transforms: main().get_transforms().
  main.CactusDataset: main().CactusDataset#
  CactusDataset._cache: CactusDataset#_cache.
  main.CactusDataset.__len__: main().CactusDataset#__len__().
  CactusDataset.img_ids: CactusDataset#img_ids.
  CactusDataset.labels: CactusDataset#labels.
  CactusDataset.cache: CactusDataset#cache.
  main.EfficientNetB0_4ch: main().EfficientNetB0_4ch#
  seed_everything: seed_everything().
  main.green_mask: main().green_mask().
  CactusDataset.img_dir: CactusDataset#img_dir.
  CactusDataset.transform: CactusDataset#transform.
  EfficientNetB0_4ch.features: EfficientNetB0_4ch#features.
  EfficientNetB0_4ch.avgpool: EfficientNetB0_4ch#avgpool.
  EfficientNetB0_4ch.head: EfficientNetB0_4ch#head.
  main.CactusDataset.__init__: main().CactusDataset#__init__().
  main.EfficientNetB0_4ch.__init__: main().EfficientNetB0_4ch#__init__().
---
# Module: [`test/notebook/testfiles/main2.py`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py)

## Classes
### `CactusDataset`
- def: [`test/notebook/testfiles/main2.py:166`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L166)
- signature: `class CactusDataset(Dataset):`
- members:
  - `cache` — [`L172`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L172)
  - `img_dir` — [`L169`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L169)
  - `img_ids` — [`L168`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L168)
  - `labels` — [`L170`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L170)
  - `transform` — [`L171`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L171)
- protocol/private: `__getitem__`[`L176`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L176), `__init__`[`L167`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L167), `__len__`[`L174`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L174), `_cache`[`L173`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L173)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `EfficientNetB0_4ch`
- def: [`test/notebook/testfiles/main2.py:231`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L231)
- signature: `class EfficientNetB0_4ch(nn.Module):`
- members:
  - `forward(self, x)` — [`L255`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L255)
  - `avgpool` — [`L249`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L249)
  - `features` — [`L248`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L248)
  - `head` — [`L251`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L251)
- protocol/private: `__init__`[`L232`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L232)
- used by: (1 test-only callers)

## Functions
- `get_transforms(mode='train')` — [`L138`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L138)
- `green_mask(img_bgr)` — [`L109`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L109)
- `load_img_as_numpy_with_mask(filepath)` — [`L117`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L117)
- `main()` — [`L37`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L37)
- `seed_everything(seed=42)` — [`L30`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L30)
- `set_requires_grad(modules, req)` — [`L294`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L294)

## Module values
- `DEBUG` — [`L25`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L25)
- `args` — [`L24`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L24)
- `parser` — [`L22`](../../../../../../../raw/code/rd-agent/test/notebook/testfiles/main2.py#L22)

