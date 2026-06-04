# Product Guide — Brand Identity

## Full Deliverables Folder Structure

```
[Client]_Brand_Identity_[Year]/
├── logos/
│   ├── AI/
│   │   ├── [client]_logo_RGB.ai
│   │   ├── [client]_logo_CMYK.ai
│   │   └── [client]_logo_variants.ai
│   ├── PDF/
│   │   ├── [client]_logo_print_CMYK.pdf
│   │   └── [client]_logo_digital_RGB.pdf
│   ├── PNG/
│   │   ├── [client]_logo_colour_RGB.png
│   │   ├── [client]_logo_mono_black.png
│   │   ├── [client]_logo_mono_white.png
│   │   └── [client]_logo_favicon_512px.png
│   └── SVG/
│       └── [client]_logo_web.svg
├── brand_guidelines/
│   └── [client]_brand_guidelines.pdf
├── colour_swatches/
│   ├── [client]_swatches.ase
│   └── [client]_swatches.pdf
└── fonts/
```

---

## Logo Artboard Structure in Illustrator

One .ai file with multiple named artboards:

| Artboard Name | Contents |
|---|---|
| Logo_Primary | Full colour, main version |
| Logo_Mono_Black | Single colour black |
| Logo_Mono_White | Single colour white |
| Logo_Reversed | White on brand colour background |
| Logo_Icon_Only | Symbol without wordmark |
| Logo_Stacked | Vertical layout |
| Logo_Horizontal | Horizontal layout |

---

## Export All Logo Formats at Once

`File > Export > Export for Screens` in Illustrator
- Selects all artboards or specific ones
- Export as PDF, PNG, and SVG simultaneously
- Scale: 1x for standard, 2x for retina PNG

---

## Colour Swatch Export as ASE

Share brand colours across all Adobe apps using Adobe Swatch Exchange files.

1. Set up all brand colours in the Illustrator Swatches panel
2. Select all brand swatches
3. Swatches panel menu — Save Swatch Library as ASE
4. Name: [client]_brand_swatches.ase

Load in Photoshop or InDesign:
Swatches panel menu — Load Swatches — select the .ase file

---

## Brand Guidelines Document

Build in InDesign. Minimum sections:

1. Logo — versions, clear space, minimum sizes, do nots
2. Colour palette — HEX, RGB, CMYK, Pantone values
3. Typography — typefaces, weights, hierarchy examples
4. Photography and image style
5. Application examples — business card, letterhead, social post

Export as:
- Interactive PDF RGB for client digital reference
- Print PDF CMYK if printing a physical brand manual

---

## Converting RGB Logo to CMYK

On a duplicate .ai file — never the master:

1. `Edit > Convert to Profile`
2. CMYK: ISO Coated v2 300%
3. Visually check all colours — adjust any that shift unacceptably
4. Save as [client]_logo_CMYK.ai
5. Export CMYK PDF for all print use

The RGB .ai file remains the source of truth. Never overwrite it.
