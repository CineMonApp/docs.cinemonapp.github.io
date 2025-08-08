---
title: Settings Sidebar
weight: 2
---

## 1  Overview / Purpose & Usage
The **Settings Sidebar** groups pipeline‑wide options that affect every preset: incoming signal characteristics, video levels, performance trade‑offs, and UI appearance.  Tap the Sidebar icon, choose **Settings**, and you’ll see four collapsable sections.

## 2  Options & Modes
| Section | Key Options | Reason to Change |
|---------|-------------|------------------|
| Signal | Log Curve (F‑Log, LogC, S‑Log3, HLG…) | Calibrates False Color, Spot Meter, and LUT transforms. |
| Levels | Data (16‑235) / Full (0‑255) | Match external recorders or LED walls. |
| Pipeline | Quality ↔ Latency slider | Drag to low latency for focus pulling; quality when image fidelity trumps delay. |
| UI Brightness | 0 – 100 % | Dim toolbars on night shoots to protect dark adaptation. |

Changing **Log Curve** informs all camera‑aware tools so 18 % grey maps correctly.  **Pipeline** slides between a single‑pass shader (lowest lag) and multi‑pass HDR tone‑mapping (highest fidelity).

## 3  Tips, Best Practices & Use‑Cases
Always set Signal before rolling; otherwise False Color may highlight middle grey as bright red when you expected green.  At outdoor concerts drag UI Brightness below 15 % so string lights don’t reveal your monitor position to the audience.  For live focus assists, push Latency to minimum—every frame counts when pulling at 120 fps.

## 4  Related Topics
* [`spot-meter.md`](tools/spot-meter.md) – uses the selected Log curve
* [`gestures.md`](gestures.md) – hide toolbars after dimming UI brightness
