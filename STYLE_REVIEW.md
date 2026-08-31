# Website Style Review

## Status

**Approved.** This document is the implementation and QA brief for the website redesign.

## Design Direction

- Desired impression: **academic and approachable**.
- The site should feel credible and research-oriented without appearing cold, overly formal, or institutional.
- Use clear hierarchy, readable typography, restrained decoration, and welcoming language.

## Approved Color Palette

| Role | Color | Hex |
|---|---|---|
| Light accent | Honeydew | `#e1f3ea` |
| Primary surface | Parchment | `#f3f2ef` |
| Deep emphasis | Space Indigo | `#21295c` |
| Primary brand | Regal Navy | `#1b3b6f` |
| Interactive accent | Baltic Blue | `#065a82` |

### Semantic Assignments

- Major headings: Regal Navy (`#1b3b6f`).
- Body text and strongest emphasis: Space Indigo (`#21295c`).
- Links, primary buttons, focus indicators, and active navigation: Baltic Blue (`#065a82`).
- Light accents, tags, and subtle highlighted regions: Honeydew (`#e1f3ea`).
- Main canvas and card surfaces: Parchment (`#f3f2ef`) and carefully selected near-white variants where separation is needed.
- All combinations must meet WCAG AA contrast requirements for their text size and role.

### Background Direction

- Use a **flat parchment background** without a gradient.
- The site should fill the viewport instead of appearing as a separate canvas floating over an outer background.
- Use Honeydew only for subtle component accents and Baltic Blue for interactive emphasis.
- Preserve strong contrast and an academic tone without decorative background effects.

## Main Portrait

- Source: `C:/Users/Caleb/Pictures/PersonalImages/WhatsApp Image 2026-08-28 at 9.00.08 AM.jpeg`
- Use as Caleb's main profile image.
- Preserve the original likeness; do not use generative alteration.
- Use responsive cropping and focal-position controls so Caleb's face remains visible at every breakpoint.
- Use a circular crop with a restrained border and soft shadow.
- Place the portrait in the left identity column of the homepage hero.
- Confirm that the face remains centered and that the crop does not overemphasize the dark jacket at small sizes.

## Approved Homepage Reference Direction

- Reference image: `C:/Users/Caleb/AppData/Local/Temp/codex-clipboard-6acf2601-9504-4e22-b376-77aa051bfa97.png`
- Use the reference for composition and visual rhythm, not for its sample identity, content, or exact colors.
- Present the homepage as a full-width page that fits the browser viewport.
- Use a two-column hero:
  - Left: circular portrait, name, role, affiliation, and compact social links.
  - Right: professional summary, CV action, and education cards.
- Translate the reference's bright gradient into a flat parchment base with restrained Honeydew component accents.
- Keep shadows soft and borders restrained so the result remains academic rather than app-like or playful.
- Collapse to a single column on smaller screens with identity first, followed by summary and education.

## Responsive Review Matrix

| Screen class | Width | Primary checks |
|---|---:|---|
| Small mobile | 320–374 px | Menu usability, text wrapping, tap targets, portrait crop, no horizontal overflow |
| Standard mobile | 375–479 px | Hero balance, section padding, publication wrapping, card density |
| Large mobile / small tablet | 480–767 px | Transition from single-column layouts, line length, image scale |
| Tablet | 768–1023 px | Navigation behavior, column balance, gutters, content density |
| Laptop | 1024–1439 px | Full navigation, hero composition, readable maximum line length |
| Desktop | 1440–1919 px | Content width, intentional margins, balanced section rhythm |
| Large desktop | 1920 px and above | Maximum-width constraints, avoidance of oversized empty areas |

## Blank-Space and Spacing Checks

The goal is comfortable separation without making the site feel empty.

- No unrelated elements should appear visually attached.
- Related items should remain grouped more tightly than separate sections.
- Section padding should scale down on mobile and increase moderately on larger screens.
- Paragraph line length should remain readable rather than stretching across wide displays.
- Hero content should remain above the fold on typical laptop and mobile screens where practical.
- Cards and publication entries should not have large empty interiors caused by mismatched heights.
- Large screens must use maximum content widths so added viewport width becomes balanced margins, not stretched content.
- Review vertical gaps between headings, body text, metadata, controls, cards, and adjacent sections.
- Flag both crowding and excessive voids during screenshot review.

## Typography

- Use a **clean sans-serif family throughout** to match the approved reference direction.
- Use weight, size, color, and spacing—not a second typeface—to establish hierarchy.
- Prefer a modern, highly legible sans-serif with strong regular, medium, semibold, and bold weights.
- Keep body copy at a comfortable reading size with approximately `1.6` line height.
- Limit long-form text width to roughly `60–72` characters per line.
- Scale headings fluidly across breakpoints so names and publication titles do not wrap awkwardly.
- Avoid ultra-light weights, condensed faces, all-caps paragraphs, and excessive letter spacing.
- Use Space Indigo or Regal Navy for major headings and Baltic Blue selectively for links and interactive emphasis.

## Shape Language

- Use **subtle rounding** for an academic, polished appearance.
- Cards and buttons should generally use a `6–8px` corner radius.
- The portrait remains circular.
- The large outer site canvas may use a slightly larger radius to retain the approved reference composition.
- Avoid pill-shaped buttons, heavily rounded cards, and playful bubble-like containers.
- Use thin, low-contrast borders and soft shadows; shadows should clarify layering rather than create floating objects.

## Display Mode

- Use **light mode only**.
- Remove the appearance/theme toggle from the header.
- Do not create or maintain a separate dark palette.
- Ensure the light palette remains comfortable in both bright and dim viewing environments.

## Content Density

- Use **balanced density**.
- Keep cards concise while retaining enough spacing for fast scanning.
- Avoid both compressed résumé-style walls of text and oversized showcase sections.
- Use progressive disclosure or detail pages for longer research descriptions rather than expanding every card.

## Navigation

- Use a **sticky header**.
- Provide links to the primary homepage sections and Experience/CV destinations.
- Highlight the active homepage section while scrolling.
- Keep the sticky header compact so it does not consume excessive vertical space on mobile or laptop screens.
- Ensure anchor destinations account for the sticky-header height.

## Motion

- Use very subtle fades and hover transitions.
- Motion should reinforce hierarchy and interaction feedback, not delay reading.
- Keep durations short and easing calm.
- Respect `prefers-reduced-motion`; remove nonessential transitions and scroll effects when reduction is requested.
- Avoid parallax, large entrance animations, bouncing controls, and continuous decorative motion.

## Required QA Before Sign-off

- Visual inspection at every screen class in the responsive matrix.
- Numeric horizontal-overflow checks at every tested viewport.
- Portrait focal-point and crop inspection at every breakpoint.
- Navigation, search, CV link, active-section highlighting, and section-anchor testing.
- Light-mode contrast review across text, controls, cards, tags, borders, and focus states.
- Reduced-motion behavior verification.
- Above-the-fold inspection on mobile, laptop, and desktop.
- Full-page spacing review to identify both crowded clusters and excessive blank regions.

## Final Approval Summary

- Academic and approachable visual tone.
- Reference-inspired, full-width two-column hero.
- Circular portrait with responsive focal-point control.
- Flat parchment background with Honeydew and Baltic-blue accents.
- Clean sans-serif typography throughout.
- Subtle corner rounding.
- Regal Navy headings, Space Indigo body text, and Baltic Blue interactions.
- Light mode only.
- Balanced content density.
- Sticky navigation with active-section highlighting.
- Subtle, reduced-motion-aware transitions.
