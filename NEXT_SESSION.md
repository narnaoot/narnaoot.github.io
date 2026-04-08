# Next Session Handoff

## Current branch

`claude/review-project-status-Ru30x`

---

## What's done (as of this session)

### Root pages (all complete)
- `index.html`, `about.html`, `work.html`, `method.html` — all reframed from "data storyteller" to **Project Leader** narrative

### redesign/ — fully built, linked site

All pages exist and nav links are self-contained within `redesign/`:

| Page | File | Status |
|------|------|--------|
| Home | `redesign/index.html` | Done — AC hero portrait, stats strip, 3 project cards |
| Work | `redesign/work.html` | Done — CareerRiver banner, career chain SVG, river CTA, 4 case studies |
| Method | `redesign/method.html` | Done — 6 diagnostic questions, Duct Tape/Drano, animated skill bars |
| About | `redesign/about.html` | Done — 8 sections, all 6 AC banners wired in |
| Career River | `redesign/career-river.html` | Done — AC river illustration, 4 career stops |

### redesign/about.html — all 6 section banners

All images are in `inspiration_samples/`. Banner height is 380px.

| Section | Image file | Notes |
|---------|-----------|-------|
| The Human Behind the Projects | `AboutHero.png` | Original (not composition-locked) — may crop awkwardly |
| Three Things I Always Bring | `ThreePillars5.png` | Cherry blossom season, no cat, composition-locked |
| One More Thing | `TeachingScene2.png` | Outdoor classroom, composition-locked |
| Things I Love | `ThingsILove3.png` | Black cat, flat-lay, composition-locked |
| What People Say | `Testimonials2.png` | Bulletin boards, no soccer ball |
| Education & Certifications | `Education3.png` | Books/owl/scrolls, composition-locked |

### Copilot image prompt formula (composition-locked)

Use this structure for any future banner generates:

```
Animal Crossing New Horizons style 3D render, ultra-wide panoramic banner, no characters.

ABSOLUTE BANNER CONSTRAINT:
– The top 45% of the image contains ONLY sky and distant treetops.
– No vertical objects, posts, boards, signs, or upright symbols exist anywhere in the scene.
– All objects lie flat on the grass or sit no higher than a teacup.
– All meaningful items are tightly clustered in the lower-center foreground.

SCENE: [describe items lying flat on grass]

BACKGROUND: Only grass fading into distant trees and open sky. No focal elements.

LIGHTING & STYLE: [lighting], vibrant saturated colors, chunky rounded cartoon proportions.
```

### 14 data visualization pages (redesign/)

All self-contained (inline CSS + SVG), no external dependencies.

| File | Description | Needs input? |
|------|-------------|-------------|
| `career-river.html` | AC-style river with career stops | No |
| `career-excitement.html` | Bubble chart: excitement per role over time | ★ Excitement levels (1–10) needed |
| `dual-timeline.html` | Horizontal timeline 2006→2025 | No |
| `work-quadrant.html` | 2×2 quadrant: creative freedom vs social intensity | No |
| `personal-evolution.html` | Stacked bar: energy by career era | Proportions approximate |
| `favorite-tools.html` | Stacked bar: tools used per era | No |
| `books-bubble.html` | Scatter: fact↔fiction vs put-down↔obsessed | ★ Book list needed |
| `inspiration-donut.html` | Radial donut: 10 inspiration segments | No |
| `game-of-life.html` | Board game path of career milestones | No |
| `gradient-circles.html` | 6 gradient circles sized by years | No |
| `dark-arc-timeline.html` | Dark charcoal arc timeline | No |
| `portrait-infographic.html` | Tall single-column infographic | No |
| `impact-scale.html` | Concentric circles: reach per role | No |
| `skills-radar.html` | 8-axis radar: 2006 vs now | No |

---

## Still open

### Needs Nabil's input
1. **Career excitement levels** (1–10) for `career-excitement.html`:
   - Elegrity (2006–2010)
   - eBay (2010–2011)
   - Apple Eng PM (2011–2014)
   - Apple Process Eng (2014–2020)
   - St. Mary's / consulting (2020–2024)
   - SFMTA (2024–now)

2. **Book list** for `books-bubble.html` — 12 books Nabil has actually read

### Optional image regeneration
- `AboutHero.png` — the only banner not generated with the composition-lock prompt. If the crop still looks off, regenerate using the formula above with this scene: "a sleek black cat curled up on the grass, a steaming teacup on a saucer, an open book, small seedling plants nearby"

### Big decision
3. **Promote redesign/ to root** — when Nabil approves the redesign, swap those files in as the live site. Steps:
   - Copy each `redesign/*.html` to root, updating all relative paths (remove `../` from image refs, update nav hrefs)
   - Or configure GitHub Pages to serve from a subfolder/branch

---

## Inspiration files reference

Full notes in `Inspiration.md`. All files in `inspiration_samples/`.

| File | Designer | What it is |
|------|----------|------------|
| `Resume+-+13.webp` | Catherine Madden | Career excitement bubble chart |
| `Resume+-+12.webp` | Catherine Madden | Bell curve — creative freedom vs job satisfaction |
| `Resume+-+11.webp` | Catherine Madden | 2×2 quadrant |
| `Resume+-+8.webp` | Catherine Madden | Life stages stacked bar |
| `Resume+-+14.webp` | Catherine Madden | "My Favorite Tools" stacked bar |
| `Emy1.webp` | Catherine Madden | Radial/donut "Inspiration" chart |
| `Emy3.webp` | Catherine Madden | "Books I've Heard Lately" bubble chart |
| `Nina1.webp` | Unknown (Tableau blog) | Dual-track horizontal timeline |
| `image4_0.png` | Nina Voordes | Portrait infographic — dot matrix, hex tools, icon grid |
| `Stephen's Game of Life.png` | Stephen (Tableau blog) | Career as Game of Life board |
| `JRashVisualResume___.jpg` | Jennifer Rash | 3×3 grid of color-coded circles |
| `CV  Resume.png` | Samuel Parsons | Dark charcoal radial arc timeline |
| `website/inspo1.pdf` | Stefanie Kraus | Portfolio homepage |
| `website/inspo2.pdf` | Stefanie Kraus | "My Process" page |
| `website/inspo3.pdf` | Stefanie Kraus | Full about page |

---

## Technical notes

- All redesign work lives in `redesign/` — root files untouched
- Same CSS tokens and fonts across all pages
- Nav is fully self-contained within `redesign/` — no `../` links remain
- Image paths from redesign pages use `../inspiration_samples/`
- **Timeout strategy**: build large pages section-by-section with a commit after each chunk
