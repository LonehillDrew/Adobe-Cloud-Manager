# Memory and Context Rules

## Always Load — Every Session
- prompts/system_prompt.md
- prompts/task_rules.md
- knowledge/colour_management.md
- knowledge/domain_facts.md

---

## Load Per Task — Trigger Words and Files

| Trigger | Load This File |
|---|---|
| Illustrator or AI file | knowledge/adobe/illustrator_settings.md |
| Photoshop or PSD | knowledge/adobe/photoshop_settings.md |
| InDesign or INDD | knowledge/adobe/indesign_settings.md |
| Bridge | knowledge/adobe/bridge_settings.md |
| Acrobat or PDF | knowledge/adobe/acrobat_settings.md |
| Print, CMYK, press-ready | knowledge/export_guides/print_export.md |
| Digital, interactive, screen | knowledge/export_guides/digital_export.md |
| Social media, Instagram, Facebook | knowledge/export_guides/social_export.md |
| Troubleshooting, error, shift | knowledge/troubleshooting/colour_issues.md |
| Magazine, editorial | products/magazine/setup_guide.md |
| Poster, large format | products/poster/setup_guide.md |
| Brand identity, logo | products/brand_identity/setup_guide.md |
| Client mentioned by name | clients/[client-name]/brand_guidelines.md |

---

## Context Management

The agent has no persistent memory between sessions.

At the start of any session involving a specific client, paste the contents of that client's brand_guidelines.md file into the conversation.

At the start of any session involving a specific product type, paste the relevant setup_guide.md from the products folder.

---

## What Not to Load Every Session

Social media specs, individual product guides, error log — load only when directly relevant to the current task to keep context focused.
