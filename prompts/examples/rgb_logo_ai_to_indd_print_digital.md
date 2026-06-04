# Example: RGB Logo (AI) to InDesign — Print PDF and Digital PDF

## Scenario
A logo was created in Illustrator in RGB. It needs to be placed in an InDesign magazine layout and exported as both a print-ready CMYK PDF and an interactive digital RGB PDF.

---

## Rule
Do NOT convert the AI file to CMYK. Keep the master .ai file in RGB. Colour conversion happens at export time through InDesign.

---

## Step 1 — Illustrator File Setup

- `File > Document Colour Mode` — keep as RGB Colour
- Artboard sized to exact logo dimensions needed
- If delivering directly to a printer, outline fonts on a duplicate: `Type > Create Outlines`
- Save as .ai (native) — places correctly into InDesign

---

## Step 2 — InDesign Document Setup

`File > Document Setup`:
- Bleed: 3mm all sides

`Edit > Colour Settings`:
- RGB Working Space: sRGB IEC61966-2.1
- CMYK Working Space: ISO Coated v2 300% (ECI)
- Colour Management Policies: Preserve Embedded Profiles

---

## Step 3 — Place the Logo

`File > Place` — select the .ai file
- Check Show Import Options in the Place dialog
- Select the correct artboard if the file has multiple

The logo appears in RGB — this is correct and expected at this stage.

---

## Step 4 — Export Print PDF (CMYK)

`File > Export` — Adobe PDF (Print)

| Setting | Value |
|---|---|
| Standard | PDF/X-4:2008 |
| Compatibility | Acrobat 7 (PDF 1.6) |
| Colour Conversion | Convert to Destination (Preserve Numbers) |
| Destination | ISO Coated v2 300% (ECI) |
| Include ICC Profile | Yes |
| Crop Marks | On |
| Bleed | Use Document Bleed Settings |
| Transparency Flattener | High Resolution |

---

## Step 5 — Export Digital PDF (RGB)

`File > Export` — Adobe PDF (Interactive)

| Setting | Value |
|---|---|
| Colour Conversion | No Colour Conversion |
| Image Resolution | 150 ppi |
| JPEG Compression | Medium to High |
| Hyperlinks | Include |
| Bookmarks | Include |

---

## Result
- magazine_print_CMYK.pdf — press-ready, CMYK, with bleed and crop marks
- magazine_digital_RGB.pdf — interactive, RGB, screen-optimised
- Master .indd and .ai files untouched and fully editable
