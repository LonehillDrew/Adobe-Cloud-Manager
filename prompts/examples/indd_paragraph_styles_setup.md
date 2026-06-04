# Example: Creating Paragraph Style Presets in InDesign

## Scenario
Setting up paragraph styles for a magazine so body text, captions, headlines, and bylines are applied consistently with one click — not formatted manually each time.

---

## Step 1 — Create a Style From Formatted Text

1. Format a text frame manually to the exact look you want
2. Place the cursor inside that paragraph (no need to select all text)
3. Open `Window > Styles > Paragraph Styles`
4. Click the New Style icon at the bottom of the panel
5. Double-click the new style to rename it
6. Click OK

The style now stores that exact formatting and can be applied to any text with one click.

---

## Step 2 — Recommended Magazine Paragraph Styles

| Style Name | Size | Leading | Tracking | Alignment | Use |
|---|---|---|---|---|---|
| H1_Cover_Title | 60–90pt | Auto | -20 | Left or Centre | Cover headlines |
| H2_Section_Title | 36–48pt | Auto | -10 | Left | Section openers |
| H3_Article_Title | 24–30pt | Auto | 0 | Left | Per-article headlines |
| Intro_Standfirst | 14–16pt | 20pt | 0 | Left | First paragraph of each article |
| Body_Copy | 9–10pt | 13–14pt | 0 | Justified | All flowing body text |
| Caption | 7–8pt | 10pt | +15 | Left | All image captions |
| Pull_Quote | 18–22pt | 26pt | -10 | Centre | Breakout pull quotes |
| Byline | 9pt | 12pt | 0 | Left | Author name attribution |
| Folio | 8pt | Auto | +20 | Outside edge | Page numbers on master pages |

---

## Step 3 — Caption Style Detailed Settings

The caption is one of the most-used recurring elements. In the Paragraph Style Options dialog:

- Font: brand body font, regular or light weight, 7.5pt
- Leading: 10pt
- Space Before: 2mm (separates the caption from the image above)
- Space After: 0mm
- Colour: 80% black or brand secondary colour
- Hyphenation: Off (short captions look bad with hyphens)
- Tracking: +15 (opens up small text for legibility)

Apply: click any caption text frame, then click Caption in the Paragraph Styles panel. Instant, consistent formatting.

---

## Step 4 — Load Styles Into a New Document

To reuse styles from a previous issue without recreating them:

1. Open the new document
2. `Window > Styles > Paragraph Styles` — panel menu top right — Load Paragraph Styles
3. Navigate to a previous issue .indd file and select it
4. Choose which styles to import
5. Click OK

All styles transfer instantly. No manual recreation needed each issue.

---

## Step 5 — Save as a Reusable Template

Save a blank .indd file with all styles pre-loaded:

`File > Save As` — Format: InDesign Template (.indt)
Name: MAGAZINE_TEMPLATE_2026.indt

Opening this file always creates a new untitled copy with all styles intact.
The template itself is never overwritten.
