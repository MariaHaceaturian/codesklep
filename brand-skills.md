# brand-skills.md: New York Monster at the Met · Brand Lock Prompt Builder + Compositor

Rulebook for the campaign tool (`NYM_brand_tool.html`). The tool does two jobs:
1. **Prompt Builder.** Writes image prompts for A.I. image generators, always inside the brand lock, in many angles and scenes.
2. **Compositor.** Takes the pictures you generate and places them into NYC ad formats and mockups, set in the brand's fonts and colours.

Campaign: **New York Monster at the Met**, a Gentle Monster × The Metropolitan Museum of Art concept. Launch spring 2027.
Line: **Look back.** Student concept; not an announced partnership; the Met has not approved it.

## 1. Brand lock (constants the tool never breaks)

### Palette
| Name | Hex | Role | Share |
|---|---|---|---|
| Marble Cream | #F3ECDD | ground, paper | 60% |
| Limestone | #DCCDB2 | secondary ground, panels | |
| Sandstone | #B9A486 | warm mid-tone, shadows | |
| Aged Silver | #A9ADB3 | the metal: frames, hairlines | 10% |
| Patina Black | #171614 | type, black ground, sunglass lenses | 25% |
| Faience | #5B8A8C | accent, Egypt (Kohl) | one accent |
| Oxblood | #8C2F2B | accent, Europe (Perseus) | per image, |
| Ochre Earth | #A9693A | accent, Oceania (Lashing) | ≤ 5% |

Rules: one accent per image, taken from the active department. No neon, glitter, gradients or colour filters.

### Type
- **Display:** Fraunces Light (300), capitals, tracked +120 to +160, "soft" and "wonk" off. Name, region titles.
- **Accent:** Bodoni Moda Italic, sentence case, never tracked. "at the Met", the line, pull quotes. One use per layout (the logotype's "at the Met" counts as part of the name).
- **Text:** Inter. Labels in caps, 11 to 12 px, tracked +200, weight 500. Body regular, 1.6 line height.
- All three are open source (SIL OFL).

### Logomark and name
- Mark: two almond lenses, a classical arch for the bridge, one keystone dot. The dot takes the accent colour, only on cream or limestone grounds (on accent grounds it turns cream).
- Name lockup: NEW YORK MONSTER (Fraunces caps) over *at the Met* (Bodoni italic). Never abbreviated.
- Endorsement stand-in: "Gentle Monster × The Metropolitan Museum of Art" (text only; real marks only as supplied by each brand).

### The three frames (hairline silver wire, always dainty)
| Dept | Frame | Spec |
|---|---|---|
| Egypt | Kohl, no. 01 | long almond lens, outer corner swept upward like the painted kohl line |
| Europe | Perseus, no. 02 | slim oval lens, laurel-leaf bridge, temples fall like marble drapery |
| Oceania | Lashing, no. 03 | round lens, fine wrapped bindings at hinge and bridge |
Sunglass versions: smoke, pale bronze, clear silver lenses.

### Imagery
Do: real gallery light (low, warm, directional); one person beside the stone; crowd as motion blur against a perfectly still sculpture; metal in sharp focus on a calm ground; the sculpture as a straight portrait, no smile.
Don't: colour filters, stock museum shots, tourists, phones, selfies; type over faces or glasses (type lives on the ground colour); more than one accent; any edit to the artwork except the glasses.

### Voice
Dry, curious, a little theatrical. Short lines. Gentle, never loud. No exclamation marks, no "shop now", no puns on "see", nothing that explains the joke.
Examples: "Look back." · "Same frame. Five thousand years apart." · "Everyone's looking. Now so is the art."

## 2. Prompt Builder

### Controls (each is a slot in the prompt)
| Slot | Options |
|---|---|
| Department | Egypt, Europe, Oceania (sets object, frame spec and accent) |
| Subject | sculpture wears the pair · visitor beside the stone · crowd in motion, stone still · frame still life · macro detail · plinth label flat lay · empty gallery at opening hour · subway echo |
| Shot | wide symmetrical · three-quarter portrait · pure profile · close-up on the eyes · low heroic · overhead · slow-shutter pan · looking back over the shoulder |
| Light | low warm gallery · soft window · single spotlight · blue hour with warm interior · flat studio on cream |
| Gaze | at camera · looks left · looks right (the diptych needs one of each) |
| Lenses | optical, smoke, pale bronze, clear silver |
| Ratio | 4:5, 9:16, 1:1, 16:9, 3:4, 2:3, 3:1 |
| Type space | none, bottom third, top third, right side (reserves empty ground for type) |
| Ground | cream, limestone, black, silver grey |

### Prompt grammar (plain version)
`[Subject sentence] [Shot] [Light] [Gaze] [Type space] [Ground] Editorial museum photograph, natural film grain. [Brand lock x5] Aspect ratio X. No text, logos or watermarks.`
Followed by a separate **Avoid** line: neon, glitter, gradients, colour filters, stock look, tourists, phones, selfies, crowds of models, extra accents, rendered text, watermark, logos, thick or ornamental frames, CGI look, oversaturation, HDR.

### Dialects
- **Gemini / ChatGPT:** full sentences, paragraphs, Avoid line.
- **Midjourney:** comma tags, then `--ar W:H --style raw --stylize 150 --no …`
- **Flux / SD:** tags, with a separate negative prompt.

### Variation engine
- Variations: 1, 2, 4 or 6 prompts.
- **Locked** (never change): palette, accent, frame spec, lighting realism, voice, no-text rule, department.
- **Free** (shuffle within the lists above): subject, shot, light, gaze. Each has a 🔒 to hold it fixed while the others vary. No repeats until the list is used up.
- Recipes preset the controls: banner diptych (visitor looks right, sculpture looks left), teaser empty plinth, Pairs post, crowd pan reel, product still, subway echo, billboard wide.

## 3. Compositor

### Formats and mockups (each format sets the ad's shape)
| Format | Ad size | Mockup scene (drawn, not photographed) |
|---|---|---|
| Billboard | 2400 × 800 (3:1) | rooftop bulletin at night, lamps, skyline, street light trails |
| Subway poster | 1200 × 1600 | tiled platform wall, "Metropolitan Museum · 86 St" band, three posters in frames with glass reflection |
| Wheat-paste | 1080 × 1620 | brick wall, torn older posters, wrinkled paste-up, drips |
| Phone reel | 1080 × 1920 | iPhone-style frame, rounded screen, Dynamic Island, status bar, story bars, CTA; safe areas 190 px top and bottom |
| Magazine | 1200 × 1600 | right-hand page of a spread, gutter shadow |
| Met banners | 640 × 1920 ×2 | facade with columns; image A on the left banner, B on the right; left carries the logomark, right the endorsement |

### Layouts (type always sits on ground colour)
- **Plinth:** picture on top (left on landscape), type panel below.
- **Type first:** type panel on top, picture below.
- **Window:** picture inset in a cream border.
- **Bleed + card:** full-bleed picture with a ground-coloured plinth-label card carrying all type.

### Type blocks (priority order; lower ones drop out if there's no room)
Headline · line · logomark · name lockup · date "SPRING 2027 · NEW YORK" · endorsement · plinth label (frame name + "Frame no. 0X · fine silver wire, 2027") · frame drawing · label description.
Headline styles: Bodoni italic (default), Fraunces caps, Inter light. Image grade: sepia 0.1, saturation 0.92. Grain: multiply, 14%.

### Image intake
- Drop, paste or choose files. Mark one as **A** and optionally **B**. Zoom and move sliders per image.
- Generate at the format's ratio when possible. Banners are 1:3, so generate 9:16 and crop with the sliders.
- The tool warns when a picture is enlarged more than 1.6×.

### Brand check (live)
Type on ground, not picture · one accent only · ground not another department's accent · no exclamation marks · no sales-line copy · picture resolution.

## 4. Export
PNG of the flat ad and PNG of the mockup. Both go into the final one-page launch site.

## 5. QA checklist before an asset is used
- [ ] Palette: only the five stones and one department accent
- [ ] Frames dainty, hairline silver, correct frame for the department
- [ ] Sculpture unaltered except glasses; no smile
- [ ] At most one person; no phones, tourists, selfies
- [ ] No type over faces or glasses; no text baked into the generated picture
- [ ] Copy dry and short; no "!"
- [ ] Logomark clear space ≥ 4 × dot height; minimum width 22 px

## 6. A.I. disclosure
The brand, the Met collaboration, the sculpture, palette direction and campaign idea are the creative director's. Claude wrote the tool and its rules from the style guide. The pictures used inside the tool as placeholders are the director's moodboard photographs; final campaign photography is to be generated with the prompts above and dropped in. Mockup scenes and the logomark are original vector artwork drawn by code.
