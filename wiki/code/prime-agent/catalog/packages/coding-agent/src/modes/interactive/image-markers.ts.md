---
title: 'Module: packages/coding-agent/src/modes/interactive/image-markers.ts'
type: catalog
provenance: extracted
module: packages/coding-agent/src/modes/interactive/image-markers.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-coding-agent 0.7.2 src/modes/interactive/`image-markers.ts`/
symbols:
  imageMarkerIds: imageMarkerIds().
  collectMarkedImages: collectMarkedImages().
  remapImageMarkers: remapImageMarkers().
  formatImageMarker: formatImageMarker().
  evictImagesToBudget: evictImagesToBudget().
  IMAGE_MARKER_REGEX: IMAGE_MARKER_REGEX.
---
# Module: [`packages/coding-agent/src/modes/interactive/image-markers.ts`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts)

## Functions
- `collectMarkedImages(pending: ReadonlyMap<number, T>, text: string)` — [`L37`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L37) — Images from `pending` whose marker still appears in `text`, in paste order
- `evictImagesToBudget(images: Map<number, T>, sizeOf: (value: T) => number, maxBytes: number, keep: ReadonlySet<number>)` — [`L57`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L57) — Evict oldest entries (insertion order) from `images` until the total of
- `formatImageMarker(id: number)` — [`L13`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L13) — The marker text inserted into the editor for pasted image `id`.
- `imageMarkerIds(text: string)` — [`L18`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L18) — Marker ids that appear in `text`, in order of appearance.
- `remapImageMarkers(text: string, remaps: ReadonlyMap<number, number>)` — [`L25`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L25) — Replace every image-marker spelling whose numeric id appears in `remaps`.

## Module values
- `IMAGE_MARKER_REGEX` — [`L10`](../../../../../../../../../raw/code/prime-agent/packages/coding-agent/src/modes/interactive/image-markers.ts#L10) — Matches `[image #N]` markers inserted when an image is pasted into the editor.

