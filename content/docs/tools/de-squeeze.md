---
title: Anamorphic De-squeeze
weight: 15
---

## 1  Overview / Purpose & Usage
Anamorphic lenses squeeze the world horizontally to record a wider field of view onto a narrower sensor.  CineMon’s **De‑squeeze** stretches that image back so you see correct proportions, enabling accurate composition and focus pulls.  
Activate the tool with the **De‑squeeze** icon.  A pop‑over lists mainstream squeeze ratios—**1.25×, 1.33×, 1.5×, 1.8×, 2.0×**—and a “Manual” slider for oddball glass.  CineMon writes the chosen ratio into each preset; switching between spherical and anamorphic looks is then as easy as swiping presets.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Purpose |
|--------|-----------|-----------------|---------|
| Preset Ratio | Radio | 1.25× → 2.0× | Matches common anamorphic families. |
| Manual Slider | Float | 1.00× → 2.50× (0.01 steps) | Fine‑tune vintage or aftermarket adapters. |
| Playback De‑squeeze | Toggle | Off / On | Applies the same ratio to recorded clips. |

Selecting a **Preset Ratio** instantly scales the live feed.  The **Manual Slider** updates the numeric label in real time so lens technicians can dial, say, **1.58×** to match rehoused projector elements.  Turning on **Playback De‑squeeze** means you can scrub recorded clips—looping them for lighting checks—without burning a temporary LUT in post.

## 3  Tips, Best Practices & Use‑Cases
Combine De‑squeeze with **Focus Peaking**: CineMon applies peaking *after* stretching, so edge‑detail reflects real geometry, not the squeezed distortion that fools many monitors.  Saving the transform as part of your “Show Look” preset means the DP flips between spherical rehearsals and anamorphic hero takes with one gesture—no hidden maths.  Remember to disable the tool before exporting frame grabs for online sharing; otherwise JPGs appear skinny on devices that don’t auto‑scale.

## 4  Related Topics
* [`image-flip.md`](image-flip.md) – solve inverted anamorphic rigs in tandem  
* [`focus-peaking.md`](focus-peaking.md) – peaking respects the stretched aspect
