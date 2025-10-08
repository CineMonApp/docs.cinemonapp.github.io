---
title: Release Notes
weight: 99
---

## v1.7.0
### Highlights
The OS26 release! CineMon v1.7.0 includes several enhancements and UI tweaks to work better with the latest version of iOS/iPadOS 26 and macOS 26 (Tahoe), including a complete set of menu commands for iPad for those of you who use it with a keyboard and mouse/touch pad. This version also includes a new 1x2 layout option (top/bottom), new presentation sheets for the CineMon PRO store, app settings (on iPad). And a new liquid glass app icon and a new startup screen image.

### New features
- Added a 1x2 layout option for stacking two viewers top/bottom
- iPad now has a full menu bar and keyboard shortcut commands (OS26+)

### Enhancements
- Updated the overlay sheet UI for several screens (app settings, CineMon PRO Store, Video Monitoring feature guide).

### Bug fixes
- Fixed custom aspect ratio pop-over bug in the Framing Guide options drawer

## v1.6.0
### Highlights
CineMon v1.6.0 now supports Accsoon SeeMo devices on iPad. This has been one of the most popular user requests since the app was announced. In addition to UVC video sources, you can now use a SeeMo, SeeMo 4K, or SeeMo Pro as input sources in CineMon running on iPad. The Accsoon SeeMo family of devices combine video input capture and an NP-style battery port in a compact form factor.

To enable Accsoon devices:
1. Open the app settings and select the new Sources Tab
2. Turn on "Enable Accsoon SeeMo Devices"
3. A new Accsoon section will be added in the Video Sources pane
4. A connected SeeMo device will appear in the new section
5. Tap the power button to start SeeMo video

### New features
- Added Support for Accsoon SeeMo devices

### Bug fixes
- Recent files list was not being properly refreshed when files changed

## v1.5.0
### Highlights:
CineMon v1.5.0 introduces movable and resizable framing guides and Crop Views. To get started, make sure you have the Viewer visible in one of the screen panels, then open the Framing options bar to reveal the new frame edit UI. Select which frame you want to edit (A or B) and turn it on. You can intuitively reposition a frame by dragging it. You can also use pinch-to-zoom, or drag from the corners or sides to resize it uniformly around the center. Use the lock button on the Framing options bar to constrain the aspect ratio of the guide. Once you have your guides customized, sized, and positioned, you can turn on the Framing Guides tool to overlay them in the viewer.

v1.5.0 also introduces a new layout view type to display a cropped version of the main image controlled by the framing guides. Just select Frame A or Frame B as the view type for any screen panel. This can be particularly useful in the Grid layouts, where you can have two different crops side-by-side, to preview different aspect ratios simultaneously, for instance.

This version also introduces luma range controls for the Vectorscope, which allow you to decide which subset of luma values to display. You can select from All (the default), Low, Mid, and High, and use additional controls to tune the low and high ranges.

There is now also a global app setting for controlling how the option bars interact with the main layout area. They can overlay it (traditional) or stack on top/bottom.

### New features:
- Framing guides can now be moved and resized
- New view types for displaying frame A/B crops of the main image
- Vectorscope luma range controls

### Enhancements:
- Global app setting for tool option bars layout options

## v1.4.0
### Highlights:
Introducing View Layouts! CineMon v1.4.0 includes a brand new layout engine inspired by your own suggestions. People have been asking for a way to show the image viewer in one of the 4-Up view quadrants. You can now right-click (on a Mac)/long-press (on an iPad) on any viewport to select from a list of view types, including Source, Viewer, R/G/B/A Channels, and Scopes. You can also resize the viewports by dragging the dividers. There is also a new 2x1 (side-by-side) layout. To switch layouts use the Layout Menu on the Status Toolbar (next to the Scopes buttons), or the Window menu on the Mac menubar.

This release also includes a revamped display stage that should render 10-bit sources with higher fidelity, and deliver higher performance, with lower processor/GPU load, and lower memory usage! If you never noticed any slowdowns with CineMon you might not notice a difference, but everything should just run faster and feel snappier.

Additional enhancements include updated menu items on Mac, and enhanced Focus Peaking and Image Overlay implementations. Loaded reference images will now auto-resize to fit the current source dimensions.

### New features:
- New layout engine with single, 2x1, and 2x2 grids, resizable and configurable viewports
- R/G/B/A channel views
- Source view
- New high-performance display stage

### Enhancements:
- New icons for menu items on the Mac and layout view options
- New Focus Peaking implementation
- New Image Overlay implementation with auto-resize snapshots

## v1.3.0
### Highlights:
CineMon v1.3.0 introduces a new exposure assist tool called Test Strip. It was inspired by photochemical printing and the process or exposing adjacent strips of photo paper to progressively longer times to fine tune the desired exposure. The new tool breaks up the image into a series of vertical or horizontal strips that have their exposure adjusted in constant increments. This makes it very easy to see, at-a-glance, what the image will look like with a range of exposure values applied. To work accurately, Test Strip requires the image's Gamma curve to be correctly configured in the preset settings. Try it out!

### New features:
- Test Strip assist tool for at-a-glance exposure adjustment evaluation

### Bug fixes:
- Zebras were not being initialized to default state

## v1.2.1 / v1.2.0
### Highlights:
CineMon v1.2.1 can now transform the calibrated input signal’s Gamma and Color Space to a different combination. This is typically used to convert from the camera’s scene-referred space (such as ARRI LogC4) to a display-referred gamma/gamut (such as Rec.709 or P3) for preview. LUTs are often used for this purpose but the Color Space Transform (CST) performs a precise mathematical conversion using the manufacturer’s specifications. You can still apply a display LUT after the CST. Other new features in v1.2.1 include new color adjustment tools (temperature, tint, hue), and the ability to activate both Zebra modes simultaneously. It also includes various enhancements and optimizations to existing  features.

### New Features:
- Color Space Transform function with support for 21 gamma curves and 16 color spaces.
- New color adjustment controls for temperature, tint, and hue
- Support for simultaneous Zebra modes

### Enhancements:
- Platform-specific UI improvements to the Presets Sidebar
- New RGB Overlay Waveform implementation that is less GPU intensive
- Improved UI control slider performance, especially on Mac
- Optimized pixel buffer format for video playback
- Minor change to the Zebras tool icon
- Increased the Vectorscope trace brightness upper bound
- Added Save and Revert Preset menu options and keyboard shortcuts for Mac
- Expanded hit box and improved layout of media playback controls

### Bug Fixes:
- Fixed overlapping frame buffering during camera authorization at app start

## v1.1.1
### Highlights:
CineMon v1.1.1 release notes:

Tetrahedral LUT interpolation! This is the first CineMon minor version update and includes some minor feature additions, enhancements, and bug fixes.

Most notably, CineMon now supports Tetrahedral interpolation for LUTs. This mode renders higher quality images (most noticeably in subtle gradients) but requires higher GPU utilization, which contributes to slightly faster battery drain. It also allows iPads to use up to 65 point LUTs. You can set the interpolation type for the Calibration LUT and the Display LUT independently in the Preset Settings sidebar.

This version also adds Forward and Backward (1x, 2x, 4x, 8x) video playback controls by pressing the buttons to cycle through the speed modes. On Macs, you can also use the JKL keys for Back/Pause/Forward.

### New Features:
- Tetrahedral Interpolation option for LUTs
- Support up to 65 point LUTs on iPad using Tetrahedral Interpolation
- Fast forward/rewind video playback with new controls

### Enhancements:
- Added new app setting to enable/disable swipe-to-cycle Presets
- Enhanced video playback quality by switching pixel buffer formats
- Added long-press gesture to open/close tool options bars (in addition to swipe)

### Bug Fixes:
- Fix a bug where video will always auto-play on iPad app start, regardless of auto-play setting

## v1.0

Initial release.