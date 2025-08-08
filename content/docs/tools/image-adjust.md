---
title: Image Adjust
weight: 24
---

## 1  Overview / Purpose & Usage
The **Image Adjust** panel gives you three realtime grading knobs—Exposure, Contrast, Saturation—processed on the GPU *after* your chosen LUT so you preview the final picture, not a flat log curve.  Tap the **Adjust** icon; three dials float above the live feed.  Spin each dial with your finger or mouse wheel and watch the image respond in a single frame.

## 2  Options & Modes
| Option | Value Type | Range | Function |
|--------|-----------|-------|----------|
| Exposure | Rotary dial | **–5 → +5** EV | Photometrically raises or lowers brightness in full‑stop increments (fine‑tunable to 0.1). |
| Contrast | Rotary dial | **0.5 → 2.0** gain | Compresses or expands mid‑tones; 1.0 is neutral. |
| Saturation | Rotary dial | **0 → 200 %** | 0 % = monochrome; 200 % exaggerates colour. |
| Reset | Button | — | Instantly zeros all three dials. |

Each dial shows numeric read‑outs beneath so a DP can say, “Give me +0.7 EV and +10 % saturation” and assistants can replicate that precisely on other units.  CineMon stores these offsets in the active preset but never writes them into the recorded media—changes are purely display‑side.

## 3  Tips, Best Practices & Use‑Cases
Pull Saturation to zero and enable **Focus Peaking**; the coloured halo leaps off the grey picture—excellent for backlit silhouettes.  Slight negative Contrast (0.8) mimics a flat grade for dynamic range checks, while a +1 EV boost previews how low‑light footage will lift in post.  Because adjustments are GPU accelerated, there is no extra latency—vital for pulling focus off the monitor.

## 4  Related Topics
* [`display-lut.md`](display-lut.md) – the LUT you grade *after*  
* [`focus-peaking.md`](focus-peaking.md) – high‑visibility peaking when saturation is 0 %
