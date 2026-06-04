# Colour Management — Core Knowledge

## The Fundamental Rule

RGB is for light (screens). CMYK is for ink (print).

Most design work starts in RGB because monitors display RGB. Print output requires CMYK. The conversion between them must be managed carefully or colours will shift unexpectedly.

---

## Colour Modes by Output

| Output Destination | Mode | Profile | Notes |
|---|---|---|---|
| Offset magazine and book print | CMYK | FOGRA39 or ISO Coated v2 300% | Standard in South Africa and Europe |
| Digital printing short-run (Indigo) | CMYK | GRACoL 2006 or printer-supplied | Ask your print vendor |
| Large format (banner, poster, vinyl) | CMYK | Vendor-supplied | Large format uses different ink sets |
| Screen, web, social | RGB | sRGB IEC61966-2.1 | Widest device compatibility |
| Interactive PDF and digital magazine | RGB | sRGB | Do not convert to CMYK |
| Video and motion | RGB | Rec. 709 | For After Effects and Premiere work |
| Photography archiving and master files | RGB | Adobe RGB (1998) | Wider gamut for retouching headroom |

---

## Colour Profiles Explained

### sRGB IEC61966-2.1
Standard for web and most screens. Narrowest RGB gamut.
Use for anything going to screen, social media, or digital PDF.

### Adobe RGB (1998)
Wider gamut — captures more greens and cyans.
Use for photography masters and retouching.
Always convert to sRGB before web output.

### FOGRA39 — ISO Coated v2
European and South African standard for coated offset printing (magazines, brochures, packaging).
Total ink limit 330%.

### ISO Coated v2 300% (ECI)
Variant of FOGRA39 with 300% ink limit.
Safe default choice when unsure which to use.

---

## Colour Conversion — When and How

### At Export (Always Preferred — Master File Untouched)

In InDesign PDF Export, Output tab:
- Colour Conversion: Convert to Destination (Preserve Numbers)
- Destination: ISO Coated v2 300% (ECI)

In Photoshop Export As:
- Colour Space: Convert to sRGB (for digital output)

### On File (Duplicates Only — Never the Master)

Photoshop: `Image > Mode > CMYK Colour`
Illustrator: `Edit > Convert to Profile`

> ⚠️ Converting RGB to CMYK will shift bright blues, vibrant greens, and neon colours significantly. Always soft-proof before committing.

---

## Soft Proofing — Preview Print Output On Screen

In Photoshop:
`View > Proof Setup > Custom`
- Device to Simulate: ISO Coated v2 (ECI)
- Rendering Intent: Relative Colorimetric
- Black Point Compensation: On
Toggle preview: `View > Proof Colours` (Cmd/Ctrl + Y)

In InDesign:
`View > Proof Setup` — select CMYK profile
`View > Proof Colours` to toggle

Gamut Warning at `View > Gamut Warning` shows out-of-gamut colours as a grey overlay.

---

## Common Colour Problems

| Problem | Cause | Fix |
|---|---|---|
| Blues go purple in print | RGB blue outside CMYK gamut | Adjust in CMYK soft proof; shift toward cyan |
| Blacks look grey in print | Using RGB black not 100K | Use C0 M0 Y0 K100 for all text |
| Colours washed out in digital PDF | Converted to CMYK before export | Export RGB version with no colour conversion |
| Logo looks different across apps | Mixed or missing embedded profiles | Standardise to sRGB in all RGB files |
| Skin tones shift in print | Wrong rendering intent | Use Relative Colorimetric with Black Point Compensation |

---

## Black Values Reference

| Use | Value | Reason |
|---|---|---|
| Body text (small sizes) | C0 M0 Y0 K100 | Single ink — crisp at small sizes |
| Large backgrounds and panels | C60 M40 Y40 K100 | Rich black — deeper and denser |
| Screen and digital | #000000 | Pure RGB black |

Never use rich black on body text. Ink spread causes blurring at small sizes.
