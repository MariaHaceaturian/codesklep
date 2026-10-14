# skills.md — Das Schweizer Plakat (Wolfgang Weingart, 1984)

Source poster: Wolfgang Weingart, *Das Schweizer Plakat*, 1984, offset lithograph,
120 × 84.1 cm (MoMA collection). Made for an exhibition at the Gewerbemuseum Basel /
Museum für Gestaltung, 24 January – 11 March 1984.

## 1. Canvas & Grid

- Format: portrait, ratio ≈ 1 : 1.42 (close to an ISO A-size, e.g. A1 594×841mm)
- Outer border: uniform cream/aged-paper margin, ≈ 5–6% of width, broken on the
  right edge by a bleeding red/white checkerboard stripe and at the top-left
  corner by a diagonal torn/lightning-bolt tear
- Live image area: top ~78% of canvas height
- Text zone: bottom ~22% of canvas height, baseline-anchored
- Horizontal split for the headline: left column (flush-left, ~0–55% width)
  carries "Das" / "Schweizer"; the right portion (~55–100% width) carries
  "Plakat," overlapping the illustration
- Small print (venue, dates) is right-aligned to the right margin, stacked two
  lines, sitting just below and right of "Plakat"

## 2. Typographic Scale

Rule: pick **one** typeface for the whole poster — it's used across the
headline and the caption, no mixing. Three options, no role labels attached
to any of them:

- **Archivo** — variable, wght + wdth axes. Grotesque bold, free stand-in for
  the original's Helvetica / Neue Haas Grotesk Bold.
- **Inter** — variable, wght axis only. Clean contemporary grotesque.
- **Bodoni Moda Italic** — variable, opsz + wght axes, italic glyphs. A
  modern-serif-italic direction, a deliberate departure from the original's
  grotesque for a more editorial feel.

Canvas reference: 1200 × 1700px (≈ the poster's 1:1.42 ratio). Scale all three
size tiers together if you resize — don't adjust one tier independently, or
the ratio breaks.

| Tier | Content | Weight (within whichever font is active) | Size | Leading |
|---|---|---|---|---|
| H1 (display) | "Das" / "Schweizer" / "Plakat" | Bold-leaning (Archivo 700 / Inter 700 / Bodoni Moda 600) | 220px | 0.92 |
| H2 (subhead) | "1900–1984" | One step down from H1 | 90px | 1.0 |
| Caption | "24. Januar – 11. März 1984," "Gewerbemuseum Basel," "Museum für Gestaltung" | Medium (500) | 24px | 1.3 |

Ratio ≈ 1 : 0.41 : 0.11 — close to the eye estimate from the scan. On
Archivo, the headline also uses a slightly condensed width (wdth 87) for the
tight, stacked Swiss feel; Inter and Bodoni Moda Italic don't have a width
axis, so that detail only applies when Archivo is the chosen font.

Size and opacity are both adjustable per-poster in the tool (Text filter):
size scales all three tiers together (50–150%), and opacity applies to the
headline only — the caption keeps its own fixed reduced opacity (see below).

Size variants (scale all three tiers together):

| Variant | H1 | H2 | Caption |
|---|---|---|---|
| Compact | 190px | 78px | 20px |
| Default | 220px | 90px | 24px |
| Bold/Large | 250px | 104px | 28px |

Letterform detail: small negative-space shapes are cut into the display type
(H1) — plus signs, rectangles, and circles knocked out of the letterforms so
the background shows through. Applied sparingly, not on every letter — a
handful of cutouts per word is enough to read as intentional rather than
decorative noise.

Caption opacity: the small date/venue text is reduced in opacity (≈ 55–65%
of full black) rather than set at full solid — gives it a printed, receding
quality against the display type.

## 3. Color Palette

Estimated by eye from the scan — verify against a color-picked source if
precision matters:

| Role | Where it appears | Approx. hex |
|---|---|---|
| Primary red/orange | dominant wash across the illustration and border stripe | #E5482E |
| Golden yellow | tear/lightning shape, border accents | #F2B705 |
| Mustard/olive | sun-disc fill | #9B8B1F |
| Green | crescent moon, lower cloud gradient | #6E8B3D |
| Blue (minor accent) | sliver at top-left border edge | #3A6EA5 |
| Black | type, crown shapes, chimney silhouettes | #000000 |
| Cream/off-white | border, "paper" ground, negative space in clouds | #F3EAD8 |

Texture rule: the illustration is built from a coarse offset halftone/rosette
pattern — flat color fields with visible dot structure, not smooth gradients.
The border and type stay flat and clean by contrast.

Texture options (tool, Texture filter — one size slider controls the scale
of whichever is active):

- **Dot Screen / Polka Dot Grid** — the default halftone: jittered circles,
  size and opacity driven by local darkness. Closest to the original's offset
  rosette.
- **Screen Tone / Manga Tone** — a regular, unjittered dot grid, size only
  (no opacity variation) — the flatter, graphic look of manga screentone.
- **Line Screen / Engraving Lines** — horizontal bars instead of dots,
  thickness driven by local darkness — an engraving/line-screen print feel.

All three apply equally to the procedurally generated scene and to an
uploaded photo rendered in halftone (see Upload, below).

Scattered marks: small black shapes — thin random lines, triangles, and other
irregular marks — are scattered through the halftone illustration, sized and
placed to read as part of the artwork (like the crown and chimney shapes),
not as separate graphic elements layered on top.

Border options (tool, Border filter): color is chosen from whichever
palette colors are currently active in the Color filter (default cream,
matching the original); size is the existing thickness slider; and style has
four options — **Uniform** (equal thickness on all sides, as in the
original), **Asymmetric** (each side a different, randomized thickness),
**Circles** (a trim of small circles along the top and bottom bands), and
**Triangles** (a zigzag trim along the top and bottom bands). All four keep
the torn top-left corner and the bleeding right-edge stripe from rule 6
below.

## 4. Explicit Composition Rules

1. Flush-left set the display type; never center it.
2. Keep leading on the display type tight enough that line 2 nearly touches
   line 1's descenders.
3. Let at least one headline word overlap or bleed into the illustration — no
   solid background plate behind it, just enough tonal contrast in the art
   underneath to stay legible.
4. Reserve the bottom band (~20–25% of the canvas) for text; keep the rest of
   the canvas as unbroken image.
5. Introduce one controlled "tear" or diagonal break in the image or border —
   an intentional disruption of the frame, not a decorative flourish.
6. Keep a thick, aged-paper-toned border around the whole piece; let at least
   one edge bleed with a contrasting pattern (stripe/checkerboard) to break the
   frame's uniformity.
7. Mix representational/collage imagery (mountains, clouds, celestial bodies)
   in halftone with hard-edged graphic shapes (bolts, crowns, crosses) — this
   texture contrast is part of the system, not decoration.
8. Small print (date, venue) stays small, tight, right-aligned, and
   subordinate — never competing with the display type.
9. Palette: one dominant warm hue (red/orange) covering more than half the
   image area, one bright secondary (yellow), and small doses of two
   cool/muted accents (green, blue) — plus black and cream for type and border.
10. Cut small knockout shapes (plus signs, rectangles, circles) into the
    display letterforms, sparingly — a few per word, not every letter.
11. Set the small date/venue text at reduced opacity (≈ 55–65%), not full
    solid black.
12. Scatter small black marks (thin random lines, triangles, irregular
    shapes) through the halftone illustration so they read as part of the
    artwork, not as a separate overlay.

## 5. Upload (tool feature)

The Upload filter lets a user's own photo replace the generated mountain /
cloud / sun scene entirely. The photo is re-rendered using whichever texture
type is active (dots, screen tone, or line screen) and recolored to the
nearest match among the currently active palette colors — it never keeps the
photo's original colors. The scattered black marks, cross, border, and
headline still draw on top as usual.

## 6. Live-data mode (quake_poster_generator.html)

A separate tool built from the same generator. The poster's elements are
driven by the USGS earthquake feed instead of random numbers. The original
poster_generator.html is unchanged.

Data source: `https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/{2.5|4.5|all}_day.geojson`
(free, no key, refreshed by USGS about once a minute; the tool polls every 60 s).
Fields used: `properties.mag / place / time / tsunami / url`, `geometry.coordinates = [lon, lat, depth km]`.

| Data | Poster element |
|---|---|
| One quake | One peak (mountain) |
| Magnitude | Peak height and width; headline weight (regular → semibold, capped at 750) |
| Depth | Peak colour: shallow = red, then yellow, olive, green, deep = blue |
| Longitude / time / magnitude rank | Peak x-position (Layout option; Generate can shuffle between them) |
| Strongest quake | The sun (disc), tied to its peak by a hairline |
| Newest quake | The crescent moon |
| USGS tsunami flag | The cross |
| Quakes in the last hour | The scattered black marks |
| Last 3 h vs 24 h average | Texture size (busier Earth = coarser dots) |
| Strongest or newest quake | The headline: "M 6.6" over the place name; depth and age as subhead |
| New quake arriving | Peak grows in, ripple ring; M4+ makes the poster quiver |

Rules for live mode:
1. Keep the one-typeface rule. The place name auto-shrinks to fit, so the data pushes back on the type.
2. Cool palette colours are reserved for depth; do not use them decoratively.
3. Generate reshuffles the layout (horizon, x-axis, headline position, cutouts) but never the data.
4. Every data driver can be switched off in the Data panel to compare against the arbitrary version.
5. Offline fallback shows clearly labelled SAMPLE data, never presented as real quakes.
6. Replay compresses the last 24 h into 20–120 s so the poster can be judged without waiting for new quakes.

Critique prompts for the assignment: Is the data readable (can you tell the biggest quake, its depth and when it happened without hovering)? Does the layout make sense (is x = longitude legible)? Does the type fit the data (weight, size, long names) and does the data shape the type?
