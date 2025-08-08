---
title: Safe Area
weight: 12
---

## 1  Overview / Purpose & Usage
Broadcast engineers invented the **Safe Area** box to stop credits and supers from being chopped off on mismatched domestic televisions.  Today the concept survives in streaming, live‑graphics, and LED‑wall control rooms.  
In CineMon you enable the overlay by tapping the **Safe** icon; a rectangle pops onto the screen sized to whatever percentage you last used.  Dragging upward reveals the familiar option drawer where you dial in the exact “Safe Percentage,” choose a compliance colour such as legal yellow, and tone down opacity so on‑set talent barely notices it.

## 2  Options & Modes
| Option | Value Type | Range / Choices | Explanation |
|--------|-----------|-----------------|-------------|
| Safe % | Integer slider | **50 – 100 %** | Scales the rectangle relative to the *current* aspect ratio. 90 % is Action‑Safe; 80 % is Title‑Safe. |
| Line Colour | RGBA swatch | Full palette | The stroke colour of the rectangle. Yellow is industry standard. |
| Opacity | Percentage slider | **0 – 100 %** | Transparency of the rectangle lines. |

Setting **Safe %** to 90 creates a box whose edges sit at 90 percent of the width and height of whatever crop is active—swap from 16 : 9 to 2.39 : 1 and the box neatly scales down.  If you need two boxes (Action *and* Title) simply store them as separate presets and swipe between them; CineMon’s animated transition makes it clear which is which.

Colour and Opacity are rendered using the display‑space primaries, so the yellow you pick on an iPad Pro will match a calibrated OLED fed from CineMon for Mac—critical when the shader wants confidence that graphics won’t flutter in HDR deliverables.

## 3  Tips, Best Practices & Use‑Cases
A clever workflow is to leave Safe Area at 95 % during blocking—this “virtual matte” keeps boom poles and reflector frames just outside audience view—then drop to 90 % after lighting to check that titles still clear.  Because the box is drawn after all scaling, you can even rotate an iPhone to portrait and watch the rectangle reorient live, ensuring vertical deliverables remain compliant.

## 4  Related Topics
* [`aspect-ratio.md`](aspect-ratio.md) – the crop bars that reshape the safe box  
* [`grid-overlay.md`](grid-overlay.md) – gives extra guidance lines inside the safe rectangle
