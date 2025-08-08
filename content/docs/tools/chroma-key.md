---
title: Chroma-Key Assist
weight: 21
---

## 1  Overview / Purpose & Usage
Green‑screen day can feel like black magic until you see the key live.  **Chroma‑Key Assist** provides an on‑set preview so gaffers detect spill and DPs gauge separation long before post.  Tap the **Key Assist** icon, sample the backdrop colour with the on‑screen eyedropper, and CineMon removes that hue in real time.  The residual image can be set transparent or composited over a background plate you load from Files.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Purpose |
|--------|-----------|-----------------|---------|
| Eyedropper | Tap sample | Any pixel | Picks key colour—even odd cyan screens. |
| Erode | Percentage slider | **0 – 100 %** | Shrinks matte edges to eliminate halos. |
| Soften | Percentage slider | **0 – 100 %** | Blurs matte edges for gentler mixes. |
| Spill Suppress | Percentage slider | **0 – 100 %** | Desaturates stray key colour on foreground. |
| Background Plate | File browser | PNG / JPG / Video | Loads a comp plate behind the key. |

**Erode** eats into the matte boundary—use 3–5 percent to remove soft fringing from diffusion frames.  **Soften** applies a Gaussian blur; 10 percent is enough to feather edges so they merge nicely.  **Spill Suppress** darkens only the sampled colour family on the foreground, letting you preview how a spill‑killer gel might rescue wardrobe.

## 3  Tips, Best Practices & Use‑Cases
Lighting crews love to toggle Spill Suppress on, then physically adjust kicker lights until the slider falls to zero—proof the scene now keys cleanly without digital help.  When scouting, comp a rough previz background plate so the director sees camera height relative to 3‑D set extension; it sells the shot and avoids reshoots.

## 4  Related Topics
* [`vectorscope.md`](../scopes/vectorscope.md) – confirm the key hue hugs the UV axis  
* [`frame-overlay.md`](frame-overlay.md) – align cg plates with the live key preview
