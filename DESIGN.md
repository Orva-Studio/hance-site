---
name: Hance
description: Marketing site for a cinematic film-look CLI. Drenched dark warm-cyan surface with a single halation-orange accent.
colors:
  cinema-black: "oklch(0.13 0.012 220)"
  cinema-black-raised: "oklch(0.17 0.013 220)"
  cinema-black-edge: "oklch(0.22 0.014 220)"
  print-cream: "oklch(0.94 0.015 80)"
  print-cream-mid: "oklch(0.72 0.012 80)"
  print-cream-shadow: "oklch(0.52 0.010 80)"
  halation-orange: "oklch(0.74 0.18 55)"
typography:
  display:
    fontFamily: "\"Inter Tight\", Inter, system-ui, sans-serif"
    fontSize: "clamp(3.25rem, 11.5vw, 11rem)"
    fontWeight: 500
    lineHeight: 0.92
    letterSpacing: "-0.045em"
  headline:
    fontFamily: "\"Inter Tight\", Inter, system-ui, sans-serif"
    fontSize: "clamp(2.25rem, 5.5vw, 4.25rem)"
    fontWeight: 500
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  title:
    fontFamily: "\"Inter Tight\", Inter, system-ui, sans-serif"
    fontSize: "clamp(1.5rem, 2.4vw, 1.875rem)"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.015em"
  body:
    fontFamily: "\"Inter Tight\", Inter, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "normal"
  body-lg:
    fontFamily: "\"Inter Tight\", Inter, system-ui, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "-0.005em"
  mono:
    fontFamily: "\"JetBrains Mono\", \"IBM Plex Mono\", ui-monospace, monospace"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "0"
  label:
    fontFamily: "\"JetBrains Mono\", ui-monospace, monospace"
    fontSize: "0.75rem"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "0.18em"
rounded:
  xs: "2px"
  sm: "4px"
  md: "6px"
  pill: "9999px"
spacing:
  hairline: "1px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "40px"
  section: "80px"
  section-lg: "112px"
components:
  button-install:
    backgroundColor: "{colors.cinema-black}"
    textColor: "{colors.print-cream}"
    rounded: "{rounded.pill}"
    padding: "10px 12px 10px 20px"
    typography: "{typography.mono}"
  button-install-hover:
    backgroundColor: "{colors.cinema-black-raised}"
    textColor: "{colors.print-cream}"
  button-download:
    backgroundColor: "{colors.cinema-black}"
    textColor: "{colors.print-cream}"
    rounded: "{rounded.pill}"
    padding: "6px 14px"
    typography: "{typography.label}"
  button-download-hover:
    backgroundColor: "oklch(0.74 0.18 55 / 0.10)"
  chip-alpha:
    backgroundColor: "transparent"
    textColor: "{colors.print-cream-shadow}"
    rounded: "{rounded.pill}"
    padding: "0px"
    typography: "{typography.label}"
  chip-copy:
    backgroundColor: "oklch(0.74 0.18 55 / 0.10)"
    textColor: "oklch(0.74 0.18 55 / 0.90)"
    rounded: "{rounded.pill}"
    padding: "2px 10px"
    typography: "{typography.label}"
  code-block:
    backgroundColor: "oklch(0.17 0.013 220 / 0.50)"
    textColor: "{colors.print-cream}"
    rounded: "{rounded.md}"
    padding: "16px 20px"
    typography: "{typography.mono}"
  faq-row:
    backgroundColor: "transparent"
    textColor: "{colors.print-cream}"
    rounded: "{rounded.xs}"
    padding: "24px 0px"
    typography: "{typography.title}"
  divider:
    backgroundColor: "oklch(0.22 0.014 220 / 0.70)"
    height: "1px"
    width: "100%"
---

# Design System: Hance

## 1. Overview

**Creative North Star: "The Local Darkroom"**

Hance is a film-look engine that runs on your machine, in your terminal, on your GPU. The site is its proof: the page itself looks color-graded. A drenched, warm-cyan-tinted near-black surface holds the entire experience like an unlit darkroom; a single halation-orange accent does all the signaling, the way a safelight or a strip of leader does. There is no chrome theatre here. Type carries the page. The product gets out of its own way.

The system rejects every visual reflex of its category. It is not the navy-and-cyan dev-tool dashboard. It is not the cream-and-charcoal SaaS landing page. It is not the neon-on-black AI-tool aesthetic. It is not the Adobe-blue creative-cloud marketing site. It refuses gradient text, glassmorphic stat tiles, identical icon-card grids, and isometric illustration. Every section breathes differently; nothing is wrapped in a default container "for safety". When in doubt the answer is bigger type, less chrome, more rest.

**Key Characteristics:**
- Drenched warm-cyan-black surface, one halation-orange accent (≤8% of any viewport).
- Type-led hierarchy: oversized grotesk display, mono captions, no decorative icon families.
- Variable vertical rhythm. Each section sets its own pace.
- Single-page, single-job: every block bends toward `download`.
- The placeholder itself is graded. There is no "neutral" surface anywhere in the system.

## 2. Colors: The Drenched Darkroom Palette

A near-monochrome of warm-cyan-tinted blacks, lit from one direction by a single halation orange. All values in OKLCH; sRGB conversion is acceptable in build output but the canonical form is OKLCH.

### Primary
- **Halation Orange** (`oklch(0.74 0.18 55)`): The system's only accent. Used for the install pill border, the download pill border, the play-button ring and glow, the alpha-status dot, the FAQ `+` indicator, the before/after handle, the mono `$` glyph in code blocks, and link-underline reveals on hover. Nothing else gets it. Its rarity is the message.

### Neutral
- **Cinema Black** (`oklch(0.13 0.012 220)`): The page surface. Tinted toward warm-cyan to read as "darkroom" rather than "void". Never substitute `#000`.
- **Cinema Black, Raised** (`oklch(0.17 0.013 220)`): Used for the code-block panel, the FAQ row hover wash, and the install-pill internal seat.
- **Cinema Black, Edge** (`oklch(0.22 0.014 220)`): The only color allowed for dividers and 1px rings. Hairline rules between sections, the FAQ divider stack, video frame ring.
- **Print Cream** (`oklch(0.94 0.015 80)`): Primary type. Warm-tinted off-white; never `#fff`. Used on display and headline type, install command text, FAQ question text, code body.
- **Print Cream, Mid** (`oklch(0.72 0.012 80)`): Secondary type. Subhead, FAQ answer body, paragraph copy, the second-line of the hero headline.
- **Print Cream, Shadow** (`oklch(0.52 0.010 80)`): Tertiary type. Mono captions, alpha-status text, footer meta, before/after section labels.

### Named Rules

**The One Light Rule.** Halation Orange is used on no more than 8% of any rendered viewport. It is the safelight. If the page starts feeling orange, an accent is wrong, not the surface.

**The Tinted-Black Rule.** Pure `#000` and pure `#fff` are forbidden. Every neutral carries chroma 0.010–0.015 toward cyan (surfaces) or warm yellow (type). Flat developer-tool greys are anti-brand.

**The No Second Accent Rule.** No green for "success", no red for "error", no blue for "link". Either Halation Orange handles it, or type weight handles it. The palette is monochrome plus one for a reason.

## 3. Typography

**Display Font:** Inter Tight (fallback: Inter, system-ui, sans-serif).
**Body Font:** Inter Tight, same family.
**Mono Font:** JetBrains Mono (fallback: IBM Plex Mono, ui-monospace, monospace).

**Character:** A single grotesk family, set tight, doing all the work. Inter Tight runs from oversized display down to body without mood-shifting. JetBrains Mono carries every machine surface: install commands, code, captions, status labels. The pairing reads as one technical voice with a softer-spoken paragraph register, not as "marketing font + UI font".

### Hierarchy

- **Display** (Inter Tight, weight 500, `clamp(3.25rem, 11.5vw, 11rem)`, leading `0.92`, tracking `-0.045em`): Hero headline only. Two stacked lines, the second muted to Print Cream Mid, treated as one composition.
- **Headline** (Inter Tight, weight 500, `clamp(2.25rem, 5.5vw, 4.25rem)`, leading `0.95`, tracking `-0.025em`): Section openers ("Three commands. Then you ship.", "Questions, plainly answered.").
- **Title** (Inter Tight, weight 500, `1.5–1.875rem`, leading `1.15`): Quickstart step titles, FAQ questions, distinctive in-content type.
- **Body** (Inter Tight, weight 400, `1rem`, leading `1.55`, max measure `65–75ch`): FAQ answers, quickstart step body. Quiet, comfortable.
- **Body, Large** (Inter Tight, weight 400, `1.25rem`, leading `1.4`, measure `~44ch`): Hero subhead only. One occurrence per page.
- **Mono** (JetBrains Mono, weight 400, `0.875rem`, leading `1.55`): Install command, code blocks, inline CLI snippets.
- **Label** (JetBrains Mono, weight 400, `0.75rem`, tracking `0.18em`, uppercase): Section captions, alpha pill, before/after labels, footer meta. The mono voice that surrounds the type-led blocks.

### Named Rules

**The Two-Voice Rule.** Sans for content, mono for the machine. Never set running prose in mono and never set a CLI snippet in sans. The pairing IS the brand.

**The Tight-Stack Rule.** Display and headline type are set with tight leading (`0.92` and `0.95`) and aggressive negative tracking (`-0.045em` / `-0.025em`). Default leading and default tracking on big type look like a draft.

**The One Paragraph Rule.** The hero subhead is the only Body Large in the system. Every other paragraph is Body. Resist the urge to upsize secondary copy.

## 4. Elevation

The system is **flat by default**. There are no decorative box shadows, no card stacks, no "elevation surfaces". Depth is conveyed entirely through tonal layering (Cinema Black → Raised → Edge), 1px hairline rings in Cinema Black Edge, and one purposeful piece of glow.

### Shadow Vocabulary

- **Halation Glow** (`box-shadow: 0 0 60px -10px oklch(0.74 0.18 55 / 0.7)`): Used on exactly one element: the play-button ring on the hero video placeholder. It is the visual rhyme of the brand name. Reuse anywhere else and it becomes meaningless.

### Named Rules

**The Flat-By-Default Rule.** No drop shadows on cards, panels, popovers, or buttons. If a surface needs to feel raised, raise its tonal value (Cinema Black → Raised), not its shadow.

**The Hairline Rule.** Borders and dividers are exactly 1px in Cinema Black Edge (`oklch(0.22 0.014 220 / 0.70)`). Halation-orange borders are reserved for interactive affordances (pills, range handle), and never exceed 1px on the side they sit on.

**The Halation-Once Rule.** The orange glow shadow appears on one element per page. If a second element needs it, the first one stops having it.

## 5. Components

### Buttons

- **Shape:** All interactive pills are full-radius (`rounded-full`). Square corners and small radii are reserved for code blocks and video frames (radius `6px`).
- **Install Pill (signature):** Cinema Black surface, 1px Halation Orange border, mono content, leading `$` in Halation Orange, body `curl ...` in Print Cream, trailing `copy` chip in `oklch(0.74 0.18 55 / 0.10)` with Halation Orange/90 text. On click, the chip label flips to `copied ✓` for 1.5s and the border briefly intensifies to ring-1 Halation Orange. Padding `10px 12px 10px 20px`.
- **Download Pill (nav):** Same pill silhouette as install, smaller. 1px Halation Orange/60 border, sans label, hover tints background `oklch(0.74 0.18 55 / 0.10)` and brightens border to /100.
- **Play Button (proof affordance):** Round, `size-20` (mobile) / `size-24` (desktop), Cinema Black/85 surface with `backdrop-blur-[3px]`, 2px Halation Orange ring, Halation Glow shadow (the only place it appears), Halation Orange triangle SVG. Disabled in v1 (the reel is pending). Cursor stays default; no false affordance.

### Chips

- **Alpha Status Chip:** Bare, no background. Halation Orange/80 dot (1.5px), label in Print Cream Shadow, mono uppercase, tracking `0.18em`. Sits inline next to the install pill, not in the nav.
- **Copy Chip:** Inside the install pill only. Halation Orange/10 background, Halation Orange/90 text, mono uppercase, never appears as a standalone control.

### Cards / Containers

There are no cards in the system. Sections separate with hairline rules and vertical rhythm, not panels. The two element types that approach card-ness:

- **Code Block (Quickstart):** Cinema Black Raised at /50 opacity, 1px Cinema Black Edge ring, radius `6px`, padding `16px 20px`, mono body in Print Cream, leading `$` glyph in Halation Orange/80. Used for CLI snippets only. Never wrap prose.
- **Video Frame (Hero):** `aspect-video`, 1px Cinema Black Edge ring, radius `6px`, the interior is the graded-still placeholder (radial halation gradient + warm-grade base + vignette + SVG film grain at 18% opacity, overlay blend). When real footage lands, swap the interior for `<video>` keeping the ring and radius intact.

### Inputs / Fields

There is one input in the system: the hidden `<input type="range">` underneath the before/after slider. Visually invisible, exists only to provide keyboard control of the comparison. Arrow keys nudge ±1, with the visible Halation Orange handle and 1px vertical bar tracking the value.

### Navigation

- **Top Nav:** No background, no border, generous top padding. Wordmark `hance` left in Inter Tight 500, lowercase, tracking `-0.045em`, hover tints to Halation Orange. Right group: `Docs` (hidden below `sm`), `GitHub`, `Download` (pill). Mono labels for Docs/GitHub at `13px` Print Cream Mid, hover lifts to Print Cream with a Halation Orange underline that draws in via `transform: scaleX(0 → 1)` over 320ms ease-out-expo.
- **FAQ "Navigation":** Native `<details>`/`<summary>` rows. Hairline divider stack, hover wash in Cinema Black Raised/30, leading `+` glyph in Halation Orange that rotates to `45deg` (i.e., `×`) on `[open]` over 300ms ease-out-quart. No chevron icons, no card boundaries.

### Signature: Before/After Comparator

Single 16:8 frame. Left half is the desaturated, low-contrast version of the same scene rendered behind the right half (radial warm-tan gradient base, `filter: saturate(0.7) contrast(0.92)`). Right half is the full graded-still: warm halation gradient, vignette, film grain. A 1px vertical Halation Orange bar with a `40px` Cinema Black circle and Halation Orange ring sits at the divide; clip-path on the right layer is driven by `--pos` custom prop. Drag-to-compare via pointer events on the frame; keyboard via the invisible range input. Labels `before` (Print Cream Mid) and `after` (Halation Orange) sit in mono uppercase pills in the upper corners, on a Cinema Black/60 wash.

## 6. Do's and Don'ts

### Do:

- **Do** keep Halation Orange usage at or below 8% of any viewport. Test by squinting; if the page reads as "an orange site", an accent is misplaced.
- **Do** tint every neutral. Surfaces toward cyan (chroma `0.012–0.014`, hue `220`); type toward warm (chroma `0.010–0.015`, hue `80`).
- **Do** set display and headline type at tight leading (`0.92` / `0.95`) and aggressive negative tracking (`-0.045em` / `-0.025em`). Default tracking on big type is a tell.
- **Do** vary vertical rhythm between sections. The effects strip breathes differently from the FAQ; the quickstart breathes differently from the hero.
- **Do** carry CLI snippets in JetBrains Mono and prose in Inter Tight, never the other way around.
- **Do** pair every accent surface with the alpha-status copy nearby ("alpha. macOS first."). Honesty is part of the brand.
- **Do** prefer hairlines, tonal layering, and whitespace over panels and shadows.

### Don't:

- **Don't** use `#000` or `#fff`. Both are forbidden everywhere in the system.
- **Don't** introduce a second accent color. No green-success, no red-error, no link-blue. The palette is monochrome plus one.
- **Don't** set gradient text (`background-clip: text`). Emphasis comes from weight, scale, and tonal contrast.
- **Don't** use glassmorphism decoratively. The hero play button is the only blur in the system; it is purposeful and singular.
- **Don't** wrap sections in cards or "feature cards". Identical icon+heading+text card grids are explicitly rejected — the strategic line in PRODUCT.md names "three-column feature cards with icons" as anti-brand.
- **Don't** add isometric illustrations, abstract mesh backgrounds, "Trusted by" logo strips, stock-photo lifestyle shots, neon-cyan grids, or animated AI-mesh gradients. These are the named anti-references from PRODUCT.md (SaaS marketing, AI-tool aesthetic, Adobe enterprise, crypto/Web3) and they ship as Don'ts here.
- **Don't** use side-stripe borders (`border-left` greater than 1px as a colored accent on rows or callouts). Use full hairline borders, background tints, or nothing.
- **Don't** write em dashes in copy. Use commas, colons, periods, or parentheses.
- **Don't** animate layout properties (`width`, `height`, `top`, `left`). Animate `transform`, `opacity`, `filter`, `clip-path`, `background-position`. Always ease-out-expo or ease-out-quart, never bounce or elastic.
- **Don't** add a theme toggle. The scene sentence — "a filmmaker at a dim desk at 1am" — forces dark; a "light mode" would dilute the brand.
- **Don't** reuse the Halation Glow shadow on more than one element per page. The play-button ring owns it.
