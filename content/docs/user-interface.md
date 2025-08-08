---
title: User-Interface Overview
weight: 2
description: A visual tour of CineMon’s main window so you know exactly where every control lives before heading on-set.
---

# CineMon UI Overview

CineMon’s layout is deliberately minimal: **picture first, controls second**.
Yet every monitoring function—from scopes to false-color—lives no more than a single tap or key-press away.
This page walks you through each region of the interface, explains what it does, and links out to deeper documentation.

---

## 1. Primary Screen Elements

| UI Area | Location | Purpose |
|---------|----------|---------|
| **Live Image Canvas** | Centre | Shows your camera feed; supports pinch-zoom and drag. |
| **Video-Assist Toolbar** | Bottom (iPad/iPhone) • Left edge (Mac) | Houses toggles for overlays and look tools. |
| **Scopes Bar** | Right edge | Quick access to Histogram, Waveform, Vectorscope, Quad Scope. |
| **Mini-Map** | Top-left (auto-shows on zoom) | Indicates your zoomed-in viewport relative to full frame. |
| **Sidebar** | Left-edge swipe or ☰ button | Opens Organizer, Settings, About, and Help. |
| **Slide-Out Drawers** | Under each toolbar icon | Reveal per-tool options when you drag the icon upward. |
| **HUD Status Badges** | Top-right overlay | Shows active LUT slot, de-squeeze ratio, flip state, and frame-rate warnings. |

---

## 2. Navigating the Interface

The very first time you launch CineMon you’re dropped into a **Clean Feed** preset—only the Video-Assist toolbar is visible.
Here’s how you unearth everything else:

* **Activate a Tool** – Tap any icon once.
  The overlay animates on-screen and the icon glows blue to confirm it’s live.
* **Adjust Tool Options** – Drag the same icon *upward*; a drawer “snaps” into place under your finger, exposing sliders, colour pickers, or file loaders.
  Drag downward or tap outside the drawer to dismiss it.
* **Open a Scope** – Tap a scope icon on the right; the floating window appears directly under your pointer.
  Pinch to resize; drag to reposition; double-tap to open that scope’s own settings or to make it full-screen.
* **Hide the Chrome** – Double-tap anywhere on the picture and both toolbars slide away, perfect for operator-only viewing or clean screenshots.
  Double-tap again to bring them back.
* **Swipe for Presets** – With one finger on the picture, swipe left or right.
  CineMon flips through the Configuration Preset carousel, animating active tools so clients *see* what changes.

---

## 3. Slide-Out Drawers in Detail

A drawer always belongs to the icon you pulled.
If you pin open multiple drawers they stack in a tidy strip; CineMon remembers their order when you reload the preset.

* **Real-time Updates** – Change a slider and watch the live image respond instantly—no “Apply” button.
* **Contextual Help** – A small 〔?〕 badge in each drawer’s corner links to the specific doc page for that tool, opening in-app.
* **Persistent per Preset** – Drawer state (open/closed) is saved with the preset, so a “Scopes” preset might launch with Waveform and Vectorscope drawers already expanded.

---

## 4. Sidebar Modules

Swipe from the far left edge or tap the ☰ button to open the Sidebar. It contains four tabs:

1. **Organizer** – Manage Configuration Presets, Display LUTs, and False-Color Gradients.
2. **Settings** – Global pipeline controls (Log curve, data vs full levels, latency).
3. **About** – Version, build number, EULA, and credits.
4. **Help** – Direct links to this documentation and troubleshooting guide.

The Sidebar is *modal*; CineMon pauses gesture recognition elsewhere so you can’t accidentally change exposure while renaming a preset.

---

## 5. Keyboard & Gesture Equivalents

On iPad/iPhone you’ll rely on touch, but on Mac the following shortcuts keep your hands on the keyboard:

| Shortcut | Action | Touch Equivalent |
|----------|--------|------------------|
| `Space` | Hide/show toolbars | Double-tap |
| `← / →` | Previous / Next preset | Swipe left/right |
| `⌘1 – ⌘9` | Toggle first nine tools | Tap icon |
| `⌘⇧H` | Toggle Histogram | Tap Histogram icon |
| `F` | Full-screen current scope | Double-tap scope |

---

## 6. Latency and Performance Indicators

A tiny **green, amber, or red dot** in the HUD shows end-to-end latency health:

* **Green** &lt; 50 ms – Ideal for focus pulling.
* **Amber** 50–90 ms – Acceptable for composition.
* **Red** &gt; 90 ms – Consider lowering camera output resolution or moving the *Pipeline* slider toward **Latency** in Settings.

Frame-rate mismatches (e.g., 29.97 fps source on a 60 Hz display) trigger a small ⚠︎ icon; hover (Mac) or long-press (iPad) to see the exact rate disparity.

---

## 7. Customising the Layout

*Drag-and-drop* scopes anywhere—even onto a second monitor via Stage Manager or Sidecar.
Toolbars can be flipped (top ↔ bottom on iPad; left ↔ right on Mac) in **Settings › Interface**.
Your layout preferences save automatically into the current Configuration Preset, so every scene can launch with its own personalised workspace.

---

## 8. Where to Go Next

You now know the neighborhood—time to explore the houses:

* **Tools Section** – Learn how Grid Overlay, False Color, Focus Peaking, and friends live inside those toolbar icons.
* **Scopes Section** – Master Histogram vs Waveform vs Vectorscope positioning and tuning.
* **Presets & Organizer** – See how to snapshot your entire UI and share it with the rest of the camera crew.

CineMon’s UI is built for speed and muscle memory; after a day of use you’ll instinctively swipe, pinch, and tap your way through complex monitoring tasks without looking away from the shot.