# Changelog

## 2025-10-20 - Major Website Redesign

### Overview
Complete redesign of personal academic website to better showcase visual/video content and make efficient use of screen space.

### Major Changes

#### 1. Layout & Width
- **Increased site width**: 800px → 1200px (50% wider)
- Implemented responsive design with breakpoints:
  - Desktop (>1025px): 1200px max-width
  - Tablet (769-1024px): 95% width
  - Mobile (<768px): 100% width with padding

#### 2. Bio Section
- Made profile photo more compact (40% → 25% width)
- Added circular border-radius to profile photo (max-width: 150px)
- Expanded bio text area (63% → 75% width)
- Updated bio to mention Hyperscape and current work on 3D world generation

#### 3. Hyperscape Featured Section
- Moved Hyperscape to prominent hero section at top of page
- Enlarged video to full 1200px width (from 800px)
- Added side-by-side layout: 60% video, 40% description on desktop
- Embedded 2 YouTube review videos in responsive grid
- Added press coverage links (TechCrunch, CNET, UploadVR, The Ghost Howls, Gizmodo)
- Highlighted with yellow background (#ffffd0)
- Updated launch date: September 2025 at Meta Connect
- Downloaded and embedded 20MB Hyperscape demo video from Twitter

#### 4. Publications Grid Redesign
- **Converted from table-based layout to CSS Grid**
- **Grid configuration**:
  - 3 columns on desktop (>1025px)
  - 2 columns on tablets (769-1024px)
  - 1 column on mobile (<768px)
  - 30px gap between cards
- **Video-first card design**:
  - Large autoplay videos at top (16:9 aspect ratio)
  - Compact title, authors, venue below
  - Venue displayed as styled badge
  - Links row at bottom
  - Hover effect: cards lift up with enhanced shadow
  - All cards uniform size (no featured/highlighted variations)

#### 5. Publication Media Updates
- **Increased video/image sizes**: 160px × 160px → 300px × 300px
- **Added new publications**:
  - Textured Gaussians for Enhanced 3D Scene Appearance Modeling (CVPR 2025)
  - LTM: Lightweight Textured Mesh Extraction and Refinement (CVPR 2024)
- **Fixed broken images**: Converted to use direct video URLs from project pages
- **Updated Hyperscape video**: Replaced static image with autoplay video

#### 6. CSS Enhancements
- Added modern card-based styling with rounded corners (8px border-radius)
- Box shadows for depth (0 2px 8px on normal, 0 4px 16px on hover)
- Smooth transitions for hover effects (transform, box-shadow)
- Responsive video sizing with media queries
- Venue badges styled with primary color (#1772d0)
- Author names in smaller, lighter font (#666)

#### 7. Technical Improvements
- Added `.gitignore` for macOS system files (.DS_Store)
- Created Python script to automate publication conversion
- Maintained all existing links and metadata
- Preserved Jon Barron template credit

### Files Modified
- `index.html` - Complete restructure of publications section, updated bio, added Hyperscape hero
- `stylesheet.css` - Added grid system, card styles, responsive breakpoints
- `.gitignore` - Added macOS file exclusions

### Files Added
- `images/hyperscape.mp4` (20MB) - Hero video for Hyperscape section
- `CHANGELOG.md` - This file

### Media Assets
- All publication videos now use direct URLs or local files
- Video sizes: 300×300px (responsive to 200×200px on mobile)
- Hyperscape hero video: Full width (1200px max)

### Publication Count
Total: 9 publications displayed in grid
- 2025: 1 (Textured Gaussians - CVPR)
- 2024: 1 (LTM - CVPR)
- 2023: 2 (OmnimatteRF - ICCV, RoDyNeRF - CVPR)
- 2022: 1 (Boosting - CVPR)
- 2021: 2 (DynDyn - ICCV, AMICO - BMVC)
- 2020: 2 (FGVC - ECCV, 3D Photos - SIGGRAPH)

### Design Goals Achieved
✅ Eliminated wasted whitespace
✅ Made video content prominent and engaging
✅ Created clean, modern visual presentation
✅ Improved mobile/tablet experience
✅ Maintained professional academic aesthetic
✅ Increased information density without clutter
✅ Fast loading with optimized layout
✅ Cross-platform compatibility

### Browser Compatibility
Tested on modern browsers with CSS Grid support:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)
