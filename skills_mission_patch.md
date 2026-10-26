# skills_mission_patch.md: Baruch × NASA mission patch

Entry for the Baruch College ISS patch competition (experiment flying Spring 2027).
Brief: a 3.5″ × 3.5″ patch that represents Baruch College's participation in
scientific research and discovery in space. It must stay recognizable when reduced.
This file is the rulebook for the patch design and for the patch-generator tool.
Source: the user's pencil sketch (circle, big B, partial NASA letters, orbit oval, star).

## 1. Output spec

- Format: PNG, transparent outside the patch circle
- Physical size: 3.5″ × 3.5″
- Pixel size: 1000 × 1000 minimum. Deliver 2100 × 2100 (600 dpi); a 1050 × 1050 (300 dpi) copy is fine for review
- Design space for all coordinates below: 1000 × 1000 units, patch centre (500, 500)
- Patch shape: circle, radius 480, with a 20-unit margin to the canvas edge
- Master file: vector (SVG). Always render the PNG from the SVG, never enlarge a PNG
- Scale test (required): export at 420 / 210 / 105 / 52 px. The B, the red N, the white oval
  and the yellow star must still read at 105 px (about 0.35″). At 52 px only the blue B,
  the red shape and the white ring should be left. Small stars may disappear; that is fine

## 2. Composition (back to front)

1. **Black patch**: filled black circle. The outline is also black (no coloured ring)
2. **Star field**: white dots and white crosses only, in the empty black areas
3. **NASA letters (red)**: the N, plus a cut-off part of the A at the right edge, behind the B
4. **White oval (back half)**: a tilted ring that wraps the lower part of the B and connects to the N
5. **Big B (blue)**: largest element, in front, left of centre
6. **White oval (front half)**: the near half of the ring passes over the B's lower bowl
7. **Yellow star**: four-point star in the middle of the oval, on top of everything

Reading order: B first (Baruch), then the ring and star (orbit, discovery), then N (NASA).

## 3. Elements

| Element | Position (design units) | Size | Colour |
|---|---|---|---|
| B | top-left of its box at (192, 220) | 361 w × 656 h, with a 16-unit offset shadow down-left | Baruch blue, shadow darker blue |
| N | x 617–843, y 376–680 | stroke 56, round caps and joins | NASA red |
| A (cut off) | left leg from (884, 652) rising to an apex near (986, 400) | stroke 56, round; clipped by the patch circle at radius 446 | NASA red |
| Oval | centre (506, 531), tilted −42° (rising to the right) | semi-axes 305 × 60; outer line 16, thin inner line 7 | white |
| Star | centre (500, 537) | radius 38 (four points, pinched waist) | gold yellow |
| Stars | scattered, about 95 | dots r 3.5–8; crosses 18–30 wide, line 3.6 | white |

## 4. Colours (approximate; confirm against brand guides)

| Role | Hex |
|---|---|
| Baruch blue | #1B4FA3 (shadow #0F2F66) |
| NASA red | #FC3D21 |
| White | #FFFFFF |
| Star yellow | #FFC72C |
| Black | #000000 |

Flat colours only; no gradients, no glow. Five colours plus a dark-blue shadow keeps it
embroidery-friendly. Replace the blue and red hex values with the official ones when you have them.

## 5. Typography rules

- **B:** heavy, upright, with a flat left stem. The inside shapes (counters) are rounded
  like the sketch: the top counter is a small rounded D, the bottom counter a larger rounded D.
  The outer corners on the left are only slightly rounded; the right bowls are fully round.
- **N and A:** rounded, with tight curves where strokes meet and round ends, as in the sketch.
  They are drawn with a constant stroke weight. No crossbar on the A.
- No other text on the patch. Letters carry the identity, so keep weights thick enough to read at 0.35″.
- If the official Baruch and NASA letterforms are available and permitted, trace them over the sketch
  positions above. The current letters are traced from the sketch, not from the official logo files.

## 6. Star-field rules

- Only white dots and white crosses; no other shapes
- Keep each star at least 14 units clear of any letter or the ring, and at least 24 units from another star
- Stay inside radius 418 so nothing touches the edge
- A few stars may sit inside the B's counters (they are open black space)
- Density: loose and even, not clustered. Vary sizes (small dots most common, crosses about 30%)
- Embroidery note: a 3.5″ patch is about 89 mm wide, so 17 units ≈ 1.5 mm. Dots under r 4 and the thin inner
  oval line may be too fine to stitch; thicken them for the stitched version

## 7. Do and don't

- Do keep the B as the hero: largest, saturated, in front
- Do let the oval connect B to N: it overlaps both
- Do keep the A cut off by the edge of the patch. Do not shrink it to fit
- Don't add borders, gradients, extra text, or colours beyond section 4
- Don't colour the outline; a black outline on a black field is intentional, so on a dark
  background the patch edge will not show. Fix with a thin light border only if the competition allows

## 8. Use of logos and AI disclosure

- NASA and Baruch marks are protected. Ask the competition organizers whether NASA-style lettering
  or the NASA insignia may appear on the patch before submitting
- Disclose in the entry: sketch and concept by the student; the vector tracing, colour values and
  star placement were generated with Claude from the sketch; hand finishing is by the student

## 9. Prompt template for variations

"Using skills_mission_patch.md, regenerate the patch with [change]. Keep sections 1, 2 and 4.
Export a 2100 × 2100 PNG and the scale test."
Safe variations: star-field density, B shadow direction, oval tilt, one accent colour swap.
