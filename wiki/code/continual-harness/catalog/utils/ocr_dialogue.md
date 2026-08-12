---
title: 'Module: utils/ocr_dialogue.py'
type: catalog
provenance: extracted
module: utils/ocr_dialogue.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.ocr_dialogue`/
symbols:
  OCRDialogueDetector.detect_dialogue_from_screenshot: OCRDialogueDetector#detect_dialogue_from_screenshot().
  logger: logger.
  OCRDialogueDetector.is_dialogue_box_visible: OCRDialogueDetector#is_dialogue_box_visible().
  create_ocr_detector: create_ocr_detector().
  OCRDialogueDetector._create_dialogue_color_mask: OCRDialogueDetector#_create_dialogue_color_mask().
  OCRDialogueDetector.debug_color_detection: OCRDialogueDetector#debug_color_detection.
  OCRDialogueDetector.get_stable_dialogue_text: OCRDialogueDetector#get_stable_dialogue_text().
  OCRDialogueDetector._extract_text_from_full_frame: OCRDialogueDetector#_extract_text_from_full_frame().
  OCRDialogueDetector._validate_and_clean_text: OCRDialogueDetector#_validate_and_clean_text().
  OCRDialogueDetector.detect_all_text_regions: OCRDialogueDetector#detect_all_text_regions().
  OCRDialogueDetector.update_dialogue_colors_from_analysis: OCRDialogueDetector#update_dialogue_colors_from_analysis().
  OCRDialogueDetector.test_dialogue_box_detection: OCRDialogueDetector#test_dialogue_box_detection().
  OCR_AVAILABLE: OCR_AVAILABLE.
  OCRDialogueDetector.analyze_dialogue_colors: OCRDialogueDetector#analyze_dialogue_colors().
  OCRDialogueDetector.enable_color_debug: OCRDialogueDetector#enable_color_debug().
  OCRDialogueDetector._preprocess_full_frame_for_ocr: OCRDialogueDetector#_preprocess_full_frame_for_ocr().
  OCRDialogueDetector._extract_text_from_region: OCRDialogueDetector#_extract_text_from_region().
  OCRDialogueDetector._preprocess_for_ocr: OCRDialogueDetector#_preprocess_for_ocr().
  OCRDialogueDetector.DIALOGUE_BOX_COORDS: OCRDialogueDetector#DIALOGUE_BOX_COORDS.
  OCRDialogueDetector.DIALOGUE_TEXT_COLORS: OCRDialogueDetector#DIALOGUE_TEXT_COLORS.
  OCRDialogueDetector._is_random_nonsense: OCRDialogueDetector#_is_random_nonsense().
  OCRDialogueDetector.OCR_TEXT_COORDS: OCRDialogueDetector#OCR_TEXT_COORDS.
  OCRDialogueDetector.stable_text_count: OCRDialogueDetector#stable_text_count.
  OCRDialogueDetector.print_color_analysis: OCRDialogueDetector#print_color_analysis().
  OCRDialogueDetector.analyze_dialogue_box_background: OCRDialogueDetector#analyze_dialogue_box_background().
  OCRDialogueDetector: OCRDialogueDetector#
  OCRDialogueDetector.last_detected_text: OCRDialogueDetector#last_detected_text.
  OCRDialogueDetector._clean_full_frame_text: OCRDialogueDetector#_clean_full_frame_text().
  OCRDialogueDetector.COLOR_TOLERANCE: OCRDialogueDetector#COLOR_TOLERANCE.
  OCRDialogueDetector.BATTLE_TEXT_COORDS: OCRDialogueDetector#BATTLE_TEXT_COORDS.
  OCRDialogueDetector.text_stability_threshold: OCRDialogueDetector#text_stability_threshold.
  OCRDialogueDetector.use_full_frame_scan: OCRDialogueDetector#use_full_frame_scan.
  OCRDialogueDetector.skip_dialogue_box_detection: OCRDialogueDetector#skip_dialogue_box_detection.
  OCRDialogueDetector._has_valid_letter_pattern: OCRDialogueDetector#_has_valid_letter_pattern().
  OCRDialogueDetector.DIALOGUE_BOX_BACKGROUND_COLORS: OCRDialogueDetector#DIALOGUE_BOX_BACKGROUND_COLORS.
  OCRDialogueDetector.DIALOGUE_BOX_BACKGROUND_THRESHOLD: OCRDialogueDetector#DIALOGUE_BOX_BACKGROUND_THRESHOLD.
  OCRDialogueDetector.__init__: OCRDialogueDetector#__init__().
---
# Module: [`utils/ocr_dialogue.py`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py)

## Classes
### `OCRDialogueDetector`
- def: [`utils/ocr_dialogue.py:22`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L22)
- doc: OCR-based dialogue detection for Pokemon Emerald
- signature: `class OCRDialogueDetector:`
- members:
  - `_clean_full_frame_text(self, raw_text: str)` — [`L234`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L234) — Clean and validate text extracted from full frame
  - `_create_dialogue_color_mask(self, image: np.ndarray)` — [`L389`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L389) — Create binary mask for pixels matching Pokemon dialogue text colors
  - `_extract_text_from_full_frame(self, screenshot: Image.Image)` — [`L171`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L171) — Extract text from the entire screenshot using OCR
  - `_extract_text_from_region(self, image_np: np.ndarray, coords: dict)` — [`L334`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L334) — Extract text from a specific region of the image
  - `_has_valid_letter_pattern(self, word: str)` — [`L956`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L956) — Check if word has valid English-like letter patterns
  - `_is_random_nonsense(self, text: str)` — [`L885`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L885) — Comprehensive detection of random letter sequences and nonsense text.
  - `_preprocess_for_ocr(self, roi: np.ndarray)` — [`L354`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L354) — Preprocess image region using Pokemon-specific dialogue color matching
  - `_preprocess_full_frame_for_ocr(self, image_np: np.ndarray)` — [`L207`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L207) — Preprocess entire frame using Pokemon-specific dialogue color matching
  - `_validate_and_clean_text(self, text: str)` — [`L859`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L859) — Validate and clean detected text
  - `analyze_dialogue_box_background(self, screenshot: Image.Image)` — [`L752`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L752) — Analyze dialogue box region to find actual background colors.
  - `analyze_dialogue_colors(self, screenshot: Image.Image)` — [`L618`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L618) — Analyze a screenshot to find the actual colors used in the dialogue box.
  - `detect_all_text_regions(self, screenshot: Image.Image)` — [`L283`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L283) — Detect all text regions in the screenshot with their locations
  - `detect_dialogue_from_screenshot(self, screenshot: Image.Image)` — [`L113`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L113) — Detect dialogue text from Pokemon Emerald dialogue regions only.
  - `enable_color_debug(self, enabled: bool = True)` — [`L610`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L610) — Enable/disable color detection debugging
  - `get_stable_dialogue_text(self, screenshot: Image.Image)` — [`L994`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L994) — Get dialogue text that has been stable across multiple frames.
  - `is_dialogue_box_visible(self, screenshot: Image.Image)` — [`L422`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L422) — Check if a dialogue box is actually visible by looking for green horizontal border lines.
  - `print_color_analysis(self, screenshot: Image.Image)` — [`L670`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L670) — Print color analysis in a readable format
  - `test_dialogue_box_detection(self, screenshot: Image.Image)` — [`L796`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L796) — Test dialogue box detection with detailed output for green line method
  - `update_dialogue_colors_from_analysis(self, screenshot: Image.Image, threshold_percentage: float = 1)` — [`L716`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L716) — Update DIALOGUE_TEXT_COLORS based on analysis of actual screenshot.
  - `BATTLE_TEXT_COORDS` — [`L98`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L98)
  - `COLOR_TOLERANCE` — [`L70`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L70)
  - `DIALOGUE_BOX_BACKGROUND_COLORS` — [`L73`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L73)
  - `DIALOGUE_BOX_BACKGROUND_THRESHOLD` — [`L95`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L95)
  - `DIALOGUE_BOX_COORDS` — [`L26`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L26)
  - `DIALOGUE_TEXT_COLORS` — [`L42`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L42)
  - `OCR_TEXT_COORDS` — [`L34`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L34)
  - `debug_color_detection` — [`L109`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L109)
  - `last_detected_text` — [`L106`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L106)
  - `skip_dialogue_box_detection` — [`L111`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L111)
  - `stable_text_count` — [`L108`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L108)
  - `text_stability_threshold` — [`L107`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L107)
  - `use_full_frame_scan` — [`L110`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L110)
- protocol/private: `__init__`[`L105`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L105)
- uses (calls/refs, reference-scoped): [`logger`](ocr_dialogue.md#logger), [`OCR_AVAILABLE`](ocr_dialogue.md#OCR_AVAILABLE)
- used by: [`read_dialog_with_ocr_fallback`](../pokemon_env/memory_reader.md#PokemonEmeraldReader.read_dialog_with_ocr_fallback), [`create_ocr_detector`](ocr_dialogue.md#create_ocr_detector)  (4 test-only)

## Functions
- `create_ocr_detector()` — [`L1014`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L1014) — Factory function to create OCR detector if available

## Module values
- `OCR_AVAILABLE` — [`L15`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L15)
- `logger` — [`L20`](../../../../../raw/code/continual-harness/utils/ocr_dialogue.py#L20)

