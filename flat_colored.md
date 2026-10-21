---
name: flat-vignette-style
description: Use when the user wants an animation in the flat vignette style, on any subject: outlined flat shapes on cream in blue, coral, yellow and green, compact scenes on a ground strip, one white object gliding between hard-cut scenes.
---

# Flat Vignette Style

A locked visual and motion style for any subject (places, products, ideas, apps, workplaces, data, stories). Apply the style exactly; only the subject changes. Don't mix in other styles.

## Look

**Palette (exact):**
| Role | Hex |
|---|---|
| Background (cream, fills the whole frame) | `#FBF1DF` |
| Deep blue (main shapes) | `#0156F2` |
| Light blue (secondary shapes) | `#3C76F4` |
| Coral red (accents, roofs, details) | `#FD4B5B` |
| Yellow (ground strip, accents) | `#F9C43E` |
| Green (plants, organic shapes) | `#2AA244` |
| Black (back silhouette layer) | `#000000` |
| White (clouds, the glider, highlights) | `#F5F5F5` |

No gradients, no shadows, no textures. Flat fills only.

**Line:** every shape has a thin dark hairline outline (~2px at 1080 wide), the same weight everywhere.

**Shapes:** simple geometric construction — rectangles, triangles, half-circles, circles. Every subject is reduced to its most recognizable silhouette. Small details (windows, buttons, dots, leaves) are tiny cream/white or colored shapes.

**Composition — the vignette:**
- Each scene is one compact cluster about one idea, sitting on **a single thin horizontal ground strip** (one palette color, outlined), slightly wider than the cluster.
- The cluster has a rounded/dome-like overall silhouette, ~85–90% of frame width, **centered in the middle of the frame** with lots of empty cream above and below.
- Layering, back to front: big **black silhouette** shapes behind → blue main shapes → coral/yellow/green accents → small details on or just below the ground strip.
- **Clouds:** white outlined puffs (several overlapping bumps, flat bottom), 1–3 per scene, tucked behind the top of the cluster at the left and right, partly overlapping it.
- A few small moving details live on the ground line (something that slides, bobs or turns).

**Format:** vertical (2:3 or 9:16). The vignette stays in the middle third.

## Motion

**Connective glider:** one white, outlined object glides through every scene on a smooth curved path and carries the viewer from scene to scene (the original uses a paper plane; use it, or another simple white outlined object that fits the subject). It is the only thing that travels between scenes. Glide is smooth and continuous (`sine.inOut` / `power1.inOut`), with slight banking/rotation along its path.

**Scene changes:** **hard cuts.** As the glider crosses, the next scene appears complete in one frame — no wipes, no fades, no build-up animations. The glider keeps its motion across the cut.

**Inside a scene (subtle):**
- Slow camera drift/push on the whole vignette (scale ~1 → 1.03 over the scene).
- Clouds drift a few pixels sideways.
- One or two small secondary loops (slide, bob, turn).
- Nothing pops, bounces or enters — the scene is already built; only gentle ambient motion.

**Pacing:** ~1.2–1.8s per scene. Steady rhythm, cut on the glider's crossing. End on a scene that holds with its ambient motion running.

## Building a scene

1. Pick the scene's idea and its 2–4 most recognizable shapes.
2. Draw the black silhouette backdrop, then the blue main shapes, then coral/yellow/green accents, then the ground strip (colored, outlined) and small details.
3. Add 1–3 outlined clouds behind the top edge.
4. Check: palette only, hairline outlines on everything, centered dome-shaped cluster on one strip, lots of cream space.
5. Plan the glider's path through the scene and the cut frame to the next one.

Build and export with the motion-graphics-director workflow (SVG on a fixed stage, one seekable timeline, MP4 export).
