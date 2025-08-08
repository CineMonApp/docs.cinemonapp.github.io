---
title: Focus Peaking
weight: 22
---

## 1  Overview / Purpose & Usage
Manual focus lacks depth of field indicators.  **Focus Peaking** solves that by colouring high‑frequency edges so the puller sees exactly where sharpness lies.  Toggle the feature via the **Focus** icon; CineMon’s GPU analysis runs at full frame rate, so the coloured halo snaps on and off as the lens ring turns.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Meaning |
|--------|-----------|-----------------|---------|
| Peaking Mode | Toggle | Full Image / Edges Only | “Edges Only” hides the video and shows just peaking strokes. |
| Highlight Colour | RGBA swatch | Full palette | Tint of the peaking overlay. |
| Sensitivity | Percentage slider | **0 – 100 %** | Lower values detect only tack‑sharp edges; higher includes semi‑sharp. |

With **Edges Only**, the screen becomes a neon wireframe—immensely helpful in loud environments where subtle colour doesn’t cut it.  **Sensitivity** defaults to 60 percent; dial to 40 when shooting wide‑open on full‑frame where the depth of field is razor thin, or up to 80 when you need to see mid‑tones crisp for deep focus work.

## 3  Tips, Best Practices & Use‑Cases
Activating **Image Adjust → Saturation 0 %** converts the scene to monochrome, letting the peaking colour pop against a grey canvas—classic in high‑contrast stage shows.  Because CineMon peaking runs *after* **De‑squeeze**, edge detection uses corrected pixel geometry, avoiding false sharpness on squeezed footage.

## 4  Related Topics
* [`image-adjust.md`](image-adjust.md) – turn saturation to zero before peaking  
* [`de-squeeze.md`](de-squeeze.md) – geometry‑correct peaking for anamorphics
