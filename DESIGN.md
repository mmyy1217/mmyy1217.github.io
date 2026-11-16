---
name: mmyy1217.github.io
description: Minimal Swiss technical index sheet for public AI compiler work
colors:
  ground: "#f7f7f5"
  surface: "#ffffff"
  ink: "#111214"
  ink-muted: "#52555a"
  accent: "#164888"
  line: "#dfded9"
  line-strong: "#c2c1ba"
typography:
  display:
    fontFamily: "'Archivo', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif"
    fontSize: "clamp(2rem, 4.8vw, 2.75rem)"
    fontWeight: 600
    lineHeight: 1.12
    letterSpacing: "-0.03em"
  body:
    fontFamily: "'Archivo', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.55
  title:
    fontFamily: "'Archivo', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif"
    fontSize: "1rem"
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: "-0.015em"
  label:
    fontFamily: "'Archivo', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.45
  caption:
    fontFamily: "'Archivo', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif"
    fontSize: "0.75rem"
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "0.01em"
rounded:
  sm: "3px"
  md: "4px"
spacing:
  row-y: "1.05rem"
  row-x: "0.85rem"
  lead-bottom: "2.5rem"
  footer-top: "2rem"
components:
  index-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "1.05rem 0.85rem"
  index-link-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.accent}"
---

## Overview

A restraint-first technical index sheet for `mmyy1217`. The page establishes focus through typographic scale, warm paper ground contrast, and a hairline-ruled link list that connects seamlessly into monochrome tools such as ACKB.

## Colors

- **Ground (`#f7f7f5`):** Warm archival paper canvas used across the viewport.
- **Surface (`#ffffff`):** Active hover/focus surface for index rows.
- **Ink (`#111214`) & Muted (`#52555a`):** High-contrast carbon primary text and cool graphite descriptions/footer.
- **Accent (`#164888`):** Deep blueprint cobalt reserved for interactive emphasis (`Live UI` tag, hover/focus title shift, text selection, and focus ring).
- **Rules (`#dfded9`, `#c2c1ba`):** Hairline row dividers and scrollbar thumb.

## Typography

- Self-hosted `@fontsource/archivo` (`400`, `500`, `600`) with zero external font host dependency.
- Primary statement uses tight negative tracking (`-0.03em`) and balanced wrapping; footer uses `tabular-nums`.

## Layout

- Single centered column (`max-width: 34rem`) inside a `100svh` CSS Grid shell with fluid edge padding (`clamp(1.25rem, 5vw, 2.5rem)`).
- Anchored by a `2px` solid ink top rule above `1px` hairline-separated rows.

## Elevation & Depth

- Flat tonal layering only (`#f7f7f5` ground to `#ffffff` active row fill); no drop shadows or glass blur.

## Shapes

- Crisp `3px` hover row radius and square-cap `16x16` directional arrow SVG (`stroke-width: 1.6`).

## Components

- **Statement & Lead:** Direct `<h1>` statement without an eyebrow label, paired with a single-sentence scope line (`max-width: 44ch`).
- **Index List (`.index-list` / `.index-link`):** Interactive rows where hovering or keyboard-focusing one item dims inactive siblings (`opacity: 0.56`) and slides the directional arrow `(2px, -2px)` via `--ease-out-expo`.

## Do's and Don'ts

- **Do:** Keep links curated, public-safe, and free of personal real-name references.
- **Do:** Keep the first viewport centered and self-contained without client JS bundles.
- **Don't:** Add eyebrows/kickers above the primary heading, decorative background grids, or card boxes around the index.
