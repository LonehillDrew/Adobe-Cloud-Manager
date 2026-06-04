# Troubleshooting — Colour and Export Issues

## Blues Turn Purple in Print
Cause: Vibrant RGB blues fall outside the CMYK colour gamut.
Fix:
1. Enable soft-proof: `View > Proof Colours` in InDesign or Photoshop
2. On a duplicate file, convert to CMYK: `Image > Mode > CMYK Colour`
3. Adjust blues: `Image > Adjustments > Hue/Saturation` — select Blues — shift Hue slightly toward cyan
4. Alternative: use Perceptual rendering intent at export for a less aggressive shift

---

## Colours Washed Out in Print
Cause: File was exported in RGB and sent to a CMYK printer without conversion, or wrong ICC profile used.
Fix:
- Re-export from InDesign with Output tab set to: Convert to Destination — ISO Coated v2 300%
- Open the delivered PDF in Acrobat — Output Preview — check colour channels before sending

---

## Black Text Looks Grey in Print
Cause: RGB black (R0 G0 B0) converts to a mixed ink value approximately C75 M68 Y67 K90 which can look soft.
Fix:
- Body text: use 100K only — C0 M0 Y0 K100 — single ink, crisp at small sizes
- In InDesign: use the swatch named [Black] — it outputs as 100K
- Large dark areas: rich black C60 M40 Y40 K100 is fine

---

## Missing Profile Warning on Open
Cause: File was saved without an embedded ICC profile.
Fix:
- In Photoshop: `Edit > Assign Profile` — select the correct profile
- Do not choose Do Not Colour Manage on any file going to print

---

## PDF Too Large for Email
Cause: Images not downsampled, or lossless compression used on photos.
Fix:
- In InDesign Export, Compression tab: Bicubic Downsampling to 150 ppi for digital, JPEG Maximum quality
- In Acrobat: `File > Compress PDF` or PDF Optimizer — downsample colour to 150 ppi

---

## Font Missing on Open in InDesign
Cause: Font not installed on the current machine.
Fix:
1. `Type > Find/Replace Font` — see all missing fonts
2. Replace with an available font, or install the missing one
3. Prevention: always use `File > Package` before archiving or sharing

---

## InDesign Links — Modified or Missing
Cause: Linked file was moved, renamed, or updated outside InDesign.
Fix: `Window > Links` panel
- Yellow triangle = Modified — click Update Link
- Red circle = Missing — click Relink — navigate to the file
Prevention: never move linked assets after placing. Keep all assets in a fixed Links folder.

---

## Image Looks Pixelated in InDesign
Cause: Display Performance set to Fast. This is a screen display setting only and does not affect export quality.
Fix: `View > Display Performance > High Quality Display`

---

## InDesign Preflight Errors

| Error | Fix |
|---|---|
| Overset text | Resize the text frame or reduce the copy |
| Missing font | Install the font or use Find/Replace Font |
| Missing link | Relink via the Links panel |
| Image below 250 ppi | Replace with higher-resolution file or reduce frame size |
| RGB image in print document | Convert source file or set colour conversion at export |
| Unexpected spot colour | Check Swatches panel for stray Pantone swatches |

---

## Photoshop Export Colour Mismatch
Cause: File has no assigned profile or the wrong profile is embedded.
Fix:
1. `Edit > Assign Profile` — confirm sRGB for digital, FOGRA39 for CMYK print
2. `File > Export > Export As` — ensure Convert to sRGB is checked for digital output

---

## Illustrator Raster Effects Look Blurry
Cause: Document Raster Effects resolution set to 72 ppi.
Fix: `Effect > Document Raster Effects Settings` — change to 300 ppi
Note: this recalculates all effects and may slightly change their appearance.
