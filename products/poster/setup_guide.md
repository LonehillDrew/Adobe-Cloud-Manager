# Product Guide — Poster and Large Format Print

## Document Setup

### A1 Poster in Photoshop
- Size: 594 x 841mm at 150 ppi (design at actual final size)
- Colour Mode: RGB for master file
- Bit Depth: 16-bit for photography, 8-bit for flat graphic work
- Profile: sRGB IEC61966-2.1

### A1 Poster in Illustrator
- Size: 594 x 841mm
- Bleed: 5mm all sides
- Colour Mode: RGB master (convert copy to CMYK at export)
- Raster Effects: 150 ppi to match final output resolution

### A1 Poster in InDesign
- Size: 594 x 841mm
- Bleed: 5mm all sides
- Margins: 10mm all sides minimum
- Facing Pages: Off

---

## Resolution Guide for Large Format

| Final Print Size | Design At |
|---|---|
| A1 indoor close viewing | 150 ppi at A1 size |
| A0 indoor 1m viewing distance | 100 ppi at A0 size |
| 1000 x 1500mm retail signage | 100 ppi at final size |
| 2000 x 3000mm outdoor hoarding | 72 ppi at final size |
| Billboard 3m and larger | 25–50 ppi at final size |

Always design at the actual final output size. Never scale up at print.

---

## Export for Print

### From Photoshop
1. Duplicate: File > Save a Copy — name it FLAT_CMYK
2. On the copy: Image > Mode > CMYK Colour
3. Export as TIFF with LZW compression

### From InDesign
1. File > Export — Adobe PDF Print
2. Preset: Agency_Print_CMYK_PDF-X4
3. Bleed: 5mm

### From Illustrator
1. File > Save a Copy — Adobe PDF
2. Preset: PDF/X-4:2008
3. Output tab: Convert to CMYK profile

---

## Non-Destructive Flatten for Photoshop Posters

Master file: layered PSD at 150 ppi, RGB
Delivery file: flat TIFF at 150 ppi, CMYK

Use File > Save a Copy — check Flatten Image — save as TIFF

Full walkthrough: prompts/examples/flatten_psd_export_nondestructive.md

---

## Bleed and Safe Zone Diagram

```
Total width including bleed
|--- 5mm bleed ---|--- trim/print size ---|--- 5mm bleed ---|
                  |-- 10mm safe zone --|

Keep all important content (text, logos) inside the safe zone.
Background must extend to the bleed edge.
Trim marks show the printer where to cut.
```

---

## Folder Structure Per Poster Job

```
[Client]_Poster_[Name]/
├── _Working/
├── _Links/
├── _Export/
│   ├── print/
│   └── digital/
└── _Archive/
```
