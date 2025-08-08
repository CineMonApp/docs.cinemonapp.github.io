---
title: Histogram
weight: 30
---

## 1  Overview / Purpose & Usage
The **Histogram** graphs how many pixels sit at each brightness value, offering an at‑a‑glance sanity check that highlights aren’t clipping and shadows aren’t crushed.  Activate it from the Scopes bar; the floating window can be pinched to any size or double‑tapped for full‑screen.

## 2  Options & Modes
| Mode | What It Shows | Typical Usage |
|------|---------------|---------------|
| Luma | Y′ only | Quick exposure gauge. |
| RGB Overlay | Single trace, colour‑coded | Channel balance in one glance. |
| RGB Stacked | Three individual traces | Pinpoint per‑channel clipping. |
| Trace Gain | 0 – +12 dB | Boost low‑contrast scenes. |
| Reticle Colour | Any | Match ambient light. |
| Background Alpha | 0 – 100 % | Fade scope to minimise distraction. |

Switching between **Luma** and **RGB** is immediate; CineMon maintains history so when you return to RGB you pick up right where you left off.  Increasing **Trace Gain** can reveal subtle mid‑tone detail on Log footage that otherwise hugs the floor.

## 3  Tips, Best Practices & Use‑Cases
Full‑screen Histogram mode on a reference OLED makes an unbeatable lighting briefing tool: slide the lights until the histogram bell curve centres around 40–60 IRE, guaranteeing the grade has wiggle room.  Pair RGB Stacked with **Display LUT Bypass** to watch how the grade shifts distribution—useful when teaching new ACs about colour science.

## 4  Related Topics
* [`waveform.md`](waveform.md) – spatial exposure view  
* [`zebras.md`](../../tools/zebras.md) – overlay clipping warnings on top of the live picture
