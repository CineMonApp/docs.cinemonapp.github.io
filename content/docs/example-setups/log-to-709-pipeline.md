---
draft: true
title: Log→Rec.709 Pipeline
weight: 3
---

## Overview
A repeatable colour pipeline that converts camera log/gamut to Rec.709 via CST, then layers a creative Display LUT, ensuring both technical correctness and creative intent on‑set.

## Options
| Step | Choice | Why |
|---|---|---|
| 1 | CST Input=Camera, Output=Rec.709 | Objective conversion from scene‑referred to display. |
| 2 | Display LUT Slot 2=Show Look | Creative intent on top of objective base. |
| 3 | False Color Pre‑LUT | Exposure evaluation unaffected by look. |

## Tips & Use Cases
Save both **709** and **P3** variants as presets for different monitors. Use **Tetrahedral** interpolation for smoother gradients when evaluating skies and beauty lighting.

## Related Topics
* [`color-management.md`](../guides/color-management.md)
* [`display-lut.md`](../tools/display-lut.md)
