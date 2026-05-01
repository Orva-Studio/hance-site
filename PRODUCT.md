# Product

## Register

brand

## Users

Three overlapping audiences:

1. **Filmmakers and colorists** who want a film look but live partly in scripted pipelines — folder-batch grading, ingest automation, no per-clip GUI fiddling.
2. **Developer educators, devrel, and technical creators** who shoot screencasts, talks, and tutorials and want their footage to feel cinematic without learning DaVinci.
3. **General video makers** who already trust the CLI/terminal and want one binary that does color, halation, bloom, grain, and vignette in a single GPU pass — no subscriptions, no plugins, no cloud upload.

Context of use: at a desk, on their own machine, processing footage they already own. They are technically comfortable. They evaluate by reading the README and trying it.

## Product Purpose

Hance is a cinematic film-look engine that runs locally, GPU-accelerated, as a single binary with an optional browser UI. The marketing site's job is to make the right person download it within one visit. Success = a download. Secondary success = the visitor understands what Hance is and isn't (alpha, local-first, pipeline-shaped) before they install.

## Brand Personality

Technical, confident, indie-craft.

- **Technical** — speaks the language of codecs, CRF, GPU, batch. No softening, no analogies for non-technical audiences.
- **Confident** — short declarative sentences. Names what it does. Doesn't oversell, doesn't apologize for being alpha — states it plainly.
- **Indie-craft** — made by a person, not a company. Honest about scope, opinionated about defaults, no enterprise theatre.

Tone is closer to a tool's man page than a SaaS landing page. Dry humor allowed; hype is not.

## Anti-references

- Generic SaaS marketing sites: cream backgrounds, abstract isometric illustrations, "Trusted by" logo strips, three-column feature cards with icons.
- AI-tool aesthetic: neon gradients, animated mesh backgrounds, "AI-powered" hero copy, glassmorphic stat tiles.
- Adobe / enterprise creative-cloud marketing: stock-photo creators, lifestyle hero shots, multi-tier pricing tables.
- "AI-generated movie poster" hero treatment: oversaturated stylized stills meant to look cinematic but signaling slop.
- Crypto/Web3 aesthetic: dark + neon-cyan + grid backgrounds.

Reference territory (for feel, not to copy): **dehancer.com** (cinema-grading heritage, real footage front and center, restrained chrome), **pencil.dev** (oversized confident type on the homepage, minimal scaffolding, video/preview as the proof). The site should feel like one of those, not like a typical dev-tool landing page.

## Design Principles

1. **Show the look, don't describe it.** The homepage proves Hance with footage, not adjectives. A before/after or graded reel is the hero, not a feature list.
2. **One CTA — download.** Everything on the page bends toward installing the CLI. Secondary actions (docs, GitHub, UI demo) are present but quiet.
3. **Practice what you preach.** A film-look tool's site should itself look color-graded — considered contrast, restrained palette, real cinematic still-frame energy. No flat developer-tool greys.
4. **Honest about alpha.** State the maturity plainly where it matters (install, hero subhead). Confidence without overpromising is the whole brand.
5. **Type does the heavy lifting.** Bold, large, opinionated typography carries the page. Decorative chrome stays minimal.

## Accessibility & Inclusion

- WCAG 2.2 AA as the floor. Contrast checked against actual rendered colors, not token names.
- Respect `prefers-reduced-motion` — any scroll-driven or auto-playing video has a static fallback and pause control.
- Keyboard reachable: download CTA, FAQ accordion, video controls.
- No color-only signaling. Status (alpha, beta, stable) carries a text label.
