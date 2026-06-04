# Print Export Guide

## Pre-Export Checklist

- [ ] Bleed set correctly (3mm magazine, 5mm large format)
- [ ] All images are 300 ppi at final output size
- [ ] All fonts are embedded or outlined
- [ ] No stray RGB images (or colour conversion handled at export)
- [ ] Spot colours converted to CMYK unless intentional
- [ ] Preflight shows zero errors
- [ ] Black text is set to 100K not rich black
- [ ] PDF standard confirmed with printer (PDF/X-4 recommended)

---

## InDesign to Print PDF

`File > Export` — Adobe PDF (Print)

### General Tab
| Setting | Value |
|---|---|
| Standard | PDF/X-4:2008 |
| Compatibility | Acrobat 7 (PDF 1.6) |

### Compression Tab
| Setting | Value |
|---|---|
| Colour Image Downsampling | Bicubic to 300 ppi for images above 450 ppi |
| Compression | JPEG |
| Image Quality | Maximum |
| Grayscale | Same as colour |
| Monochrome | 1200 ppi |
| Compress Text and Line Art | Yes |

### Marks and Bleeds Tab
| Setting | Value |
|---|---|
| Crop Marks | On |
| Registration Marks | On |
| Bleed | Use Document Bleed Settings |

### Output Tab
| Setting | Value |
|---|---|
| Colour Conversion | Convert to Destination (Preserve Numbers) |
| Destination | ISO Coated v2 300% (ECI) |
| Include Destination Profile | Yes |

### Advanced Tab
| Setting | Value |
|---|---|
| Transparency Flattener | High Resolution |
| OPI | Off |

---

## Photoshop to Print TIFF

1. `File > Save a Copy` — Format: TIFF
2. Compression: LZW (lossless)
3. Check Discard Layers (delivery copy only)
4. On the copy: `Image > Mode > CMYK Colour`
5. Embed profile: ISO Coated v2 300%

---

## Illustrator to Print PDF

1. `File > Save a Copy` — Format: Adobe PDF
2. Preset: PDF/X-4:2008
3. Output tab: Convert to Destination — ISO Coated v2 300%
4. Marks and Bleeds: Crop marks on, bleed 3mm

---

## Large Format Posters and Banners

| Setting | Value |
|---|---|
| Resolution | 100–150 ppi at final output size |
| Colour mode | CMYK |
| Profile | Ask vendor — large format varies |
| Bleed | 5mm minimum, 20mm for banner hems |
| Format | PDF/X-4 or TIFF (ask vendor preference) |

> Always design at the actual final output size. A 300 ppi A4 file printed at A0 is only approximately 35 ppi.

---

## File Naming — Print Outputs

```
[client]_[product]_[version]_print_CMYK.[ext]

Examples:
brandx_magazine_issue3_v2_print_CMYK.pdf
agency_poster_A1_v1_print.tiff
```
