---
title: Display LUT
weight: 25
---

## 1  Overview / Purpose & Usage
**Display LUT** loads external `.cube` files and applies them in real time so everyone on set views the footage through the intended look.  Tap the **LUT** icon; three quick‑slots pop up.  Tap a slot to toggle it, or long‑press to replace it with a different LUT from Files, Dropbox, or AirDrop.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Details |
|--------|-----------|-----------------|---------|
| Quick‑Slots | Three toggles | A, B, C | Hold three LUTs per preset for instant A/B/C. |
| LUT Library | File list | Unlimited `.cube` | Managed in **Organizer › Display LUTs**. |
| Bypass | Toggle | Off / On | Temporarily disables LUT without clearing slot. |

When you replace a LUT, CineMon validates its cube size and bit‑depth, then stores it inside the app container so you can unplug network drives without “LUT missing” warnings.  The **Bypass** toggle blinks the image to log for one second—handy for teaching students how a grade affects dynamics.

## 3  Tips, Best Practices & Use‑Cases
Slot 1 usually carries the camera manufacturer’s tech LUT; Slot 2 a show look from the colourist; Slot 3 a “print stock” for fun.  During dailies reviews, operators swipe between LUT presets (Grid, False‑Color, etc.) and the quick‑slots survive, so you can compare log and graded images under the same scopes.  Remember to note which slot was live when capturing frame‑grabs—the PNG embeds that info in its metadata for editorial.

## 4  Related Topics
* [`image-adjust.md`](image-adjust.md) – refine exposure after the LUT  
* [`presets.md`](../presets.md) – where LUTs are organised and shared
