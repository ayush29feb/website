# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static academic personal website built with plain HTML and CSS. The site showcases research publications, professional experience, and academic contributions in computer vision, computer graphics, and machine learning.

## Architecture

### File Structure

- `index.html` - Single-page website containing all content including bio, research publications, and professional activities
- `stylesheet.css` - Styling with Lato font family, custom link colors (#1772d0 primary, #f09228 hover), and responsive media elements
- `images/` - Profile photos, publication thumbnails/videos, and visual assets
- `data/` - BibTeX files for publications (amico.bib, boostingvs.bib, dyndyn.bib, fgvc.bib, omnimatterf.bib, photos3d.bib, rodynerf.bib)
- `CNAME` - GitHub Pages custom domain configuration

### Content Structure

The index.html follows a table-based layout (max-width: 800px, centered) with these sections:

1. **Header**: Bio with profile photo, name, current position at Meta Reality Labs, contact links (Email, Google Scholar, Twitter, Github)
2. **Research Introduction**: Brief research interests summary
3. **Publications**: Research papers displayed with:
   - 25% width left column: Thumbnail image or autoplay video
   - 75% width right column: Title, authors (with name in bold), venue, links (project page, video, paper, code)
   - Highlighted rows (bgcolor="#ffffd0") for select publications
4. **Miscellanea**: Professional service activities (program committee, peer reviewing)

### Visual Design

- Highlighted publications use `bgcolor="#ffffd0"` on table rows
- Publication media uses `.one` and `.two` classes for 160x160px containers
- Videos are set to `muted autoplay loop` for continuous playback
- Responsive hover effects with `.fade` class for opacity transitions

## Development

### Viewing the Site Locally

Since this is a static HTML site, open `index.html` directly in a browser:

```bash
open index.html
```

Or serve with a simple HTTP server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`

### Deployment

This site is configured for GitHub Pages with a custom domain (specified in CNAME). Push to the repository's main branch to deploy.

## Making Changes

### Adding a New Publication

1. Add the publication entry in `index.html` within the publications table
2. Follow the existing pattern: create a `<tr>` element (optionally with `bgcolor="#ffffd0"` for highlighting)
3. Left `<td>`: Add thumbnail image or video in a div with classes `one` and `two`
4. Right `<td>`: Include title (wrapped in `<span class="papertitle">`), authors (your name in `<strong>`), venue in `<em>`, and links
5. Add corresponding BibTeX file to `data/` directory
6. Add media assets (images/videos) to `images/` directory

### Updating Profile Information

Edit the bio section in `index.html` (lines 23-41). The layout uses a 63% text / 40% image split.

### Styling Changes

Modify `stylesheet.css`. Key design tokens:
- Primary link color: `#1772d0`
- Hover color: `#f09228`
- Font: Lato (fallback: Verdana, Helvetica, sans-serif)
- Base font size: 14px
- Name font size: 32px
- Heading font size: 22px
