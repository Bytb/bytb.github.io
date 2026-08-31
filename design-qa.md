# Design QA

## Comparison

- Reference: `C:/Users/Caleb/AppData/Local/Temp/codex-clipboard-6acf2601-9504-4e22-b376-77aa051bfa97.png`
- Implementation: `.codex-tools/desktop-final.png`
- Side-by-side comparison: `.codex-tools/reference-vs-implementation.png`
- Comparison viewport: 1440 × 900 px

The implementation preserves the reference's compact sticky navigation, two-column identity/summary composition, circular portrait, strong name hierarchy, summary and CV action, and three-card education row. Following the final review, the reference's exterior gradient and contained canvas were removed in favor of a full-width parchment page.

## Findings and Resolutions

### P0 — Blocking

- None found.

### P1 — High priority

- None remaining.

### P2 — Medium priority

- Resolved: the initial identity column was vertically centered against all right-column content and placed the portrait too low. Both columns now begin on the same visual baseline.
- Resolved: the initial hero used excessive vertical space. Hero padding, section margins, education-card padding, and grid gaps were tightened.
- Resolved: five social controls wrapped to two rows at 375 px. Mobile control size and gaps were adjusted so they remain on one row.
- Resolved: social icon links inherited icon names as accessible names. Explicit Email, GitHub, LinkedIn, Google Scholar, and ORCID labels are now applied.
- Resolved: the page wrapper clipped scrolling in the in-app preview. The wrapper now uses normal visible overflow and vertical scrolling was verified programmatically.
- Resolved: stacked template padding created excessive space below the navbar. The hero now begins 60 px below the desktop navbar content baseline.
- Resolved: the portrait subject appeared left of center. The image is slightly enlarged and shifted within its circular crop.
- Resolved: the gradient and rounded outer canvas were removed; the parchment surface now fills the viewport.

## Responsive Matrix

| Viewport | Navigation | Columns | Horizontal overflow | Result |
|---|---|---|---:|---|
| 320 × 780 | Mobile toggle | Single | 0 px | Passed |
| 375 × 812 | Mobile toggle | Single | 0 px | Passed |
| 480 × 900 | Mobile toggle | Single | 0 px | Passed |
| 768 × 1024 | Mobile toggle | Two | 0 px | Passed |
| 1024 × 900 | Full navigation | Two | 0 px | Passed |
| 1440 × 900 | Full navigation, full-width page | Two | 0 px | Passed |
| 1920 × 1080 | Full navigation, full-width page | Two | 0 px | Passed |

## Interaction and Accessibility Checks

- Mobile navigation opens and closes successfully.
- Sticky navigation remains compact and section links target valid anchors.
- Active-section styling is visible and exposes `aria-current`.
- Search remains available on desktop and mobile.
- CV link targets the existing résumé PDF.
- Social links expose meaningful accessible labels.
- Focus-visible styling is present for keyboard navigation.
- Motion is subtle and disabled under `prefers-reduced-motion`.
- Light mode is fixed; the theme toggle is removed.
- Portrait remains circular and centered at desktop, tablet, and mobile sizes.
- Research navigation scrolls to its section and updates the active navigation state.

## Build Check

- Hugo production build completed successfully: 52 pages, 11 processed images, and no content errors.
- Local Windows preview uses Hugo 0.160 because Hugo 0.161+ introduced a Windows-specific Node CLI detection issue; the repository's standard Linux GitHub Pages workflow remains unchanged.

final result: passed
