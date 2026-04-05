# Vibe Coded Projects Section — Design Spec

**Date:** 2026-04-05  
**Status:** Approved

## Overview

Add a new "Vibe Coded Projects" section to `index.html` showcasing personal side projects built with AI assistance, distinct from formal academic research.

## Placement

Between the Hyperscape section and the Research section (after the Hyperscape `<table>` block, before the Research `<table>` block).

## Section Structure

### Heading
A heading table matching the existing Research heading pattern:
```html
<table> <tr> <td> <h2>Vibe Coded Projects</h2> </td> </tr> </table>
```
No `bgcolor` highlight — keeps it visually distinct from Hyperscape.

### Card Grid
Reuse the existing `.pub-grid` / `.pub-card` CSS classes (already defined in `stylesheet.css`) with one card per project.

## First Project: Khana

| Field | Value |
|-------|-------|
| Thumbnail | `http://khana.ayushsaraf.com/images/meals.png` (external URL, reused directly) |
| Title | Khana |
| Title link | `http://khana.ayushsaraf.com` |
| Description | Log food by talking to Claude. Tracks your pantry, macros, and grocery list — runs entirely inside a Claude Code session. |
| Links | `live` → `http://khana.ayushsaraf.com` / `github` → `https://github.com/ayush29feb/khana` |

## Implementation

Single file change: `index.html` — insert ~25 lines of HTML between the closing `</table>` of the Hyperscape block (line ~97) and the opening `<table>` of the Research block (line ~98).

No CSS changes needed — `.pub-grid` and `.pub-card` styles already exist.
