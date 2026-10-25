# Color Palette Guide

## 1. Semantic color roles
Use semantic tokens rather than scattering raw HEX values through components.

| Token | Purpose |
|---|---|
| `primary` | Main actions and links |
| `secondary` | Supporting actions |
| `background` | Main page background |
| `surface` | Cards, panels, menus |
| `text` | Main text |
| `muted` | Secondary text |
| `border` | Borders and dividers |
| `accent` | Highlights |
| `success` | Successful outcomes |
| `warning` | Caution states |
| `error` | Error states |
| `focus` | Keyboard focus indicator |

## 2. Example palettes

These are starter palettes. Check contrast and brand suitability before using them in production.

### Indigo / Violet
- Primary: `#6366F1`
- Secondary: `#8B5CF6`
- Accent: `#06B6D4`
- Background: `#FFFFFF`
- Surface: `#F8FAFC`
- Text: `#0F172A`
- Muted: `#64748B`
- Border: `#E2E8F0`
- Success: `#15803D`
- Warning: `#B45309`
- Error: `#B91C1C`

### Dark Slate / Cyan
- Primary: `#818CF8`
- Secondary: `#A78BFA`
- Accent: `#22D3EE`
- Background: `#0F172A`
- Surface: `#1E293B`
- Text: `#F8FAFC`
- Muted: `#CBD5E1`
- Border: `#334155`
- Success: `#4ADE80`
- Warning: `#FBBF24`
- Error: `#F87171`

### Earth / Natural
- Primary: `#365314`
- Secondary: `#78716C`
- Accent: `#B45309`
- Background: `#FAFAF9`
- Surface: `#F5F5F4`
- Text: `#1C1917`
- Muted: `#57534E`
- Border: `#D6D3D1`
- Success: `#166534`
- Warning: `#A16207`
- Error: `#B91C1C`

## 3. Importing palette data
When a user supplies HEX codes, a palette file, or a URL:
1. Read the content if the current environment supports access.
2. Validate color syntax (e.g. `#RGB` or `#RRGGBB`).
3. Ask about missing semantic roles only if they materially affect the task.
4. Map colors to semantic tokens.
5. Check foreground/background contrast using a reliable tool when available.
6. Report inaccessible URLs or unverified contrast honestly.

A URL may point to a page rather than raw palette data. If extraction fails, ask the user to paste the palette or provide a raw file URL.

## 4. Generating a palette
Consider:
- brand personality;
- audience and product context;
- light or dark theme;
- contrast and legibility;
- status colors;
- color-blind-friendly distinctions;
- consistency with the existing design.

Provide each color's HEX value and semantic purpose. Do not rely on color alone to communicate status.

## 5. Light and dark themes
Define separate semantic tokens for each theme. Do not simply invert every color. Verify text, borders, focus states, and status colors in both themes.

## 6. Contrast and accessibility
Prefer WCAG contrast checks when tooling is available. As a general target, normal text should meet 4.5:1 contrast and large text 3:1 for WCAG AA. Report the tested foreground/background pair and result; if not tested, say so.
