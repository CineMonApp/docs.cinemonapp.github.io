---
title: Presets
weight: 5
---

{{< screenshot name="preset-1" alt="Presets Screen" >}}

## Overview

CineMon **Presets** capture the entire monitoring configuration state (active tools, tool option values, signal processing settings, UI layouts, etc.) so you can easily recall them when needed. Presets are a {{< pro-pill >}} feature.

You can create as many Presets as you need to organize your most frequently used monitoring configurations. This is a time saver compared to manually toggling tools, options, and layouts every time.

For instance, you might have a **Camera Preset**, with your favorite composition guides and focus peaking turned on. An **Exposure & Lighting** preset with Zebras and False Color set to your preferred levels. A **Look Preview** preset with a custom aspect ratio frame blanking and a creative LUT applied. And a **Technical** preset with a 2x2 grid populated with your favorite arrangement of scopes.

## Switching Presets

There are several ways to activate a saved preset:

* Select the **Preset** from the **Presets Menu** in the **Assist Toolbar**
* Select the **Preset** from the **Presets List** in the **Organizer** (if visible)
* Swipe left or right on a viewer to cycle through the **Presets** (if enabled in the **Global App Settings**)

## Configuration Change Indicator

If you make a change to the monitoring configuration, the color of the **Preset Name** on the **Assist Toolbar** will change from `White` to `Orange`, to warn you that the current configuration no longer matches the saved version. If you have the **Organizer** open, an orange "edited" badge will appear next to the Active Preset name.

{{< screenshot name="organizer-presets-edit" alt="Presets Organizer" >}}

## Preset Actions

To manage your Presets the following actions are available from the **Preset Actions** menu on the **Assist Toolbar** or the context menu in the **Organizer**:

| Action | Effect | Notes |
|--------|--------|-------|
| **New** | Creates a new blank Preset named "New Preset" with all assist tools and scopes turned off and all options reset at their default values. | |
| **Duplicate** | Creates a copy of the current configuration with the same name + "(Copy)". | |
| **Save** | Save all configuration changes to the active preset. | Only available if the configuration has changed. |
| **Revert** | Reverts any configuration changes to the last saved version of the preset. | Only available if the configuration has changed. |
| **Rename** | Enters rename mode to allow you to change the Preset name. | |
| **Delete** | Deletes the active Preset. | |
| **Export** | Opens an export dialog to save the active Preset to the file system. | Only available from the **Organizer**. |

## Preset Settings

The **Settings** tab on the **Sidebar** shows a series of controls to configure the signal processing pipeline, performance optimization settings, and UI. For instance, This is where you will configure your camera or input signal **Log Profile**, which is required for the correct functioning of several features.

| Control | Description | Values |
|---------|--------|-------------|
| Active Preset | This field shows the name of the active preset. | Name of the active preset |
| Convert Levels to Full | If on, CineMon converts the input signal data levels from video (16-235) to full (0-255). | `On`/`Off` |
| Input Gamma[*](#input-gamma-notes) | The input signal's gamma curve. | `Rec.709`, `ACEScc`, `ACEScct`, `Apple Log`, `ARRI LogC3`, `ARRI LogC4`, `Blackmagic Film Gen5`, `Canon CLog2`, `Canon CLog3`, `Kodak Cineon`, `DaVinci Intermediate`, `DJI DLog`, `Fujifilm F-Log`, `Fujifilm F-Log2`, `GoPro ProTune`, `Leica LLog`, `Nikon NLog`, `Panasonic VLog`, `Red Log3G10`, `Sony SLog2`, `Sony SLog3` |
| Input Color Space (Gamut) | The input signal's color space or gamut. | `Rec.709/sRGB`, `Rec.2020 (Apple/Fujifilm/Nikon/Leica)`, `DisplayP3`, `ACES AP0`, `ACES AP1`, `ARRI Wide Gamut 3`, `ARRI Wide Gamut 4`, `Blackmagic Film Gen5 Wide Gamut`, `Canon Cinema Gamut`, `DaVinci Wide Gamut`, `Fujifilm F-Gamut C`, `Panasonic V-Gamut`, `Red Wide Gamut`, `Sony SGamut3.Cine`, `Sony SGamut3`, `Sony Venice SGamut3.Cine`, `Sony Venice SGamut3` |
| Calibration LUT | A LUT to be applied to the input signal at the beginning of the signal processing pipeline. | Optional LUT |
| Interpolation | Interpolation type used when applying the Calibration LUT. | `Standard`/`Tetrahedral` |
| Apply Color Space Transform | Activates a Color Space Transform (CST) or Display Rendering Transform (DRT) from the Input Gamma and Color Space to the Output Gamma and Color Space. | `On`/`Off` |
| Output Gamma | The destination gamma for a CST. | Same as Input Gamma |
| Output Color Space | The destination color space for a CST. | Same as Input Color Space |
| Tone Mapping | Applies a tone mapping function to compress higher dynamic range values to fit in the destination color space. | `On`/`Off` |
| Preserve Saturation | Modifies the tone mapping function to preserve saturation values. | `On`/`Off` |
| Gamut Compression | Compresses color values from a larger gamut to fit the a smaller destination gamut. | `On`/`Off` |
| Crop Horizontal | Crops the input image horizontally by the selected amount. | `0`-`500`px |
| Crop Vertical | Crops the input image vertically by the selected amount. | `0`-`500`px |
| Tap Signal At | Controls the stage of the image processing pipeline is used as input to Scope processing. Start means the Scopes measure the raw source signal. End means the Scopes measure the processed signal (after CST, color adjustments, etc.) | `Start`/`End` |
| High Resolution Scopes | Enables high resolution Scopes processing. If off, Scopes work on a internally resized image to improve real-time performance. | `On`/`Off` |
| Apply Low-pass Filter | Control the use of a low-pass filter to reduce high-frequency noise in Scope traces. | `On`/`Off` |
| Low-pass Filter Level | Change the amount of high-frequency filtering. | Range |
| Display LUT Interpolation | Interpolation type used when applying the monitoring Look LUTs. | `Standard`/`Tetrahedral` |
| Limit to HD Resolution | Reduces the size of the input image to a maximum of 1080p (HD) | `On`/`Off` |
| Toolbar Brightness | Dim the toolbar's brightness. | `10`–`100`% |
| Show System Status Bar ({{< ipad >}} Only) | Show or hide the System Status Bar, which shows the date/time, WiFi signal strength, Battery level, etc. | `On`/`Off` |

### Input Gamma Notes

The following tools are photometrically accurate only if the input signal is in a scene referred gamma, and if the **Input Gamma** setting matches the input image's log curve:

* **Spot Meters**
* **Test Strip**
* **Exposure Adjust**
* **Color Space Transform**

> If the input image is not in a log format (e.g. Rec.709), or the **Input Gamma** setting is not properly configured, these tools will report inaccurate exposure levels.