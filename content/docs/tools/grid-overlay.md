---
title: Grid Overlay
weight: 10
---

## 1  Overview / Purpose & Usage
The Grid Overlay sprays an evenly‑spaced lattice of vertical and horizontal guide lines across your live video.  Cinematographers lean on these grids to honour the classic **Rule‑of‑Thirds**, centre symmetrical products, or divide the frame into equal cells for multi‑host interviews.  
Turn the feature on by tapping the **Grid** icon in the Video‑Assist toolbar.  CineMon immediately remembers—and re‑applies—the last grid you used; a gentle snap animation shows that the overlay is active.  Drag the icon upward and a drawer slides out beneath your finger, giving you direct manipulation of line counts and appearance.  As you move each slider, the grid updates in real time, so you never lose sight of composition while you tweak.

## 2  Options & Modes
The quick reference table lists the adjustable parameters; the paragraphs that follow explain why you would reach for each one.

| Option | Value Type | Range / Choices | Role in the Overlay |
|--------|-----------|-----------------|---------------------|
| Vertical Lines | Integer slider | **1 – 10** columns | Sets the number of equally‑spaced *columns*. |
| Horizontal Lines | Integer slider | **1 – 10** rows | Sets the number of equally‑spaced *rows*. |
| Line Colour | RGBA swatch | Full colour & alpha | Controls the hue the grid is rendered in. |
| Opacity | Percentage slider | **0 – 100 %** | Makes the lines fully solid (100 %) or ghosted (0 %). |

**Vertical & Horizontal Lines** The sliders accept whole numbers because fractional divisions are visually confusing in a moving frame.  Choose **3×3** for a textbook thirds layout; choose **5×5** when you need finer granularity—common on beauty commercials where eyes, lips, and products all demand their own horizontal bands.

**Line Colour** Tap the colour thumbnail to open the system picker.  A neon cyan pops on location exteriors, whereas a warm amber avoids clashing with tungsten house lights.  Because CineMon decouples colour and transparency, you can keep a bold hue and simultaneously lower opacity so the grid feels airy instead of oppressive.

**Opacity** Full‑strength lines are ideal when blocking the first master shot of the day.  Once composition is locked, many camera operators pull opacity to 20–30 percent; the guide remains visible to them but vanishes to less‑trained eyes crowding around the monitor.

## 3  Tips, Best Practices & Use‑Cases
CineMon renders the grid *after* image transformations but *before* scopes.  That means when you enable **Aspect Ratio Guides** the grid automatically re‑calibrates itself to the visible crop—no math in your head, no offsets to dial.  
A popular preset routine is to save “Thirds” and “Fifths” as separate **Configuration Presets**.  During a rehearsal you can swipe left or right on the picture to morph between the two; CineMon cross‑fades the lattice so the director can decide which composition better serves the story.  If you pinch‑zoom to inspect focus, beware that the grid re‑centres on the newly cropped window—great for macro work, but remember to zoom back out before you roll!

## 4  Related Topics
* [`aspect-ratio.md`](aspect-ratio.md) – crop bars that respect the same thirds  
* [`safe-area.md`](safe-area.md) – broadcast boxes that sit inside the grid
