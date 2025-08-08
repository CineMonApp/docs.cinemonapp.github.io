---
title: Image Flip
weight: 14
---

## 1  Overview / Purpose & Usage
Certain rigs—Steadicams, gimbals, and periscope lenses—invert or mirror the camera feed.  Rather than forcing operators to work “upside‑down,” CineMon provides **Image Flip**.  Tap the **Flip V** button to invert vertically; tap **Flip H** for a mirror; tap both for a 180‑degree rotation.  CineMon overlays a subtle HUD icon confirming the active orientation, so you can glance at the monitor and know you are seeing “true north.”

## 2  Options & Modes
| Option | Value Type | Choices | Effect |
|--------|-----------|---------|--------|
| Flip V | Toggle | Off / On | Swaps top and bottom. |
| Flip H | Toggle | Off / On | Swaps left and right. |
| Both Flips | Compound toggle | Off / On | Activates V + H in one tap. |

Internally CineMon applies the transform in the GPU just before scope sampling, ensuring the waveform and histogram reflect the *flipped* view—critical when pulling focus in mirror mode.

## 3  Tips, Best Practices & Use‑Cases
For Steadicam day exteriors, operators often flip **Both** and save that as a preset labelled “Upside Down.”  When the rig transitions to low‑mode dolly later, they swipe to an unflipped preset without diving into menus.  Because CineMon remembers the last state globally, you can close and reopen the app without re‑flipping—a timesaver on fast turnaround sets.

## 4  Related Topics
* [`de-squeeze.md`](de-squeeze.md) – combine when shooting inverted anamorphic  
* [`gestures.md`](../gestures.md) – quick preset swiping to toggle flips
