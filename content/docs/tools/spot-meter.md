---
title: Spot Meter
weight: 150
---

{{< screenshot name="spot-meters" alt="Spot Meters Tool" >}}

## Overview

With this patent pending tool you can have two virtual spot light meters to accurately measure relative scene luminance using photometric units (F-stops). For this to work properly you need to make sure that the input image gamma curve is properly configured in the [preset settings sidebar](/docs/presets). You can move the spot meter probes around the frame and get an accurate exposure value. Middle gray is initially represented by 0 EV at 18% gray, but can be re-calibrated as needed. Other luminance values are represented by the number of stops over or under middle gray. You can also turn on a contrast ratio guide to show the relative lighting ratio between the two probes.

## Options

{{< option-bar-sprite row="11" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Meter A | EVs | - | Shows the scene luminance value in relative stops over/under middle gray. |
| Set A | EVs | - | Sets the value of middle gray to whatever meter A is measuring. |
| Meter B | EVs | - | Shows the scene luminance value in relative stops over/under middle gray. |
| Set B | EVs | - | Sets the value of middle gray to whatever meter B is measuring. |
| Contrast | Ratio | - | The luminance contrast ratio between meter A and meter B. |
| Contrast Label | `On`/`Off` | `On` | Controls the visibility of the contrast ratio elastic bar. |
| 0 EV Luma | Real number | `0.18` | The luma value considered middle gray. |
| 0 EV Luma Stepper | - | - | Increment/Decrement the value of middle gray by 0.01. |
| Reset 0 EV | - | - | Resets the value of 0 EV to 0.18. |

## Tips

If you want a 2:1 key‑to‑fill ratio, place meter A over a portion of the image that is illuminated by the key light (e.g. the talent's cheek bone), then drag meter B to the fill side. Adjust lights until the contrast ratio reads **2.0:1**.
