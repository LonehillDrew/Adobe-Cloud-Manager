# Adobe Acrobat — Settings and PDF Workflows

## Core Use Cases in a Design Agency

- Preflight and verify print PDFs before sending to printer
- Add passwords and permissions to client-delivery PDFs
- Combine multiple PDFs into one document
- Flatten interactive PDFs for archiving
- Check and fix colour profiles in exported PDFs
- Collect client sign-offs via Comments and markup tools
- Reduce file size for email distribution
- Add bookmarks, hyperlinks, and table of contents to digital PDFs

---

## Preflight — Verify a Print PDF

Before sending any print PDF to a printer, run Preflight.

`Tools > Print Production > Preflight`

Recommended profiles to run:
- PDF/X-4 compliant — verifies the PDF meets the print standard
- Colour spaces — checks for unexpected RGB in a CMYK document
- Resolution check — flags images below 250 ppi

To create a custom profile:
Preflight panel — Options — Create New Profile — set rules for your standard

If errors are found, Preflight can auto-fix some issues or report exact page and object locations.

---

## Output Preview — Check Colours Before Sending

`Tools > Print Production > Output Preview`

- Separation preview: see each ink channel (C, M, Y, K) individually
- Total area coverage: shows ink density and flags areas above 300%
- Simulate overprinting: previews how black overprinting will appear
- Colour space filter: quickly find stray RGB objects in a print PDF

---

## Reduce File Size

For digital distribution:

`File > Compress PDF` (Acrobat DC 2023 and later)

For more control:
`File > Save As Other > Optimized PDF`

In PDF Optimizer:
- Images: Downsample colour to 150 ppi for digital, JPEG High compression
- Fonts: Subset embedded fonts below 100%
- Discard Objects: Remove comments, JavaScript, form fields if not needed

---

## Combine Multiple PDFs

`File > Create > Combine Files into a Single PDF`
- Drag files into the correct order
- Outputs as a single PDF

Use for: assembling multi-section magazines, compiling proofing sets, packaging ad files.

---

## Password and Permissions

`File > Protect > Protect Using Password`

For client delivery:
- Open Password: requires password to view
- Permissions Password: restricts printing, editing, copying

Recommended for proofing PDFs: allow low-resolution printing, disallow editing and content copying.

---

## Markup and Client Approval Workflow

1. Send PDF to client
2. Client annotates using Comment tools (sticky note, highlight, draw)
3. You receive the commented PDF — `View > Comment` to review all notes
4. Reply to comments and mark as resolved when actioned

---

## Flatten Interactive PDF for Archiving

`File > Print` — print to Adobe PDF printer — save as flat PDF
Or: Preflight — Fixup — Flatten Annotations and Form Fields

---

## Common Acrobat Issues

| Problem | Cause | Fix |
|---|---|---|
| Preflight fails on RGB objects | RGB images in a CMYK print PDF | Fix in source file or use Preflight fixup |
| PDF too large for email | High-res images embedded | Use PDF Optimizer — downsample to 150 ppi |
| Fonts not embedded | Exported without embed setting | Re-export from InDesign with fonts embedded |
| Pages in wrong order | Assembled incorrectly | Drag page thumbnails in the Pages panel |
| Print colours differ from screen | No ICC profile embedded | Re-export with profile — verify in Output Preview |
