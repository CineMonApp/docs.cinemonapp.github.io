---
title: Image Adjust
weight: 110
---

{{< screenshot name="image-adjust-bw" alt="Image Adjust Tool" >}}

## Overview

This tool provides image adjustment controls. The first set of sliders allow you to adjust exposure, contrast, and saturation. The exposure control works photometrically (requires the input signal gamma curve to be correctly configured in the [preset settings sidebar](/docs/presets)). It can be particularly useful to preview an image that has been purposely over/under-exposed for technical reasons, for instance, when "exposing to the right" (ETTR) by overexposing to saturate the sensor. The second set of sliders control color temperature, tint, and hue.

## Options

{{< option-bar-sprite row="8" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Mode | `Light`/`Color` | Light | Selects which set of sliders are visible. |
| Exposure | `-4`-`+4`EV | 0 EV | Photometrically adjusts exposure in EVs or F-Stops. |
| Contrast | `0`-`2` | 1 | Adjusts the image contrast. |
| Saturation | `0`-`2` | 1 | Adjusts the image saturation. 0 is fully desaturated or B&W. |
| Temperature | `-4000`-`+4000`K | 0 K | Adjusts the color temperature in Kelvin. |
| Tint | `-100`-`+100` | 0 | Adjusts the image tint from green to magenta. |
| Hue | `0`-`100` | 50 | Preforms a hue rotation in CW or CCW directions. |

## Tips

Pull Saturation to zero in combination with **Focus Peaking** for very busy scenes where a single peaking color is not visually distinctive.

## Related Topics

* [Presets](/docs/presets)
* [Focus Peaking](/docs/tools/focus-peaking)
