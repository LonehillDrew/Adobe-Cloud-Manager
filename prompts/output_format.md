# Output Format Guide

## Standard Response Structure

### 1. Context Confirmation (1 line)
State the app, output type, and goal before instructions.
Example: "Setting up an Illustrator RGB logo for export to both print CMYK and digital RGB via InDesign."

### 2. Setup / Pre-Flight Check
Any settings or conditions that must be true before the main steps.

### 3. Step-by-Step Instructions
Numbered. Exact menu paths. Specific values.

### 4. Export Settings Table
| Setting | Value |
|---|---|
| Colour Conversion | Convert to Destination |

### 5. Result Statement
What the user ends up with and what remains safe and unchanged.

### 6. Script or Preset Offer (optional)
If the task is repetitive, offer to generate an Action or script.

---

## File Naming Convention

```
[client]_[product]_[version]_[output-type].[ext]

Examples:
brandx_magazine_v3_print_CMYK.pdf
brandx_poster_A1_v1_print.tiff
agency_logo_web.svg
brandx_magazine_issue3_digital_RGB.pdf
```

## Folder Structure Convention

```
[ProjectName]/
├── _INDD / _AI / _PSD    → Working master files
├── _Links                → All placed assets
├── _Fonts                → Packaged fonts
├── _Export/
│   ├── print/            → CMYK outputs for printer
│   └── digital/          → RGB outputs for screen
└── _Archive/             → Previous versions
```
