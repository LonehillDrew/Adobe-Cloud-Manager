# Digital and Interactive Export Guide

## Key Rule
Digital exports stay in RGB and sRGB. Never convert to CMYK for screen output.

---

## InDesign to Interactive PDF

`File > Export` — Adobe PDF (Interactive)

| Setting | Value |
|---|---|
| View | Single Page Continuous |
| Hyperlinks | Include |
| Bookmarks | Include |
| Colour Conversion | No Colour Conversion |
| Resolution | 150 ppi |
| JPEG Compression | Medium to High |

For digital magazines: add bookmarks per article at `Window > Interactive > Bookmarks` before exporting.

---

## InDesign to Screen PDF (via Print export, no conversion)

Use Adobe PDF (Print) but skip colour conversion:
Output tab — Colour Conversion: No Colour Conversion
This preserves RGB throughout for screen reading while giving full control over compression.

---

## Photoshop to Web and Digital

### JPEG — photos, editorial images, posters
`File > Export > Export As` — JPEG
- Quality: 80–90
- Colour Space: Convert to sRGB
- Resize to final use dimensions before export

### PNG — logos, graphics with text, transparency
`File > Export > Export As` — PNG
- Transparency: On
- Colour Space: Convert to sRGB

---

## Illustrator to SVG (Logos for Web)

`File > Export > Export As` — SVG

| Setting | Value |
|---|---|
| Styling | Presentation Attributes |
| Font | Convert to Outlines |
| Images | Embed |
| Minify | Yes |
| Responsive | Yes (removes fixed width and height) |

Always provide a PNG fallback alongside the SVG.

---

## Digital Magazine Checklist

- [ ] Colour mode is RGB throughout the document
- [ ] Interactive elements added (links, bookmarks)
- [ ] Table of contents linked to pages
- [ ] Images at 150 ppi (300 ppi is unnecessary for screen and adds file size)
- [ ] File size under 50MB for email, under 100MB for download
- [ ] Tested in Acrobat Reader before distributing

---

## File Naming — Digital Outputs

```
[client]_[product]_[version]_digital_RGB.[ext]

Examples:
brandx_magazine_issue3_v1_digital_RGB.pdf
brandx_logo_web.svg
agency_poster_instagram_v2.jpg
```
