---
title: Vectorscope
weight: 32
---

{{< screenshot name="vectorscope-floating" alt="Vectorscope" >}}

## Overview

The **Vectorscope** is a precision color measurement instrument that displays the hue and saturation distribution of pixels in the image. It maps these values onto a polar graph, where angle equals hue and distance from center equals saturation. There are two types of Vectorscope displays: **Luma** and **Colorized**.

*Double-click/tap* in the window to open the Vectorscope settings bar. You can toggle the display of multiple reticle reference guides to aid in calibration, including 75% and 100% saturation targets for BT.709, a skin tone guide, 2x zoom, signal extents, and trace brightness adjustments, in addition to the display controls of the other floating scopes.

{{< screenshot name="vectorscope-extents" alt="Vectorscope Extents" >}}

## Settings

| Setting | Options | Description |
|---------|---------|-------------|
| Display Mode | `Mono`/`Colorized` | Select the vectorscope display mode. |
| Scope Settings | Reticle Color | Customize the color of the reticle. |
|  | Skin Tone Line | Displays a guide where average skin tones show up in a neutrally lit scene. |
| | 75% Targets | Shows 75% saturation target guides for Rec.709. |
| | 100% Targets | Shows 100% saturation target guides for Rec.709. |
| | Polar Scale | Shows a series of concentric polar guides. |
| | 2x Zoom | Applies a 2x zoom the the scope trace. |
| | Extents | Show an envelope of the min/max saturation values that might otherwise be difficult to see on the trace. |
| | `All`/`Low`/`Mid`/`High` | Optionally filters the trace to show only the colors in the shadow areas (Low), the mid tones, or the highlights. |
| | Low Range | Defines the IRE value threshold for the Low filtering. |
| | High Range | Defines the IRE value threshold for the High filtering. |
| Trace Brightness | Slider | Configures the brightness of the vectorscope trace. |
| Window Settings | Size | Adjust the size of the floating window. |
| | Opacity | Change the transparency of the floating window background. |
| Full Screen | - | Make the floating scope full screen. |

> Any signal that goes beyond 100% targets is considered oversaturated and might be illegal under the Rec.709 standard. There are several post production methods for compressing the signal's gamut when that happens.

> Use a standard color chart to aid in calibration of white balance and other camera settings.

{{< screenshot name="vectorscope-fs-options" alt="Vectorscope Settings" >}}
