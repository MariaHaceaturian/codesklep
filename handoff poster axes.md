# handoff.md — Poster-Generator Tool (Weingart reference)

## Status
- Reference poster chosen: Wolfgang Weingart, *Das Schweizer Plakat* (1984)
- skills.md drafted from stream-of-consciousness notes on the poster plus a
  direct visual analysis of the uploaded scan (grid, hierarchy, color, rules)
- Typographic scale and color palette in skills.md are eye estimates from the
  scan, not measured/color-picked from the physical print — still need
  confirmation
- A vision-model hierarchy-measurement pass (comparing H1/H2/body ratios and
  cross-referencing Google Fonts) has not been run yet; skills.md currently
  reflects direct visual inspection instead
- Paper UI sketch: done, and the tool has been built and iterated on directly
  from it (poster_generator.html) — further changes now go straight into the
  tool rather than back through the sketch

## Decided
- Grid: portrait canvas ≈ 1:1.42, bottom ~22% reserved for text, headline
  split into a left column ("Das"/"Schweizer") and a right column ("Plakat")
  overlapping the image
- Type scale: three tiers (display / subhead / caption), ratio ≈ 1 : 0.41 : 0.11
  on a 1200×1700px canvas reference, default sizes 220px / 90px / 24px, with
  Compact/Default/Bold-Large size variants
- Font rule changed: only one typeface is chosen for the whole poster at a
  time (no separate display/body roles). Three options in the tool: Archivo,
  Inter, and a new addition — Bodoni Moda Italic (variable, opsz+wght,
  uploaded as a .ttf and embedded directly in the tool)
- Texture filter now offers three selectable types, one shared size slider:
  Dot Screen / Polka Dot Grid (default), Screen Tone / Manga Tone, Line
  Screen / Engraving Lines — all three also apply to an uploaded photo
- Border filter expanded: color is now choosable from the currently active
  palette colors (default cream), and style has four options — Uniform,
  Asymmetric (randomized per-side thickness), Circles, and Triangles (trims
  along the top/bottom bands) — alongside the existing size slider
- Text filter expanded: opacity (20–100%) and size (50–150%) sliders added
  for the custom headline text; the caption keeps its own fixed opacity
- Composition rules locked in skills.md: flush-left type, tight leading,
  headline overlapping the image with no background plate, one controlled
  "tear," a bleeding border edge, halftone texture against flat type/border
- Added three detail rules after a closer look at the poster: small knockout
  shapes (plus signs, rectangles, circles) cut into the display letterforms,
  date/venue text set at reduced opacity (~55–65%), and small black marks
  (random lines, triangles) scattered through the halftone illustration

## Live-data project (current)
- Class brief: live data stream + LLM-assisted build + site/poster whose type, color, layout and shapes react to the data, keeping a generate button
- Bluesky firehose rejected; USGS earthquakes chosen
- Built quake_poster_generator.html (new file, original poster_generator.html untouched): USGS polling every 60 s, Live + 24 h Replay, hover tooltips, per-driver switches, PDF download, labelled offline sample fallback. Mapping table is in skills.md section 6
- Tested in headless Chromium with a mocked USGS response (schema from the real feed) and with the network blocked. Fetching the real feed from a browser was not verified from the sandbox (proxy blocked it); if it fails on your host, the status pill shows OFFLINE / SAMPLE
- Added quake_poster_axes.html (quake_poster_generator.html kept as the previous version): Fraunces added; headline is live HTML text whose font axes follow magnitude, depth and activity for all four fonts, with an on/off switch and an optional Cursor X stream. Mapping table in skills.md section 7. Tested in headless Chromium (axes change per font, off state, PDF export keeps axes)
- Axes made more dramatic (same file, quake_poster_axes.html): intensity slider (default 80), signals rescaled to their real range, wider axis ranges, jolt on arrival. In a mocked replay at 100% Fraunces moved wght 247–780, opsz 9–133, SOFT 4–100, WONK 0.38–1; at 20% about a third of that. Details in skills.md 7a
- Website styling added to quake_poster_axes.html: UI text follows the chosen typeface, sun/moon light-dark toggle bottom-left, barely-visible halftone overlay. See skills.md section 8
- Not yet embedded in index.html (offer pending)

## Open questions
- Do the H1:H2:caption ratios need to be verified against the poster's actual
  printed dimensions (120 × 84.1 cm), or are the eye-estimated ratios enough
  to build from?
- Do the palette hex values need color-picking from a higher-quality scan, or
  are the named/approximate colors in skills.md sufficient for a first version
  of the tool?

## Next steps
1. Set up the local project folder (fonts/ + inspiration/ + skills.md +
   handoff.md at the root) — fonts now include Archivo, Inter, and Bodoni
   Moda Italic
2. Keep iterating directly on poster_generator.html as new feature requests
   come in; update skills.md and handoff.md alongside each change
3. Judge the quake poster for readability, layout sense and type-fits-data; tweak mappings
4. Optionally embed quake_poster_generator.html in index.html (needs the live fetch to work inside the iframe)
5. Decide whether to pursue true vector (SVG) export, noted as a bigger
   rebuild in an earlier session — still open if wanted

## How to resume this project
Paste skills.md and this handoff.md at the start of a new session so the
model has the rules and the current state without re-deriving them.
