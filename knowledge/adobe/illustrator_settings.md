# Adobe Illustrator — Settings and Best Practices

## New Document Setup

### For Print Work
`File > New` — Profile: Print
- Units: Millimetres
- Colour Mode: CMYK (print-only work)
- Raster Effects: High (300 ppi)

### For Screen and Web
`File > New` — Profile: Web
- Units: Pixels
- Colour Mode: RGB
- Raster Effects: Screen (72 ppi)

### For Master Logo Files (Print and Digital Both)
Create masters in RGB with Raster Effects at 300 ppi.
- RGB preserves the widest colour gamut for editing
- Convert to CMYK at export — never in the master file
- One .ai master exports to separate CMYK and RGB PDFs as needed

---

## Colour Settings

`Edit > Colour Settings`
- RGB Working Space: sRGB IEC61966-2.1
- CMYK Working Space: ISO Coated v2 300% (ECI)
- Colour Management Policies: Preserve Embedded Profiles
- Profile Mismatches: Ask when opening, Ask when pasting

---

## Essential Preferences

`Illustrator > Preferences > General` (Mac) or `Edit > Preferences > General` (Windows)
- Keyboard Increment: 0.1mm for precise nudging
- Snap to Pixel: Off for print work, On for screen and UI work

`Preferences > Units`
- General: Millimetres (print) or Pixels (screen)
- Type: Points

---

## Artboard Organisation

Use multiple artboards for logo variants and name them clearly:
- Logo_Full_Colour
- Logo_Mono_Black
- Logo_Mono_White
- Logo_Reversed
- Logo_Icon_Only

`File > Export > Export for Screens` exports each artboard as a separate file simultaneously.

---

## Text Handling

For print delivery — outline fonts on a duplicate:
`Type > Create Outlines`

Keep the live-text master for future edits.
Name the outlined version: logo_OUTLINED.ai

For editable shared files — keep text live and package:
`File > Package`

---

## Saving and File Formats

| Purpose | Format | Notes |
|---|---|---|
| Editable master | .ai | Default settings |
| Place into InDesign | .ai or .pdf | PDF: check Preserve AI Editing Capabilities |
| Send to printer | .pdf | PDF/X-4, CMYK profile embedded |
| Web use | .svg | Responsive, scalable |
| Web fallback or social | .png | Export at 2x pixel dimensions for retina |
| Archive or sharing | Package via File > Package | Includes fonts and linked files |

---

## Common Illustrator Issues

| Problem | Cause | Fix |
|---|---|---|
| Raster effects look blurry | Document Raster Effects set to 72 ppi | `Effect > Document Raster Effects Settings` — set to 300 ppi |
| Colours shift when placed in InDesign | Missing or mixed colour profiles | `Edit > Assign Profile` to set correct sRGB or CMYK profile |
| File will not open on another machine | Missing linked images or fonts | `File > Package` before sharing |
| PDF is too large | High-res embedded rasters | Reduce raster image resolution before saving to PDF |
| Text reflows when opened by others | Font not available on their machine | Outline fonts on the delivery copy |
