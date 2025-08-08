---
title: False Color
weight: 26
---

## 1  Overview / Purpose & Usage
False Color remaps luma to rainbow‑style bands so operators *see* exposure instead of deciphering numbers.  Enable via the **FC** icon; CineMon overlays a semi‑transparent legend at screen right and colours pixels according to the active gradient.  Drag the icon up to swap gradients or open the node‑based editor.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Description |
|--------|-----------|-----------------|-------------|
| Gradient Library | List | Built‑in presets + user | Choose which colour set to use. |
| Node Editor | GUI | Drag nodes, pick colours | Redefine what IRE maps to which colour. |
| Legend | Toggle | On / Off | Shows live IRE‑colour correspondence. |

**Gradient Library** ships with popular maps: Atomos, SmallHD, and a neutral CineMon default.  Duplicating a gradient opens the **Node Editor**, where each node sits at an IRE coordinate.  Drag a node to 41 IRE and colour it green—now middle grey shows bright lime, a cue most operators internalise faster than reading spot numbers.  The **Legend** can be hidden once the team memorises the palette, freeing screen space.

## 3  Tips, Best Practices & Use‑Cases
Calibrate a gradient to your camera’s log curve: set 95 IRE to hot pink so clipped highlights scream at you.  Export the gradient—CineMon saves a lightweight JSON—and AirDrop to every iPad on set, ensuring DIT, DP, and Client monitor speak the same exposure language.  Pair False Color with **Spot Meter** to cross‑check numeric EV against colour bands for bulletproof exposure decisions.

## 4  Related Topics
* [`zebras.md`](zebras.md) – stripe warnings that complement colour bands  
* [`spot-meter.md`](spot-meter.md) – numeric EV to validate the colours
