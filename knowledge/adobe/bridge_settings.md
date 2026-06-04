# Adobe Bridge — Settings and Workflow

## What Bridge Is Used For
- Browsing and previewing all asset types (AI, PSD, INDD, PDF, images, video)
- Batch renaming files consistently
- Applying metadata and copyright information
- Running batch Photoshop Actions across folders
- Colour management — assigning and converting profiles on files
- Organising assets with labels, ratings, and collections
- Camera Raw access for RAW photo files (.CR2, .ARW, .DNG)

---

## Preferences

`Edit > Preferences > General`
- Thumbnails: Prefer Embedded (faster) or Always High Quality (colour accurate)
- Background: Set to neutral grey for accurate colour previewing

`Edit > Preferences > Thumbnails`
- Maximum Size: 256px
- Generate 100% Previews: On (slower first open, faster zoom previews after)

---

## Workspace Setup

Recommended panels to keep visible:
- Folders (navigation)
- Filter (narrow by type, date, rating)
- Metadata (view and edit file metadata)
- Preview (large preview panel)
- Content (thumbnail grid)

Save as workspace: `Window > Workspace > New Workspace`
Name it: Design Production

---

## Labels and Ratings System

Use consistently across all projects.

| Label | Colour | Meaning |
|---|---|---|
| Select | Green | Approved and final |
| Second | Yellow | In review or with client |
| Approved | Cyan | Ready to export |
| Review | Red | Needs changes |
| To Do | Purple | Not yet started |

Apply labels: Select file — `Label` menu or keyboard shortcuts (6 = red, 7 = yellow, 8 = green)
Apply star ratings: `Label > [star count]` or Cmd/Ctrl + 1 through 5

---

## Batch Rename

`Tools > Batch Rename`

Useful naming patterns:
- Client_Product_Sequence — BrandX_Magazine_001
- Date_Description_Version — 2026_CoverShoot_v2

Options:
- Rename in same folder or copy to a new folder
- Preserve current filename in metadata
- Preview results before applying

---

## Batch Photoshop Actions

1. Create the Action in Photoshop first (`Window > Actions`)
2. In Bridge: select the target files or folder
3. `Tools > Photoshop > Batch`
4. Choose the Action — set destination folder — Run

Common uses:
- Resize a folder of images to 1080px for social media
- Apply colour profiles to a batch of images
- Export flat TIFFs from a folder of layered PSDs

---

## Metadata and Copyright

Set default metadata on all delivered files.

`Tools > Create Metadata Template` — name it: Agency_Default_Copyright

Recommended fields:
- Creator and Author
- Copyright Notice: Copyright [Year] [Agency Name]
- Rights: All rights reserved
- Description: brief content description
- Keywords: client name, product type, year

Apply to any file or folder selection: `Tools > Append Metadata` — select your template

---

## Common Bridge Workflows

| Task | Path |
|---|---|
| View all files in a project | Folders panel — navigate to project folder |
| Filter by file type | Filter panel — File Type |
| Find all unrated files | Filter panel — Rating — No Rating |
| Open file in correct app | Double-click thumbnail |
| Open RAW file in Camera Raw | Double-click .CR2 / .ARW / .DNG file |
| Export a contact sheet | Output — PDF — Contact Sheet layout |
