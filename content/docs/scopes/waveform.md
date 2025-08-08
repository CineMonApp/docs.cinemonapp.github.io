---
title: Waveform
weight: 31
---

## 1  Overview / Purpose & Usage
Where the Histogram shows how *much* brightness exists, the **Waveform** shows *where* that brightness sits across the image width.  Activate via the Scopes bar; the scope appears as a strip you can resize or full‑screen.  Shadows anchor at the bottom of the graph, highlights at the top, so a rising coastline indicates a bright sky across the top of frame.

## 2  Options & Modes
| Option | Choices | Intended Use |
|--------|---------|--------------|
| Display Type | Luma, Colourized Luma, RGB, RGB Parade | Progressive detail for exposure and balance. |
| Instant Extents | Toggle | Overlays min/max envelope—great for flickering lights. |
| Trace Brightness | 0 – 100 % | Brighten trace on sunny sets. |
| Background Alpha | 0 – 100 % | Fade background so image shows through. |

**Colourized Luma** keeps luma shape but colours pixels by hue—ideal for spotting colour contamination in gradients.  **RGB Parade** separates channels so you can ride white‑balance: align the three waveforms and neutrals snap into place.

## 3  Tips, Best Practices & Use‑Cases
Keying a talking‑head against a window?  Watch the right side of the waveform: if highlights scrape 100 IRE while the face hovers at 50, you know contrast is within broadcast safe.  For music videos, enable **Instant Extents**; flashing LEDs produce a bright envelope that warns how far peaks reach, without cluttering the main trace.

## 4  Related Topics
* [`histogram.md`](histogram.md) – statistical companion  
* [`vectorscope.md`](vectorscope.md) – chroma balance after luma is locked
