---
title: Zebras
weight: 100
---

{{< screenshot name="zebras-all" alt="Zebras Tool All" >}}

## Overview

**Zebras** are an exposure assist tool that layer diagonal stripes over pixels that fall above or below chosen luma thresholds. The **Hi/Lo** mode can warn of clipping whites or crushed shadows. The **Band** mode highlights an IRE range, useful for nailing middle gray or skin tones.

Use the options to customize the shadow/highlight IRE values, or the target IRE value and band width. Both modes can be active at once and the zebra colors are individually customizable.

## Options

{{< option-bar-sprite row="6" >}}


| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| Mode | `Hi/Lo`/`Band` | Hi/Lo | Selects which zebras mode to configure. |
| Active | `On`/`Off` | On for Hi/lo, Off for Band | Activates the current zebras mode. |
| Shadow IRE Threshold | `0`–`50`% | 0% | Pixels *below* this IRE show Shadow zebras. |
| Highlight IRE Threshold | `50`–`100`% | 100% | Pixels *above* this IRE show Highlight zebras. |
| Shadow Color | Color | Blue | Tint of shadow stripes. |
| Highlight Color | Color | Black | Tint of highlight stripes. |
| IRE Target | `0`-`100`% | 65% | IRE target for band zebras. |
| Band Width | `1`-`50`% | 5% | Percentage above and below IRE Target to highlight. |
| Band Color | Color | Black | Tint of the band stripes. |