---
title: False Color
weight: 140
---

{{< screenshot name="false-color-bmd" alt="False Color Tool" >}}

## Overview

You can apply a false color scheme to visually assist with exposure and lighting ratios. The tool remaps the image's pixel colors based on their IRE value. The active gradient dictates the mapping from 0 to 100. This helps gauge exposure based on objective IRE values instead of relative scene luminance.

Use one of the built-in popular false color schemes, or easily create your own gradients and share them with other CineMon users.

## Custom Gradients

{{< screenshot name="false-color-edit" alt="False Color Editing" >}}

CineMon supports an unlimited number of False Color Schemes, in addition to the built-in ones. To create a new False Color Gradient:

1. Duplicate an existing one (from the Actions menu)
2. Show the guide (if not already visible)
3. Tap/Click the Edit button next to the scheme name on the guide
4. Tap/Click on individual color gradient stops to select them
5. Drag them left/right to change their IRE value
6. Tap/Click the color picker to change its color
7. Add new gradient stops to the left or right by tap/clicking on the plus buttons
8. Delete the selected gradient by tap/clicking the red X button

## Options

{{< option-bar-sprite row="10" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Color Scheme | False Color Gradients | `ARRI - Rec.709` | Choose which false color gradient set to use. |
| Actions Menu | `Duplicate`/`Delete` | - | You can duplicate the current scheme or delete any of the custom ones (not the built-in ones). |
| Show Guide | `On`/`Off` | `On` | Toggles the visibility of the Scheme's IRE gradient guide. |

> CineMon ships with popular schemes: ARRI, Atomos, Blackmagic, and a grayscale CineMon default that is a useful starting point for customizing your own.

## Tips

You can calibrate gradients to your specific camera’s log curve. For example, some camera log profiles may render middle gray at 38 IRE. Setting a green color band around that value can simplify getting a neutral exposure when an 18% gray card in the shot, by adjusting lighting or camera settings until the gray card looks green.
