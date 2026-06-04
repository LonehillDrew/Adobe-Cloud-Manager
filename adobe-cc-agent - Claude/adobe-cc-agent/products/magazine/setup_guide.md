# Product Guide — Magazine and Editorial

## New Issue Setup Checklist

- [ ] New INDD file: Facing Pages On, Intent Print, 3mm bleed, 6mm slug
- [ ] Page size and column grid confirmed with printer
- [ ] Master pages created: A-Master with folios and guides, B-Master blank
- [ ] Paragraph styles loaded from template or previous issue
- [ ] Object styles created
- [ ] Colour swatches loaded from client brand file
- [ ] Preflight profile loaded: Agency_Magazine_Preflight
- [ ] Linked assets folder created

---

## Folder Structure Per Issue

```
[Client]_Magazine_Issue[XX]/
├── _INDD/
│   └── [Client]_Magazine_Issue[XX]_v[X].indd
├── _Links/
│   ├── images/
│   ├── logos/
│   └── ads/
├── _Fonts/
├── _Export/
│   ├── print/
│   └── digital/
└── _Archive/
```

---

## Paragraph Styles — Quick Reference

| Style | Use |
|---|---|
| H1_Cover_Title | Cover headlines only |
| H2_Section_Title | Section and chapter openers |
| H3_Article_Title | Per-article headlines |
| Intro_Standfirst | First paragraph of each article |
| Body_Copy | All flowing body text |
| Caption | All image captions |
| Pull_Quote | Breakout pull quotes |
| Byline | Author attribution |
| Folio | Page numbers on master pages only |

Full style specs: knowledge/adobe/indesign_settings.md

---

## Export Checklist — Per Issue

### Before Export
- [ ] Links panel: zero missing, zero modified
- [ ] Preflight: zero errors
- [ ] All fonts available
- [ ] Client final approval received in writing
- [ ] Page count divisible by 4 for saddle stitch or by 8 for perfect bind

### Print PDF
- [ ] Preset: Agency_Print_CMYK_PDF-X4
- [ ] Colour conversion: ISO Coated v2 300%
- [ ] Bleed: Use document settings 3mm
- [ ] Crop marks: On
- [ ] Filename: [client]_magazine_issue[XX]_v[X]_print_CMYK.pdf
- [ ] File copied to _Export/print/ and archived

### Digital PDF
- [ ] Export: Adobe PDF Interactive
- [ ] No colour conversion
- [ ] Images at 150 ppi
- [ ] Hyperlinks and bookmarks included
- [ ] Filename: [client]_magazine_issue[XX]_v[X]_digital_RGB.pdf
- [ ] File copied to _Export/digital/

---

## Image Size Requirements

| Placement | Minimum Resolution |
|---|---|
| Full-page bleed | 300 ppi at page size plus 3mm bleed |
| Half-page | 300 ppi at placement size |
| Column image | 300 ppi at column width |
| Small thumbnail | 250 ppi minimum |

Check effective PPI: Window > Links — select the image — see Info in panel.

---

## Ad Spec Template for Advertisers

```
Full Page Ad — [Magazine Name]
Trim size: [W]mm x [H]mm
Bleed: 3mm all sides — total [W+6]mm x [H+6]mm
Safe zone: 5mm inside trim — keep all text and logos within this area
Format: PDF/X-4:2008
Colour: CMYK — ISO Coated v2 300% (ECI)
Resolution: 300 ppi minimum
Fonts: Embedded or outlined
Deadline: [X] working days before print date
Send files to: [email or FTP details]
```
