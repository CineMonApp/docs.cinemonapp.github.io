---
title: Zebras
weight: 23
---

## 1  Overview / Purpose & Usage
Zebras layer diagonal stripes over pixels that fall above or below chosen luma thresholds.  Highlight zebras warn of clipping whites, shadow zebras flag crushed blacks.  Tap the **Zebra** icon; CineMon applies your last thresholds and colours.  Opening the drawer reveals dual sliders so you can tune each band with single‑digit precision.

## 2  Options & Modes
| Option | Value Type | Range | What It Does |
|--------|-----------|-------|--------------|
| Shadow Threshold | Percentage slider | **0 – 50 % IRE** | Pixels *below* this IRE show Shadow zebras. |
| Highlight Threshold | Percentage slider | **50 – 110 % IRE** | Pixels *above* this IRE show Highlight zebras. |
| Shadow Colour | RGBA swatch | Full palette | Tint of shadow stripes. |
| Highlight Colour | RGBA swatch | Full palette | Tint of highlight stripes. |

The slider labels display numeric IRE values as you drag.  For log curves, set *Highlight* roughly 5 IRE under the camera’s clipping code‑value (e.g., 93 IRE for ARRI LogC).  Shadow warnings usually sit one or two stops above the noise floor—about 10 IRE on typical cinema sensors.

## 3  Tips, Best Practices & Use‑Cases
Pull highlight zebras down slightly during sunset: a faint zebra on the sun means the grade can safely push exposure without losing texture.  In night shoots, enabling only shadow zebras helps spot tunnel‑vision blacks so the colourist isn’t forced to lift noisy shadows later.

## 4  Related Topics
* [`false-color.md`](false-color.md) – holistic exposure map that complements zebras  
* [`histogram.md`](../scopes/histogram.md) – numerical distribution to back up zebra decisions
