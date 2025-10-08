---
title: Test Strip
weight: 130
---

{{< screenshot name="test-strip-7" alt="Test Strip Tool" >}}

## Overview

Inspired by photochemical printing practices, this tool breaks up the image into a series of strips with exposure adjustments in constant increments. This makes it very easy to preview the image at different exposure levels. Test Strip requires the image's Gamma curve to be correctly configured in the [Preset Settings](/docs/presets) to show accurate exposure increments.

## Options

{{< option-bar-sprite row="7" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Strip Orientation | `Vertical`/`Horizontal` | `Vertical` | Orientation of the test strips. |
| Number of Strips | `2`-`11` | `7` | The number of test strips to render. |
| EV Delta | [`½`, `1`, `2`] | `½` | The EV or F-stop diffence between each test strip. |
| Invert Direction | `On`/`Off` | `Off` | Invert the direction of exposure gradient (dark to light). Default when off is Left to Right/Top to Bottom depending on the orientation. |
| Show Labels | `On`/`Off` | `On` | Show the EV/F-stop labels for each strip. |

> As mentioned above, Test Strip requires the image's Gamma curve to be correctly configured in the [Preset Settings](/docs/presets) to show accurate exposure increments.

## Related Topics

* [Preset Settings](/docs/presets)
