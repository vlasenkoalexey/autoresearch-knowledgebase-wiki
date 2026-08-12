---
title: 'Module: packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py'
type: catalog
provenance: extracted
module: packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py
status: fresh
symbol_base: scip-python python prime-agent 0.0.0 `packages.coding-agent.skills.attach-image.src.attach_image.attach_image`/
symbols:
  _resize_image: _resize_image().
  _validate_image: _validate_image().
  _load_image_for_attachment: _load_image_for_attachment().
  _emit_attachment: _emit_attachment().
  run: run().
  _MAX_ATTACHMENT_DATA_CHARS: _MAX_ATTACHMENT_DATA_CHARS.
  _detect_image_mime: _detect_image_mime().
  _base64_chars: _base64_chars().
  _MAX_SOURCE_IMAGE_BYTES: _MAX_SOURCE_IMAGE_BYTES.
  _MAX_SOURCE_IMAGE_PIXELS: _MAX_SOURCE_IMAGE_PIXELS.
  _MAX_ATTACHMENT_DIMENSION: _MAX_ATTACHMENT_DIMENSION.
  _TRANSPARENCY_BACKGROUND: _TRANSPARENCY_BACKGROUND.
  _ATTACHMENT_DISPLAY_MIME: _ATTACHMENT_DISPLAY_MIME.
  _JPEG_QUALITIES: _JPEG_QUALITIES.
  _IMAGE_SIGNATURES: _IMAGE_SIGNATURES.
  _image_dimensions: _image_dimensions().
  _validate_decodable_image: _validate_decodable_image().
  _encode_jpeg: _encode_jpeg().
---
# Module: [`packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py)

## Functions
- `_base64_chars(data: bytes)` — [`L103`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L103)
- `_detect_image_mime(data: bytes)` — [`L30`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L30)
- `_emit_attachment(filepath: Path, mime_type: str, size: int, dimensions: tuple[int, int])` — [`L194`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L194)
- `_encode_jpeg(image, quality: int)` — [`L131`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L131)
- `_image_dimensions(filepath: Path)` — [`L39`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L39)
- `_load_image_for_attachment(data: bytes)` — [`L107`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L107)
- `_resize_image(filepath: Path, mime_type: str, size: int, dimensions: tuple[int, int])` — [`L137`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L137)
- `_validate_decodable_image(filepath: Path)` — [`L56`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L56)
- `_validate_image(path: str)` — [`L70`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L70)
- `run(*paths: str)` — [`L208`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L208) — Load one or more on-disk images into the model's context as attachments.

## Module values
- `_ATTACHMENT_DISPLAY_MIME` — [`L10`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L10)
- `_IMAGE_SIGNATURES` — [`L22`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L22)
- `_JPEG_QUALITIES` — [`L19`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L19)
- `_MAX_ATTACHMENT_DATA_CHARS` — [`L16`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L16)
- `_MAX_ATTACHMENT_DIMENSION` — [`L17`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L17)
- `_MAX_SOURCE_IMAGE_BYTES` — [`L14`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L14)
- `_MAX_SOURCE_IMAGE_PIXELS` — [`L15`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L15)
- `_TRANSPARENCY_BACKGROUND` — [`L18`](../../../../../../../../../../raw/code/prime-agent/packages/coding-agent/skills/attach-image/src/attach_image/attach_image.py#L18)

