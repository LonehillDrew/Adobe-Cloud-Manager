# Adobe Photoshop — Settings and Best Practices

## New Document Setup

### For Print
| Setting | Value |
|---|---|
| Resolution | 300 ppi |
| Colour Mode | RGB (master file) |
| Bit Depth | 16-bit for retouching, 8-bit for delivery |
| Colour Profile | sRGB IEC61966-2.1 |

### For Screen and Social
| Setting | Value |
|---|---|
| Resolution | 72 ppi |
| Colour Mode | RGB |
| Bit Depth | 8-bit |
| Colour Profile | sRGB IEC61966-2.1 |

---

## Colour Settings

`Edit > Colour Settings` (Cmd/Ctrl + Shift + K)
- RGB Working Space: sRGB IEC61966-2.1
- CMYK Working Space: ISO Coated v2 300% (ECI)
- Gray: Dot Gain 15%
- Colour Management Policies: Preserve Embedded Profiles
- Mismatches: Ask when opening, Ask when pasting

---

## Layer Management — Non-Destructive Workflow

- Use Adjustment Layers — never direct `Image > Adjustments` on a pixel layer
- Use Smart Objects for any raster content that may be resized
- Use Layer Groups to organise: Background, Typography, Artwork, Logo, Effects
- Use Layer Comps (`Window > Layer Comps`) for version variations in one file

### Layer Naming Convention
```
[BG] Background gradient
[ART] Hero illustration
[TYPE] Headline text
[LOGO] Client logo
[FX] Vignette or overlay effect
```

---

## Non-Destructive Flatten for Export

> ⚠️ Never flatten the master PSD. Use one of these three methods instead.

### Method 1 — Export As (Zero Risk)
`File > Export > Export As`
Composites all visible layers at export. Master file completely untouched.

### Method 2 — Save a Copy (Flat File Delivery)
`File > Save a Copy` — check Flatten Image — save with new descriptive name.
Master stays open and layered.

### Method 3 — Stamp Visible Layer
Cmd + Alt + Shift + E (Mac) or Ctrl + Alt + Shift + E (Windows)
Creates a merged layer on top. All original layers remain below it.

---

## Smart Objects — When to Use

Always convert to Smart Object for:
- Placed logos and AI/vector assets
- Images you may resize (no quality loss on transformation)
- Any filter you may need to adjust later (Smart Filters)

Double-click a Smart Object thumbnail to open and edit in its source app.

---

## Photoshop Actions for Repetitive Tasks

`Window > Actions` — New Action — Record — perform steps — Stop

Recommended actions to build:
- Export Print TIFF: Save a Copy, TIFF, 300 ppi, CMYK profile embedded
- Export Social JPEG: Save a Copy, JPEG Quality 85, sRGB, resize to 1080px
- Flatten Export Copy: Save a Copy, Flatten, save to Exports folder

---

## Resolution Guide

| Output | Resolution |
|---|---|
| Magazine full-page bleed | 300 ppi at full bleed size |
| Poster A1 | 150 ppi designed at A1 actual size |
| Large format banner | 72–100 ppi at final output size |
| Instagram 1080 x 1080 | 72 ppi — pixel count is what matters |

---

## Common Photoshop Issues

| Problem | Cause | Fix |
|---|---|---|
| File is 500MB or larger | 16-bit with many Smart Objects | Flatten to 8-bit for delivery — keep 16-bit master |
| Smart Filter is greyed out | Layer is not a Smart Object | Right-click layer — Convert to Smart Object |
| Colour shifts on export | sRGB not assigned | `Edit > Assign Profile > sRGB` before export |
| Exported JPEG looks different to screen | Profile mismatch or uncalibrated display | Assign sRGB — calibrate monitor |
