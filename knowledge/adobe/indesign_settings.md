# Adobe InDesign — Settings, Styles and Best Practices

## New Document Setup

### Magazine and Editorial
| Setting | Value |
|---|---|
| Intent | Print |
| Facing Pages | On |
| Page Size | 210 x 280mm (confirm with printer) |
| Columns | 3, Gutter 4.5mm |
| Margins | Outside 15mm, Inside 20mm, Top 15mm, Bottom 20mm |
| Bleed | 3mm all sides |
| Slug | 6mm (space for printer marks) |

### Poster
| Setting | Value |
|---|---|
| Intent | Print |
| Facing Pages | Off |
| Page Size | 594 x 841mm A1 or custom |
| Margins | 10mm all sides |
| Bleed | 5mm all sides |

---

## Document Colour Settings

`Edit > Colour Settings`
- RGB Working Space: sRGB IEC61966-2.1
- CMYK Working Space: ISO Coated v2 300% (ECI)
- Colour Management Policies: Preserve Embedded Profiles

---

## Paragraph Styles — Magazine Standard

| Style Name | Size | Leading | Tracking | Alignment | Use |
|---|---|---|---|---|---|
| H1_Cover_Title | 60–90pt | Auto | -20 | Left or Centre | Cover headlines |
| H2_Section_Title | 36–48pt | Auto | -10 | Left | Section openers |
| H3_Article_Title | 24–30pt | Auto | 0 | Left | Per-article headlines |
| Intro_Standfirst | 14–16pt | 20pt | 0 | Left | First paragraph of each article |
| Body_Copy | 9–10pt | 13–14pt | 0 | Justified | All flowing body text |
| Caption | 7–8pt | 10pt | +15 | Left | All image captions |
| Pull_Quote | 18–22pt | 26pt | -10 | Centre | Breakout pull quotes |
| Byline | 9pt | 12pt | 0 | Left | Author name |
| Folio | 8pt | Auto | +20 | Outside edge | Page numbers on master |
| Sidebar_Body | 8–9pt | 12pt | 0 | Left | Callout and sidebar text |

### Caption Style Detailed Settings
- Font: brand body font, regular or light, 7.5pt
- Leading: 10pt
- Space Before: 2mm
- Colour: 80% black or brand secondary
- Hyphenation: Off
- Tracking: +15

---

## Object Styles

`Window > Styles > Object Styles`

| Style | Settings |
|---|---|
| Image_Frame_Standard | No stroke, default clipping |
| Caption_Box | No fill, no stroke |
| Pull_Quote_Box | Brand colour fill, 4mm padding |
| Ad_Frame | Hairline stroke, no fill |

---

## Master Pages

`Window > Pages` — Double-click A-Master

Add to master:
- Page number marker: `Type > Insert Special Character > Markers > Current Page Number`
- Header and footer text frames with Folio style applied
- Column guides matching the document grid

Apply masters by dragging the master name onto page thumbnails in the Pages panel.

---

## Preflight Profile

`Window > Output > Preflight` — Define Profile — name it Agency_Magazine_Preflight

Settings:
- Images: Minimum resolution 250 ppi, warn on RGB images in print documents
- Text: Error on overset text, error on missing fonts
- Links: Error on missing links, warn on modified links
- Colour: Warn on unexpected spot colours

Run before every export. Target is zero errors.

---

## Save as Template

`File > Save As` — Format: InDesign Template (.indt)
Name: MAGAZINE_TEMPLATE_2026.indt

Opening the template always creates a new untitled copy.
The template itself is never overwritten.

---

## Common InDesign Issues

| Problem | Cause | Fix |
|---|---|---|
| Image looks pixelated on screen | Display Performance set to Fast | `View > Display Performance > High Quality Display` |
| Text overset — red plus icon | Text does not fit the frame | Resize frame or reduce copy |
| Missing links on open | Files moved or renamed | `Window > Links` — Relink each file |
| Colours differ from Photoshop | Profile mismatch | Confirm both apps use same CMYK profile |
| PDF export too large | Images not downsampled | Set 300 ppi downsampling in Export Compression tab |
| Fonts missing | Not installed on machine | `Type > Find/Replace Font` or install the font |
