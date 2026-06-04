# Social Media Export Guide

## Universal Rules for All Platforms
- Colour mode: RGB and sRGB always
- No embedded ICC profiles needed (platforms strip them)
- JPEG for photos and complex images, Quality 80–90
- PNG for graphics with text, flat colour, or transparency
- Resolution: 72 ppi (pixel dimensions matter, not dpi)
- Strip all metadata before uploading

---

## Platform Specifications

### Instagram
| Format | Dimensions px | Ratio |
|---|---|---|
| Feed Square | 1080 x 1080 | 1:1 |
| Feed Portrait | 1080 x 1350 | 4:5 |
| Feed Landscape | 1080 x 566 | 1.91:1 |
| Stories and Reels | 1080 x 1920 | 9:16 |
| Profile Picture | 320 x 320 | 1:1 |

### Facebook
| Format | Dimensions px |
|---|---|
| Feed Post | 1200 x 630 |
| Square Post | 1200 x 1200 |
| Stories | 1080 x 1920 |
| Cover Photo | 851 x 315 |
| Profile Picture | 170 x 170 |
| Event Cover | 1920 x 1080 |

### LinkedIn
| Format | Dimensions px |
|---|---|
| Post Image | 1200 x 628 |
| Post Square | 1080 x 1080 |
| Company Logo | 300 x 300 |
| Cover Photo | 1128 x 191 |

### Twitter and X
| Format | Dimensions px |
|---|---|
| Post Image | 1200 x 675 |
| Header | 1500 x 500 |
| Profile Picture | 400 x 400 |

### WhatsApp Status and Broadcast
| Format | Dimensions px |
|---|---|
| Status | 1080 x 1920 |
| Shared Image | 1080 x 1080 |

---

## Export from Photoshop

`File > Export > Export As`
- Format: JPEG or PNG
- Colour Space: Convert to sRGB
- Resize to exact platform dimensions before export

## Export from InDesign

Set document to exact pixel dimensions.
`File > Export` — JPEG or PNG
Resolution: 72 ppi

---

## File Naming

```
[client]_[platform]_[format]_[version].[ext]

Examples:
brandx_instagram_square_v2.jpg
agency_facebook_cover_2026.jpg
brandx_linkedin_productlaunch_v1.png
```
