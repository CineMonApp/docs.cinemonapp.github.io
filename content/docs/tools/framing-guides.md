---
title: Framing Guides
weight: 40
---

{{< screenshot name="framing-guides-passepartout" alt="Framing Guides Tool" >}}

## Overview

Modern productions often finish in multiple aspect ratios: a 2.39:1 theatrical master, a 16:9 television pass, and vertical 9:16 teasers for social.

The **Framing Guides** can help you compose a frame for different aspect ratios than the one being captured. For example, if your project calls for a 2.29:1 wide screen image you can use this guide to preview the area of the image that will remain visible after the original image is cropped in post.

You can configure up to two different aspect ratios guides (A & B) simultaneously. For each guide you can control it's aspect ratio, size and position within the image frame.

> **IMPORTANT NOTE:** Even if the guides are enabled in the Framing Guides options drawer, they won't be visible until the Faming Guides tool button is activated.

> **Frame A** is used as the base frame to render all other composition tool guides. As you change the size, position, or aspect ratio of Frame A, all other guides will adjust accordingly.

## How to use

The options drawer offers a few aspect ratio presets as shortcuts, including square, and vertical for social media. You can also tap the aspect ratio button to enter a custom value as a fraction. Use the lock button to constrain the aspect ratio when resizing the guides.

{{< screenshot name="framing-custom-aspect" alt="Framing Guides Tool" >}}

Other options allow you to configure how the guides are rendered, with independent color and opacity controls for the frame outline and the out-of-frame regions (or matte).

To edit the guides, the options drawer needs to be open. It shows controls for one guide at at time. You select which guide to edit (labeled `Frame A` or `Frame B` on screen) with the segmented picker. The one currently being edited will have a solid border and the other one will have a dashed appearance.

{{< screenshot name="framing-edit-a-b" alt="Framing Guides Tool" >}}

To postion the active guide, *drag* it from its center marked by crossed arrows. To resize the active guide, use a *pinch-to-zoom* gesture, or *drag* any of its corners or edges. The guide will resize around its center.

> If the guide is flush against one of the image borders, you might need to move it before resizing.

## Relationship To Crop Viewers

Even when the Framing Guide tool is inactive, you can use the [**Specialized Crop Viewers**](/docs/user-interface#specialized-viewers) to display a cropped view of the input image. The crop viewers use the size and position of the enabled framing guides to crop the image.

{{< screenshot name="layout-2x1-custom-3" alt="Framing Guides Tool" >}}

## Options

{{< option-bar-sprite row="0" >}}

| Option | Values | Default | Description |
|--------|-----------|-----------------|--------|
| Guide Selector | `A`/`B` | `A` | Select which Framing Guide to edit. |
| Enable | `On`/`Off` | `On` (for `A`), `Off` (for `B`) | Enable or disable the current Framing Guide. |
| Custom Aspect Ratio | Numerator/Denominator Fraction | - | Shows a pop-over to customize the aspect ratio as a fraction. |
| Lock Aspect Ratio | `On`/`Off` | `Off` | Locks the aspect ratio so that resizing operations maintain the frame proportions. |
| Matte Color | Color/Opacity | Black, 90% | The color and opacity of the matte that is rendered over the portion of the image that falls outside the guide. |
| Frame Color | Color/Opacity | White, 50% | The color of the frame guide itself. |
| Aspect Ratio Presets | [`2.39:1`, `1.85:1`, `16:9`, `1.66:1`, `3:2`, `4:3`, `1:1`, `9:16`] | - | Shortcuts to popular, full-screen aspect ratios. |

> Selecting a **Preset** recenters and resizes the guide to fit the image.

## Tips

To monitor two aspect ratios at once:

* Configure Frame A & B and show them as outlines only.
* Configure Frame A & B and use a 2x1 (side-by-side) with crop viewers to to visualize both crops.
* Configure two different presets, each with a different Framing Guide configuration, and switch between them.

## Related Topics

* [**Specialized Crop Viewers**](/docs/user-interface#specialized-viewers)
* [**Composition Guides**](/docs/tools/composition-guides)
* [**Center Mark**](/docs/tools/center-mark)
* [**Safe Area**](/docs/tools/safe-area)
