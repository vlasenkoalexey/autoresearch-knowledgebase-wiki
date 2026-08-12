---
title: 'Module: src/arc3/vision.py'
type: catalog
provenance: extracted
module: src/arc3/vision.py
status: fresh
symbol_base: scip-python python Retrodict 0.0.0 `src.arc3.vision`/
symbols:
  describe_opening: describe_opening().
  render_board_png: render_board_png().
  PROMPT: PROMPT.
  PALETTE: PALETTE.
---
# Module: [`src/arc3/vision.py`](../../../../../../raw/code/Retrodict/src/arc3/vision.py)

## Functions
- `describe_opening(board: list[list[int]], *, model: str = "gpt-5.5", api_key: str | None = None)` — [`L44`](../../../../../../raw/code/Retrodict/src/arc3/vision.py#L44) — Render the board and ask an OpenAI vision model to describe it. Returns (description, png_bytes).
- `render_board_png(board: list[list[int]], *, cell: int = 12)` — [`L30`](../../../../../../raw/code/Retrodict/src/arc3/vision.py#L30) — Render a 2-D grid of colour indices to a nearest-neighbour PNG (the game's own look).

## Module values
- `PALETTE` — [`L17`](../../../../../../raw/code/Retrodict/src/arc3/vision.py#L17)
- `PROMPT` — [`L24`](../../../../../../raw/code/Retrodict/src/arc3/vision.py#L24)

