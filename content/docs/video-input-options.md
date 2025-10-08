---
title: Video Input Options
weight: 4
description: Options for connecting external video signals
---

![Video Adapters](/images/docs/CineMon-Connection-Diagram.png)

## Overview

Most modern cameras output HDMI or SDI video. To connect these signals to an iPad or Mac running CineMon you need a video capture adapter/card. CineMon supports **UVC-class** devices, the same plug-and-play protocol webcams use. You simply connect the HDMI or SDI cable to the adapter, and the adapter to the iPad or Mac with a USB cable.

> **Please Note:** A USB-to-HDMI cable is not the same as a video capture adapter. USB-to-HDMI cables are used to send video **OUT** to external monitors from your iPad or Mac. A video capture adapter is used to convert video signals **IN** to the iPad or Mac.

Some cameras and wireless video receivers can output UVC video directly via USB. In that case, no adapter is needed.

> **UVC Video Tip:** If the video source is avaialble as a camera and visible in FaceTime it should work in CineMon.

CineMon also supports other video input options. For instance, Accsoon SeeMo devices are supported via direct integration with the Accsoon SDK. Visit the [Partners Page](https://www.cinemon.app/partners/) on the CineMon website for information on supported partner products.

## Supported Input Options

| Input Option | Examples | Notes |
|--------------|----------|-------|
| UVC Capture Adapter | HDMI/SDI Video Capture Adapters | Considerations: price, latency, color accuracy, compression, frame rates. |
| Native UVC output | Cameras and video transmission systems | Make sure the device is properly configured to output UVC video |
| Accsoon SeeMo Devices | SeeMo, SeeMo 4K, SeeMo Pro | Enable Accsoon device support in the general app settings. Only supported on {{< ipad >}} |
| Built-in Cameras | Back and Front FaceTime cameras | Always available |
| Video & Audio files | .mov, .mp4, .avi | Any file supported by Apple's AVFoundation |

## UVC Adapter Notes

There is no perfect video capture device. The right adapter for you will depend on your use case and workflow. The are several characteristics to consider when choosing an adapter:

| Characteristic | Options |
|----------------|---------|
| Connection type | HDMI, SDI, Both |
| Cost | $10 to $500 |
| Image quality | Highly compressed to lossless |
| Latency | Low (0-1 frame) to Medium (2-3 frames) |
| Form factor | Dongle, box, battery mount |
| Features | External USB PD power |
| Output resolutions | HD (1080), 4K (2160) |
| Supported frame rates | 10-60 |

There are many video capture adapter options available today in a wide range of price points and quality. The good news is that, as new products hit the market, you can easily replace the adapter without changing anything else about yoru monitoring solution. You get to keep all your your settings, configurations, and workflows.

### Tradeoffs

Typical tradeoffs are cost vs. image quality, and resoulution vs. latency. Generally, cheaper adapters deliver more compressed video signals with lower color accuracy. 4K resolution signals tend to have more latency than HD ones.

As of 2025, Inexpensive adapters ($10-$30) can be perfectly adequate for general monitoring and composition. Some of the newer products tend to have relatively low latency, but they tend to suffer from color shifts (they generally bias towards green in the shadows) and show compression artifacts. Slightly more expensive adapters (in the $100 range) can have very good color accuracy and low compression, which is great for image analysis, but may introduce more latency (~2-3 frames), which is not ideal for focus pulling. There are products in the ~$200 range that have excellent color accuracy, no compression, and very low latency. Technology evolves fast and future products will surely improve in all of these dimensions.

### Form Factor

For long monitoring sessions with an iPad you will likely need an external power source. To connect an external power source and a video capture adapter at the same time you will need a USB-C hub, which may require some custom rigging and cable management. Some newer adapters come with an integrated USB-C Hub and PD input power port.

## UVC Native Devices

Some cameras and wireless video receivers can deliver UVC video directly via a built-in USB-C port. If your system supports this, you can connect it directly to your Apple device, without the need for a separate capture adapter.

## Other Input Options

There are other video input options like the Accsoon SeeMo line, which offer a compact, all-in-one adapter with an NP-style battery plate. However, they are not UVC devices and deliver video via an MP4 stream.

Becaues these adapters use proprietary communication protocols, they require additional technical integration to work with CineMon. Visit the [Partners Page](https://www.cinemon.app/partners/) on the CineMon website for information on all supported partner products.