---
name: Assa Raviv — Composer & Sound Designer
description: A quiet, paper-and-ink editorial portfolio for a Tel Aviv composer, with a single brass-gold accent and work revealed on hover.
colors:
  brass-gold: "#c8a96e"
  brass-deep-text: "#7a5a24"
  ink: "#0f0d0b"
  paper: "#f4f1eb"
  muted-taupe: "#7a7268"
  hairline: "rgba(15,13,11,0.11)"
typography:
  wordmark:
    fontFamily: "'Unbounded', sans-serif"
    fontSize: "1.5rem"
    fontWeight: 900
    letterSpacing: "-0.02em"
  display:
    fontFamily: "'Instrument Sans', -apple-system, BlinkMacSystemFont, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "clamp(1.4rem, 2.8vw, 2.4rem)"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "'Cormorant Garamond', serif"
    fontSize: "1.8rem"
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: "0em"
  body:
    fontFamily: "'Cormorant Garamond', serif"
    fontSize: "1.35rem"
    fontWeight: 300
    lineHeight: 1.75
    letterSpacing: "0em"
  label:
    fontFamily: "'Instrument Sans', -apple-system, BlinkMacSystemFont, 'Helvetica Neue', Arial, sans-serif"
    fontSize: "0.72rem"
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: "0.12em"
rounded:
  none: "0px"
spacing:
  grid-seam: "2px"
  section-y-desktop: "4rem"
  section-y-mobile: "2.5rem"
  section-x-desktop: "3rem"
  section-x-mobile: "1.25rem"
components:
  nav-link:
    textColor: "{colors.muted-taupe}"
    typography: "{typography.label}"
  nav-link-hover:
    textColor: "{colors.ink}"
  card-badge:
    backgroundColor: "rgba(15,13,11,0.72)"
    textColor: "{colors.brass-gold}"
    typography: "{typography.label}"
    padding: "0.4rem 0.65rem"
  card-client:
    textColor: "{colors.paper}"
    typography: "{typography.display}"
---

# Design System: Assa Raviv — Composer & Sound Designer

## Overview

**Creative North Star: "The Score Page"**

The site reads like a hand-bound orchestral score laid open: warm cream paper, near-black ink, and exactly one metallic accent — a brass gold used the way a score uses a single colored pencil mark. Everything else is restraint: flat surfaces, hairline rules, sharp unrounded corners, and a serif voice (Cormorant Garamond) reserved for the About-section prose and section titles, paired with a quiet all-caps sans (Instrument Sans) for everything functional — navigation, labels, badges, captions, the card-hover client name — plus one heavy display face (Unbounded, 900) reserved for the nav wordmark alone.

The work itself supplies the color and motion. Thumbnails sit as dense, edge-to-edge grids separated by 2px hairline seams, like contact sheets; on hover, a dark scrim rises, a looping preview plays, and the client name and accolades stagger into view. At rest the grid is a quiet wall of imagery; the page's own chrome never competes with it.

Explicitly rejected: dark-mode "tech portfolio" tropes — neon accents, glassmorphism, gradients, glowing borders, rounded "SaaS card" surfaces. This is paper and ink, not a dashboard.

**Key Characteristics:**
- Two-tone base (warm paper / near-black ink) plus exactly one accent hue (brass gold), never a second.
- Serif (Cormorant Garamond) reserved for About-section prose and section titles; sans (Instrument Sans) for every functional/label/caption role and the card-hover client name; a heavy display face (Unbounded) for the nav wordmark alone.
- Zero border-radius anywhere — every edge is sharp.
- No shadows; depth comes from ink/paper value contrast, translucent scrims, and backdrop blur only.
- Metadata (client, campaign, recognition) is hidden at rest and revealed on hover/touch, not shown persistently.

## Colors

A two-tone paper/ink base carries the whole system; one brass-gold accent is the only hue allowed beyond it.

### Primary
- **Brass Gold** (#c8a96e): The system's one accent. Used decoratively on dark (ink) surfaces only — award badges on card thumbnails, uppercase micro-labels on the dark awards/modal chrome. Low contrast against paper, so it never appears as body text on the light background.
- **Deep Brass** (#7a5a24): The same accent, darkened to carry text-contrast duty (≥4.5:1) wherever the gold needs to sit directly on the paper background — currently the italicized emphasis inside About-section prose. Same hue family as Brass Gold; treat it as that color's "on-paper" tone, not a second accent.

### Neutral
- **Near-Black Ink** (#0f0d0b): Primary text color on paper; the page background for the awards grid, brand/film cards, footer-adjacent dark chrome, and the video modal.
- **Warm Paper** (#f4f1eb): The page's base background and the primary text color on dark (ink) surfaces.
- **Soft Taupe** (#7a7268): Secondary/muted text — nav links at rest, the About section's vertical label, contact links, footer copy.
- **Hairline** (rgba(15,13,11,0.11)): Section dividers, the nav's bottom border. Always a low-opacity tint of ink, never a flat gray.

### Named Rules
**The Single Accent Rule.** Brass gold is the only hue in the system besides ink and paper. It never multiplies into a second accent color, and it never appears as small-print body text directly on paper — use Deep Brass there instead.

## Typography

**Wordmark Font:** Unbounded, weight 900 only (with sans-serif fallback) — a single deliberate exception, used only for the nav wordmark ("Assa Raviv"), uppercase, tracked -0.02em. Loaded as a single weight with a text subset (only the letters the wordmark needs) to keep it light.
**Display Font:** Instrument Sans (with system sans fallback)
**Headline Font:** Cormorant Garamond (serif fallback) — section titles only.
**Body Font:** Cormorant Garamond (serif fallback) — reserved for the About-section prose; shared with the headline role above.
**Label Font:** Instrument Sans (with system sans fallback)

**Character:** A heavy, geometric display face announces the name once in the nav; a quiet serif carries section titles and the About-section prose — anything meant to read as a heading or a sentence; and a plain, humanist sans (Instrument Sans) handles everything else functional — navigation, labels, badges, captions, the card-hover client name. The pairing reads as editorial rather than corporate — closer to a type specimen or a film credits sequence than a SaaS marketing page.

### Hierarchy
- **Wordmark** (900, 1.5rem desktop / 1.25rem tablet / 1.1rem phones, tracked -0.02em, uppercase): The nav wordmark only, in Unbounded — the one display moment in the chrome.
- **Display** (700, `clamp(1.4rem, 2.8vw, 2.4rem)`, line-height 1): The client/project name revealed on card hover — the boldest, largest text in the body of the page, reserved for that one moment.
- **Headline** (300, 1.8rem desktop / 1.4rem phones, line-height ~1.2): Section titles ("Brand Work", "Film & TV", "About"), in Cormorant Garamond.
- **Body** (300, 1.35rem desktop / 1.1rem mobile, line-height 1.75): About-section prose, set in serif — the same serif voice as the headline role above.
- **Label** (400, ~0.7–0.75rem, letter-spacing 0.12–0.22em, uppercase): Nav links, contact links, the About sidebar label, footer copy, card type captions, award badges, and the modal title/close control. The system's workhorse sans usage.

### Named Rules
**The Serif-Reads, Sans-Labels Rule.** Cormorant Garamond carries anything meant to be read as a heading or a sentence — section titles and the About-section paragraphs. Everything functional or navigational — labels, captions, badges, the card-hover client name, the modal chrome — runs in Instrument Sans, uppercase and tracked where it's a caption. The nav wordmark is the single exception to both: it runs in Unbounded, the system's only display face.

## Layout

A single max-width container (1600px), centered, holds every section. The nav is sticky-top with a blurred, translucent paper background (`backdrop-filter: blur(10px)` over `rgba(244,241,235,0.96)`) so it stays legible over scrolling content without a hard edge.

Work grids (`.brand-grid`, `.film-grid`) are dense, edge-to-edge tile grids with a 2px gap between cards — the gap is just enough to read as a seam, not a gutter, so the grid reads as one continuous contact sheet. Brand Work and Sonic Identity run 2–3 columns; Film & TV runs 2 (1 on mobile). The About section is a fixed 160px label column plus a flexible prose column on desktop, stacking to one column on mobile.

Section rhythm: 4rem vertical / 3rem horizontal padding on desktop, dropping to 2.5rem / 1.25rem on mobile (≤768px), with further tightening at 600px (nav becomes a two-row stack) and 480px (grids collapse to one column).

## Elevation & Depth

Flat by default — there are no box-shadows anywhere in the system. Depth is conveyed entirely through value contrast (ink vs. paper), translucent dark scrims over imagery (`rgba(15,13,11,0.45–0.88)`), and one instance of backdrop blur on the sticky nav. A hovered card doesn't lift or cast a shadow; it reveals a scrim and a staggered reveal of text instead.

### Named Rules
**The Flat-By-Default Rule.** No box-shadow, ever. Depth and focus come from opacity layering (scrims, translucent chrome) and backdrop blur only — never from elevation/shadow.

## Shapes

Every corner in the system is sharp — no `border-radius` appears anywhere, on cards, badges, the modal frame, or any other surface. Form language leans toward the rectangular, grid-aligned geometry of a contact sheet or a printed layout, reinforced by the 2px hairline seams between grid tiles and 1px hairline borders between sections.

### Named Rules
**The No-Radius Rule.** Zero border-radius across the entire system. A rounded corner anywhere would immediately read as "app UI" rather than the printed-page character this system is built on.

## Components

### Cards (Brand/Film/Sonic Identity tiles)
- **Corner Style:** Sharp (0 radius).
- **Background:** Near-Black Ink; the thumbnail image/video fills the tile (`object-fit: cover`), lightly punched up with `contrast(1.08) brightness(1.04) saturate(1.12)`.
- **Rest state:** Only the image is visible; a small always-on badge chip (translucent ink background, Brass Gold uppercase label) may sit pinned top-left for award recognition.
- **Hover/Touch:** Image scales to 1.045 (0.6s, `cubic-bezier(0.22, 1, 0.36, 1)`); a secondary MP4 preview crossfades in over the static thumbnail; a dark scrim (`rgba(15,13,11,0.45)`) rises over the whole tile; the client name (Display type) and a caption row (type + badge) stagger up from 14px below with a fade, the caption row trailing the name by ~60ms. On touch devices (no hover), the scrim and caption stay permanently visible as a bottom-anchored gradient caption instead of a full-tile reveal.
- **Internal Padding:** 1.5rem around the centered overlay content; 0.9rem (0.6rem mobile) inset for the corner badge.

### Navigation
- **Style:** Sticky top, blurred translucent paper background, 1px ink hairline bottom border.
- **Wordmark:** Unbounded 900, uppercase, tracked -0.02em, Ink — the system's one display moment in the chrome.
- **Links:** Label type (Instrument Sans), Soft Taupe at rest, Ink on hover, 0.2s color transition, no underline.
- **Mobile (≤600px):** Wordmark sits on its own line above the links; the full-label links wrap onto a second row (small even gaps) instead of truncating.

### Modal (video lightbox)
- **Style:** Full-viewport scrim (`rgba(15,13,11,0.88)`) behind a centered 16:9 frame (max 900px) holding a Vimeo iframe; frame background is pure black, no radius, no border.
- **Chrome:** Title and close control sit above the frame (not overlaid on the video) in small uppercase Label type (Instrument Sans), Paper at ~55–60% opacity, Paper at full opacity on hover for the close control.
- **Transition:** Opacity-only fade (0.3s); no scale or slide.

## Do's and Don'ts

### Do:
- **Do** keep the system to exactly three hues: Ink, Paper, and the one Brass Gold accent (plus its Deep Brass on-paper variant).
- **Do** set the About-section prose and section titles in Cormorant Garamond, and anything functional/navigational/caption-level in uppercase, tracked Instrument Sans; reserve Unbounded for the nav wordmark alone.
- **Do** keep every corner sharp — no `border-radius` anywhere in the system.
- **Do** reveal card metadata (client name, campaign, recognition) on hover/touch rather than showing it at rest; let the grid read as pure imagery until the visitor engages.
- **Do** use Deep Brass (#7a5a24), not Brass Gold (#c8a96e), whenever gold text sits directly on the paper background — Brass Gold only passes contrast on dark (ink) surfaces.

### Don't:
- **Don't** add a second accent color. Color richness comes from the photography/video content, not from the UI palette.
- **Don't** add shadows, elevation, glassmorphism, or glow effects — depth is flat-plus-blur only.
- **Don't** round any corner — rounded surfaces read as generic app/SaaS chrome, which this system is deliberately not.
- **Don't** drop functional or label-level text below an ~11px rendered floor for the sake of a smaller-looking caption; the tracked-caps treatment already reads as quiet without going illegibly small.
