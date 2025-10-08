---
title: Color Management
weight: 8
---

{{< screenshot name="preset-gamma" alt="Presets Screen" >}}

## Overview

*This is an advanced topic that only applies to input signals that are in a log format, and is only available in {{< pro-pill >}}. If your input signal is already in a display format (e.g. Rec.709), feel free to skip this whole section.*

Some CineMon monitoring functions work in linear light. This works best when the input signal provides a wide dynamic range of tonal and color values, which is usually accomplished by encoding the signal using a log curve and a wide color gamut.

Use [**Preset Settings**](/docs/presets#preset-settings) to configure your input signal's **Input Gamma** and **Input Gamut**. This will ensure that CineMon's photometric features work correctly with your video.

## Color Space Transform (CST)

CineMon supports a **Color Space Transform (CST)** function that converts the input signal's gamma and gamut (Color Space) to a destination space (e.g., `ARRI LogC4`/`ARRI Wide Gamut` → `Rec.709`/`BT.709`). Some professional video editing and color correcting applications offer similar capabilities, also known as Display Rendering Transforms (DRTs). CineMon's CST functions are GPU-accelerated, mathematical functions built from official camera vendor specifications for their supported log curves, and color primaries.

{{< screenshot name="preset-gamut" alt="Presets Screen" >}}

When the CST is turned on, the processing happens right after the **Calibration LUT** is applied, and before any other image manipulation.

> Features dependent on linear light processing, such as the **Spot Meters** and **Test Strip** will tap the image before the CST is applied.

This feature is commonly used to convert from a camera log profile (e.g. Sony `SLog3`/`SGamut3.Cine`), also known as a **Scene Referred** color space, to a range of tones and colors that look better on standard screens, also known as **Display Referred** space (e.g. `Rec.709`).

Scene referred signals usually look flat and washed out, with low color saturation, which can make it more difficult to monitor on set. Applying a CST is a dependable, clinical way to preview the image, without introducing a creative look bias.

Another popular way of achieving a similar result is by applying a Display Lookup Table (LUT), which CineMon supports. However, because of how LUTs work, they always involve a certain amount of creative manipulation by the author. So the transformed image often deviates from the pure mathematical precision of a CST, which may be what you want.

We recommended that you test your Color Management workflow end-to-end before deciding which method is the best fit for your project.

> You can still layer a **Display LUT** after a CST for a creative look. In fact, many popular Display LUTs are built assuming the base image is in a specific Log Space (e.g. `ARRI LogC3` or `Cineon`). The CST doesn't need to convert from a scene referred gamma to a display referred one. You can convert from a camera-specific log curve (e.g. `VLog`/`V-Gamut`) to a different one (e.g. `Cineon`), to use as a base for further processing.
> These transforms are high-precision (64-bit), GPU-accelerated math functions that don't introduce any signal quality loss.

## Supported Log Profiles

| Type | Description | Values |
|------|-------------|--------|
| Gamma[*](#input-gamma-notes) | Supported gamma curves. | `Rec.709`, `ACEScc`, `ACEScct`, `Apple Log`, `ARRI LogC3`, `ARRI LogC4`, `Blackmagic Film Gen5`, `Canon CLog2`, `Canon CLog3`, `Kodak Cineon`, `DaVinci Intermediate`, `DJI DLog`, `Fujifilm F-Log`, `Fujifilm F-Log2`, `GoPro ProTune`, `Leica LLog`, `Nikon NLog`, `Panasonic VLog`, `Red Log3G10`, `Sony SLog2`, `Sony SLog3` |
| Color Space (Gamut) | Supported color spaces or gamuts. | `Rec.709/sRGB`, `Rec.2020 (Apple/Fujifilm/Nikon/Leica)`, `DisplayP3`, `ACES AP0`, `ACES AP1`, `ARRI Wide Gamut 3`, `ARRI Wide Gamut 4`, `Blackmagic Film Gen5 Wide Gamut`, `Canon Cinema Gamut`, `DaVinci Wide Gamut`, `Fujifilm F-Gamut C`, `Panasonic V-Gamut`, `Red Wide Gamut`, `Sony SGamut3.Cine`, `Sony SGamut3`, `Sony Venice SGamut3.Cine`, `Sony Venice SGamut3` |

Associated [**Preset Settings**](/docs/presets#preset-settings):

| Type | Description | Values |
|------|-------------|--------|
| Apply Color Space Transform | Activates a Color Space Transform (CST) or Display Rendering Transform (DRT) from the Input Gamma and Color Space to the Output Gamma and Color Space. | `On`/`Off` |
| Tone Mapping | Applies a tone mapping function to compress higher dynamic range values to fit in the destination color space. | `On`/`Off` |
| Preserve Saturation | Modifies the tone mapping function to preserve saturation values. | `On`/`Off` |
| Gamut Compression | Compresses color values from a larger gamut to fit the a smaller destination gamut. | `On`/`Off` |

### Input Gamma Notes

The following tools are photometrically accurate only if the input signal is in a scene referred gamma, and if the **Input Gamma** setting matches the input image's log curve:

* **Spot Meters**
* **Test Strip**
* **Exposure Adjust**
* **Color Space Transform**

> If the input image is not in a log format (e.g. Rec.709), or the **Input Gamma** setting is not properly configured, these tools will report inaccurate exposure levels.
