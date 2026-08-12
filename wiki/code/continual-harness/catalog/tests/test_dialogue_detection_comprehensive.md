---
title: 'Module: tests/test_dialogue_detection_comprehensive.py'
type: catalog
provenance: extracted
module: tests/test_dialogue_detection_comprehensive.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `tests.test_dialogue_detection_comprehensive`/TestDialogue
symbols:
  TestDialogueDetection._test_state_file: Detection#_test_state_file().
  TestDialogueDetection.detector: Detection#detector.
  TestDialogueDetection.test_coordinate_tightness: Detection#test_coordinate_tightness().
  TestDialogueDetection.test_ocr_preprocessing_quality: Detection#test_ocr_preprocessing_quality().
  TestDialogueDetection.agent_port: Detection#agent_port.
  TestDialogueDetection.test_static_image_detection: Detection#test_static_image_detection().
  TestDialogueDetection.test_no_dialog_states: Detection#test_no_dialog_states().
  TestDialogueDetection.test_dialog_states: Detection#test_dialog_states().
  TestDialogueIntegration.test_comprehensive_state_includes_dialog: Integration#test_comprehensive_state_includes_dialog().
  TestDialogueDetection: Detection#
  TestDialogueDetection.setup: Detection#setup().
  TestDialogueDetection.teardown_method: Detection#teardown_method().
  TestDialogueIntegration: Integration#
---
# Module: [`tests/test_dialogue_detection_comprehensive.py`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py)

## Classes
### `TestDialogueDetection`
- def: [`tests/test_dialogue_detection_comprehensive.py:23`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L23)
- doc: Test dialogue detection accuracy across all provided states
- signature: `class TestDialogueDetection:`
- members:
  - `_test_state_file(self, state_file, expected_dialogue, description="")` — [`L42`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L42) — Helper to test a single state file
  - `setup(self)` — [`L27`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L27) — Setup for each test
  - `teardown_method(self)` — [`L37`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L37) — Cleanup after each test
  - `test_coordinate_tightness(self)` — [`L124`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L124) — Test that OCR coordinates are properly tight around text area
  - `test_dialog_states(self)` — [`L158`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L158) — Test states that SHOULD have dialogue
  - `test_no_dialog_states(self)` — [`L143`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L143) — Test states that should NOT have dialogue
  - `test_ocr_preprocessing_quality(self)` — [`L187`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L187) — Test that OCR preprocessing produces high-quality black/white output
  - `test_static_image_detection(self)` — [`L173`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L173) — Test detection on static images
  - `agent_port` — [`L30`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L30)
  - `detector` — [`L29`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L29)
- uses (calls/refs, reference-scoped): [`detect_dialogue_from_screenshot`](../utils/ocr_dialogue.md#OCRDialogueDetector.detect_dialogue_from_screenshot), [`create_ocr_detector`](../utils/ocr_dialogue.md#create_ocr_detector), [`is_dialogue_box_visible`](../utils/ocr_dialogue.md#OCRDialogueDetector.is_dialogue_box_visible), [`_preprocess_for_ocr`](../utils/ocr_dialogue.md#OCRDialogueDetector._preprocess_for_ocr), [`DIALOGUE_BOX_COORDS`](../utils/ocr_dialogue.md#OCRDialogueDetector.DIALOGUE_BOX_COORDS), [`OCR_TEXT_COORDS`](../utils/ocr_dialogue.md#OCRDialogueDetector.OCR_TEXT_COORDS)

### `TestDialogueIntegration`
- def: [`tests/test_dialogue_detection_comprehensive.py:211`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L211)
- doc: Test integration with LLM agent comprehensive state
- signature: `class TestDialogueIntegration:`
- members:
  - `test_comprehensive_state_includes_dialog(self)` — [`L214`](../../../../../raw/code/continual-harness/tests/test_dialogue_detection_comprehensive.py#L214) — Test that comprehensive state includes dialogue reading
- uses (calls/refs, reference-scoped): [`create_ocr_detector`](../utils/ocr_dialogue.md#create_ocr_detector)

