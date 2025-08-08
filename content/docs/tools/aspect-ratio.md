---
title: Aspect Ratio Guides
weight: 13
---

## 1  Overview / Purpose & Usage
Modern productions often finish in multiple aspect ratios: a 2.39 theatrical master, a 16:9 television pass, and vertical 9:16 teasers for social.  CineMon’s Aspect Ratio Guides let you visualise those mattes in real time *without* sacrificing live pixels.  
Tap the **Ratio** icon once; black bars appear top and bottom (or left and right, depending on orientation).  Drag again to open the preset selector: choose a standard crop or enter a custom ratio—CineMon parses the pair of integers you type and builds the matte on the fly.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Detail |
|--------|-----------|-----------------|--------|
| Preset Ratio | Radio buttons | 2.39, 2.00, 1.85, 1:1, 9:16 | One‑tap access to industry standards. |
| Custom Ratio | Two integer fields | Any positive pair | Enter width and height; e.g., **18 × 9** draws a 2:1 matte. |
| Bar Colour | RGBA swatch | Full palette | The colour of the crop bars. |
| Opacity | Percentage slider | **0 – 100 %** | Full black down to barely‑there grey. |

Selecting a **Preset** redraws the matte instantly.  Choosing **Custom** pops two numeric spinners; CineMon overlays live feedback so you know you typed the ratio correctly.  *Bar Colour* defaults to black, but a 50 percent grey is handy when you need to see lighting gear that might creep into the overscan.

## 3  Tips, Best Practices & Use‑Cases
Because the guide lives in the post‑LUT display chain, you can flip LUTs yet keep the matte intact.  Many crews keep two presets—“Deliver 16:9” and “Deliver 9:16”—and swipe left/right to reassure agencies that creative intent survives every screen.  During a rush grab of still images, set opacity to 0 percent: you retain the safe outlines (thin dashed line) but remove heavy bars, keeping thumbnails uncluttered.

## 4  Related Topics
* [`safe-area.md`](safe-area.md) – fits inside whatever crop you set  
* [`grid-overlay.md`](grid-overlay.md) – automatically scales to the active crop
