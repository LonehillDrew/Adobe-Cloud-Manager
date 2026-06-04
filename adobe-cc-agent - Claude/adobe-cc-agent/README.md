# Adobe CC Design Agent — Project Brain

> Version-controlled source of truth for your Adobe Creative Cloud design operations.

## What This Is

This repository powers a Claude-based AI design assistant for a solo operator running a full-service media house and brand agency. It contains the system prompts, domain knowledge, export schemas, client templates, and product-type guides that the agent uses to answer questions, troubleshoot errors, and generate consistent workflows across Illustrator, Photoshop, InDesign, Bridge, and Acrobat.

---

## Folder Structure

```
adobe-cc-agent/
├── /prompts          → Agent identity, rules, and worked examples
├── /knowledge        → App guides, colour management, export how-tos, troubleshooting
├── /schemas          → Export preset definitions and platform specs
├── /config           → Agent model settings and memory/context rules
├── /clients          → Per-client brand guidelines (duplicate _template per client)
└── /products         → Per-deliverable-type setup guides and checklists
```

---

## Core Use Cases

| Scenario | File |
|---|---|
| Set up AI/PSD/INDD document correctly | `/knowledge/adobe/` |
| Export print-ready CMYK PDF | `/knowledge/export_guides/print_export.md` |
| Export interactive RGB PDF | `/knowledge/export_guides/digital_export.md` |
| Flatten PSD for export without destroying layers | `/prompts/examples/flatten_psd_export_nondestructive.md` |
| RGB logo in AI → INDD → print + digital | `/prompts/examples/rgb_logo_ai_to_indd_print_digital.md` |
| Magazine paragraph styles and caption presets | `/prompts/examples/indd_paragraph_styles_setup.md` |
| New client onboarding | `/clients/_template/brand_guidelines.md` |
| Social media dimensions | `/schemas/export_presets/social_media_specs.md` |
| Troubleshooting colour shifts and errors | `/knowledge/troubleshooting/colour_issues.md` |

---

## How to Use With Claude

1. Copy the contents of `/prompts/system_prompt.md`
2. Paste into your Claude Project as the system prompt
3. For client-specific work, paste `/clients/[client-name]/brand_guidelines.md` into the conversation

---

## Maintained By

Solo operator — media house and brand agency.
Last updated: 2026
