# Example: Export Flattened PSD Without Permanently Flattening Layers

## Scenario
A poster PSD is 150MB with all layers intact. It needs to be exported as a flattened file (~40MB) for delivery or print, but all layers must be preserved in the working file for future revisions.

---

## Rule
> ⚠️ Never use Layer > Flatten Image on your master file. This is permanent once saved and cannot be undone.

---

## Method 1 — Export As (Recommended — Zero Risk)

Photoshop composites all visible layers into the export without touching the working document.

1. `File > Export > Export As`
2. Choose format: TIFF for print, JPEG for digital delivery
3. For print TIFF: set Colour Space to CMYK profile, 300 ppi
4. Click Export

The exported file is flat. The master .psd is completely untouched.

---

## Method 2 — Save a Copy (When a Flat PSD or TIFF File is Required)

1. `File > Save a Copy` (Photoshop 2021 and later)
2. Name it clearly: poster_FLAT_v1.tiff or poster_print_delivery.psd
3. In the Save dialog, check Flatten Image
4. Save

The original file stays open and layered. Only the named copy is flat.

---

## Method 3 — Stamp Visible (For In-Document Composite Layer)

Press Cmd + Alt + Shift + E on Mac or Ctrl + Alt + Shift + E on Windows.

Creates a new merged layer on top of the stack. All original layers remain intact below it.
Use this merged layer for any in-document work, then delete it when done.

---

## File Size Reference

| State | Approximate Size |
|---|---|
| Layered PSD | 150MB |
| Flattened TIFF CMYK 300dpi | 40–60MB |
| Flattened JPEG Quality 10 | 5–15MB |
| Flattened Print PDF | 20–40MB |

---

## For Print Delivery — on the flat copy only

- Colour mode: CMYK — `Image > Mode > CMYK Colour` on the copy, never the master
- Resolution: 300 ppi
- Embed ICC Profile: ISO Coated v2 300%
- Extend bleed if required by the printer spec
