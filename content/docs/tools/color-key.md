---
title: Color Keyer
weight: 80
---

{{< screenshot name="color-key-comp" alt="Color Key Tool" >}}

## Overview

This tool helps you preview scenes staged in front of a color backdrop (typically green or blue) that will be replaced in post production with a different background. Start with the tool turned off (inactive), and use the color picker to sample an area of the screen that contains the color you want to remove or key out. Then turn on the tool to preview the image with the color replaced by transparency. You can load a background plate to create a simple composite that can help with framing, lighting, etc.

The options let you tweak the effect. Use a lower threshold to identify and fix uneven color and lighting in the background, which can save time in post production. Use higher thresholds to completely remove the background and focus on composition and match lighting the foreground. [Zebras](/docs/tools/zebras) and [Spot Meters](/docs/tools/spot-meter) are alternative tools that can help with this task as well.

## Options

{{< option-bar-sprite row="4" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Key Color | Color | Green | The color to key out. |
| Threshhold | `0%`-`100%` | Low | Control the sensitivity of the keying effect. |
| Soften | `0%`-`100%` | Low | Blurs matte edges for gentler mixes. |
| Despill | `0%`-`100%` | Low | Desaturates the background color from matte edges. |
| Background Plate | File browser | None | Loads an image behind the key. |

## Related Topics
* [Zebras](/docs/tools/zebras)
* [Spot Meters](/docs/tools/spot-meter)
