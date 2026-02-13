# Logo Integration Instructions

## Files
- `logo-bilateral.svg` — Full logo mark, light background
- `logo-bilateral-dark.svg` — Full logo mark, dark background  
- `favicon.svg` — Simplified mark for browser tab favicon

## Sizing Rules (IMPORTANT)

The logo height should always scale relative to the adjacent text's cap-height (the height of a capital letter). This keeps proportions consistent regardless of where the logo appears.

**Logo beside site title text:**
- Logo height = **1.5× the cap-height** of the adjacent site title text
- Example: If "The Limit Case" is set at `font-size: 1.4rem` (~22px rendered), the cap-height is roughly 16px, so the logo should be **24px tall**
- Example: If the title is `clamp(2.8rem, 6vw, 4.2rem)` on the welcome page (~45-67px rendered), the logo scales proportionally — roughly **48-72px tall**
- The logo should vertically center-align with the text baseline/midline
- Gap between logo and text: approximately **0.5em** of the adjacent text size

**Standalone icon (no adjacent text):**
- Use whatever size suits the context
- Favicon: 32x32

**As a decorative divider element:**
- The tiny bilateral mark can replace divider ornaments (like the diamond on the welcome page's horizontal rule)
- Size for dividers: approximately **0.6rem** (scaled to be a subtle accent, not a focal point)
- Use at reduced opacity (0.3-0.5) when serving as a divider ornament

## Title Bar / Header Component

The site-wide header should contain:
1. The bilateral logo SVG (sized per the rules above relative to the title text)
2. Site title: "The Limit Case" in Newsreader, font-weight 300, with "Limit" in italic and accent color
3. Logo and title as a single linked group pointing to `/`

**Light pages:** `logo-bilateral.svg`, ink-colored text (#1a1a1a), accent on "Limit" (#c45d3e)
**Dark pages (homepage):** `logo-bilateral-dark.svg`, light text (rgba(245,240,232,0.92)), accent on "Limit" (#e8764f)

## Color Reference
- Light accent: #c45d3e
- Dark/glow accent: #e8764f  
- Ink (light bg text): #1a1a1a
- Paper (dark bg text): #f5f0e8 at 80-92% opacity
- Asymptote line (light): #d4cdbf
- Asymptote line (dark): rgba(245,240,232,0.08)

## Design Notes
- The logo's center dot (the "limit point") is a key visual motif — it connects to the wormhole center on the homepage
- The right-side curves are intentionally faded — they're reflections, not equal partners
  - Light variant: reflection opacity 0.25 (subtle against white)
  - Dark variant: reflection opacity 0.4–0.45 (boosted for visibility against dark backgrounds)
- The bilateral mark can also serve as a small decorative element in dividers and separators (see divider rules above)
- SVGs use consistent cubic bezier curves — keep these paths unchanged when scaling
