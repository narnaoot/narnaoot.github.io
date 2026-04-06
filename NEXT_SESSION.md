# Next Session Handoff

## Visual direction: Animal Crossing theme

The redesign has committed to an **Animal Crossing visual theme**. The hero and career journey both now use illustrated AC-style images of Nabil. All source images are in `inspiration_samples/`.

| Image | Where used |
|-------|-----------|
| `inspiration_samples/ProfilePicture.jpeg` | `redesign/index.html` hero — full-body AC character portrait, two-column layout |
| `inspiration_samples/CareerRiver.png` | `redesign/career-river.html` — Nabil in inner tube floating past 4 career sign posts |

## What's done

- `Inspiration.md` fully documented with file references, 5 designers + Stephen's Game of Life analyzed
- Root site pages updated: index, about, work, method — all reframed from "data storyteller" to **Project Leader**
- `redesign/` folder built with AC visual theme applied to hero + career journey
- Branch: `claude/update-redesign-direction-RQr7R`

### Root page changes (session 2)

- **index.html**: title/tagline → "Project Leader"; about lead/body copy reframed around PM clarity
- **about.html**: section headers updated; English Lit note reframed; 9 new PM-focused testimonials added (Wanda Davis, Faron Lyons, Karina Sanz, Salathiel Bluitt, Brianna Gamp, Cliff Winnig, Séain Gutridge, Tom, Laura)
- **work.html**: iTunes project reframed as PM story; SHAP project reframed toward stakeholder translation; career chain caption updated
- **method.html**: skill columns reordered — "Project & Program Leadership" leads; "Data & Analysis" → "Analysis & Insight"; "Data Storytelling" → "Translating Complexity"

### redesign/ folder (session 3)

- **redesign/index.html**: Stefanie Kraus-inspired homepage — warmer hero, stats strip kept, Brianna Gamp as featured pull quote, 3 project cards, single CTA footer
- **redesign/career-river.html**: Shows `CareerRiver.png` — Nabil floating past 4 wooden career signs (eBay 2006-2011, Apple 2011-2020, St. Mary's 2020-2024, SFMTA 2024-Now)

### redesign/index.html hero (session 6 — AC theme)

- Replaced 80px avatar circle with full `ProfilePicture.jpeg` in a two-column grid layout
- Hero background updated to soft green gradient (`#e0f0d8 → --bg`) to evoke AC nature theme
- `.hero-portrait` image is 260px wide on desktop, stacks on mobile (max-width 200px centered)

### redesign/about.html (session 4 — branch: claude/fix-about-page-timeout-PmOOO)

Built incrementally (7 commits) to avoid timeouts. Sections in order:

1. **Hero** — lavender kicker, "About Nabil" heading, short sub
2. **Personal Portrait** — 6-item grid: cats (Octavia & Cleopatra), tea, English Lit, 0→1 problems, career through-line, SFMTA
3. **Three Pillars** — Mary Salome's exact words: Networked Intelligence / Fierce Advocacy / Incorruptible Practicality
4. **Teaching Vignette** — Saint Mary's cohort story, anchored by Ipsita's quote
5. **Things I Love** — 10-item Nina Voordes-style icon grid
6. **Bell Curve SVG** — "My Professional Sweet Spot" (Catherine Madden-inspired; X=creative freedom, Y=job satisfaction; peak = Trust/Vision/Leadership)
7. **Testimonials** — all 15, Brianna Gamp featured first
8. **Education & Certifications**

---

## All inspiration files (quick reference)

Full notes on each are in `Inspiration.md`. Every file is in `inspiration_samples/`.

| File | Designer | What it is |
|------|----------|------------|
| `Resume+-+13.webp` | Catherine Madden | Career excitement bubble chart — X=time, Y=excitement, bubbles=skills/focus areas |
| `Resume+-+12.webp` | Catherine Madden | Bell curve — X=creative freedom, Y=job satisfaction; peak = trust/vision/leadership |
| `Resume+-+11.webp` | Catherine Madden | 2×2 quadrant on dark bg — business vs pleasure × solo vs group |
| `Resume+-+8.webp` | Catherine Madden | Life stages stacked bar / stream chart — age 0–30 |
| `Resume+-+14.webp` | Catherine Madden | "My Favorite Tools" — stacked bar by age |
| `Emy1.webp` | Catherine Madden | Radial/donut "Inspiration" chart |
| `Emy3.webp` | Catherine Madden | "Books I've Heard Lately" bubble chart |
| `Nina1.webp` | Unknown (Tableau blog) | Dual-track horizontal timeline |
| `image4_0.png` | Nina Voordes | Full portrait infographic — dot matrix skills, hex tools, "Things I ♥" icon grid |
| `Stephen's Game of Life.png` | Stephen (Tableau blog) | Career as a Game of Life board |
| `JRashVisualResume___.jpg` | Jennifer Rash | 3×3 grid of color-coded circles on black |
| `CV  Resume.png` | Samuel Parsons | Dark charcoal, landscape — radial arc timeline |
| `website/inspo1.pdf` | Stefanie Kraus | Portfolio homepage |
| `website/inspo2.pdf` | Stefanie Kraus | "My Process" page |
| `website/inspo3.pdf` | Stefanie Kraus | Full about page |

---

## Session 5: 14 Visualization Files Built (redesign/)

All 14 HTML visualization files are now committed to `redesign/`. Each is self-contained (CSS inline, SVG inline, no external files).

| File | Description | Placeholder data? |
|------|-------------|-------------------|
| `redesign/career-river.html` | Animal Crossing–style SVG river with 6 illustrated career stops, landmarks, hills, clouds | No |
| `redesign/career-excitement.html` | Bubble chart: X=time, Y=excitement, bubbles=skill focus areas. Hand-drawn feel. | ★ Excitement levels (1–10) need Nabil's confirmation |
| `redesign/dual-timeline.html` | Horizontal timeline 2006→2025. Career roles below center, personal threads above as arcs | No |
| `redesign/work-quadrant.html` | Dark charcoal 2×2 quadrant: creative freedom vs social intensity. Energizes vs drains. | No |
| `redesign/personal-evolution.html` | Stacked bar chart with Sankey-style ribbons. Energy distribution by career era. | Proportions are approximate |
| `redesign/favorite-tools.html` | Stacked bar chart of tools used per era (Sheets → SQL/Python/Tableau). Primary vehicle row. | No |
| `redesign/books-bubble.html` | Scatter plot: X=fact↔fiction, Y=put down↔obsessed. Bubble size=page count. 12 books. | ★ All 12 book titles are placeholder — Nabil to confirm his actual reading list |
| `redesign/inspiration-donut.html` | Radial donut with 10 segments (Cities, Transit, Lit, Cats, etc.). NA monogram center. | No |
| `redesign/game-of-life.html` | Board game path of career milestones. "You Are Here" at SFMTA. Illustrated SVG. | No |
| `redesign/gradient-circles.html` | Dark background. 6 gradient circles (one per role), sized by years. Hard+soft skills list. | No |
| `redesign/dark-arc-timeline.html` | Dark charcoal. Arc spans above horizontal timeline. Core Values strip. 3 impact stats. | No |
| `redesign/portrait-infographic.html` | Tall single-column: header, dot matrix skills, hex tool grid, timeline strip, services, loves. | No |
| `redesign/impact-scale.html` | Concentric circle waves showing scale of reach per role. Logarithmic. Dramatic dark bg. | No |
| `redesign/skills-radar.html` | 8-axis radar chart. Entry 2006 (muted) vs Now 2025 (coral). CSS fade-in animation. Written key. | No |

### Items still needing Nabil's input
1. **Excitement levels** in `career-excitement.html` — current values are estimates (Elegrity:6, eBay:7, Apple EPM:9, Apple Process:7, St.Mary's:8, SFMTA:8)
2. **Book titles** in `books-bubble.html` — 12 suggested books; Nabil to confirm actual reading list

---

## Still open / future sessions

1. **Career excitement chart** (Catherine Madden style) — needs Nabil's excitement levels per role:
   - Elegrity (2006–2010)
   - eBay (2010–2011)
   - Apple Eng PM (2011–2014)
   - Apple Process Eng (2014–2020)
   - St. Mary's / consulting (2020–2024)
   - SFMTA (2024–now)

2. **Books bubble chart** — which books to include? (for a Catherine Madden Emy3-style chart)

3. **Promotion of redesign/ to root** — once Nabil approves the redesign files, swap them in as the live pages

---

## Technical notes

- All redesign work lives in `redesign/` — root files untouched
- Same CSS tokens and fonts as root pages
- Push to `claude/update-redesign-direction-RQr7R` (current branch)
- **Timeout strategy**: build large pages section-by-section with a commit after each chunk — never write a full page in one shot
