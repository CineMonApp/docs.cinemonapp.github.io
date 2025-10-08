---
title: Image Overlay
weight: 70
---

{{< screenshot name="overlay-blend" alt="Overlay Tool" >}}

## Overview

This tool overlays an image on top of the input signal. You can *tap/click* the camera icon to take a snapshot of the current frame and use that as the overlay, or load a saved image from a file. This can be useful for aligning the camera position or an in-frame object with a previous reference, or for comparing composition, color, or exposure values.

This tool can use two different blend modes for the overlay: normal mix and difference.

Additional options provide control of the opacity, wipe amount and angle of the overlay.

{{< screenshot name="overlay-difference-wipe" alt="Overlay Tool" >}}

> A small thumbnail of the currently loaded reference frame is shown in the reference frame well on the options drawer.

## Options

{{< option-bar-sprite row="3" >}}

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Take Snapshot | - | - | Takes a snapshot of the current image and stores it in frame memory. |
| Snapshot Actions | `Save`/`Clear`/`Load` | - | Actions to take on the contents of frame memory. |
| Blend Mode | `Mix`/`Difference` | `Mix` | Overlay blend mode to use. |
| Opacity | `0%` to `100%` | `50%` | Controls the transparency of the frame overlay. |
| Wipe Amount | `0%` to `100%` | `100%` | Controls the overlay wipe amount across the image. |
| Wipe Angle | `-90°` to `+90°` | `0°` | Controls the angle of the wipe. |
| Swap Source/Snapshot | `On`/`Off` | `Off` | Inverts the compositing order of the source and snapshot. |
| Difference Color | Color | Red | Controls the color of the difference hightlight. |
