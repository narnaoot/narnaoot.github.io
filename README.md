# narnaoot.github.io — Nabil Arnaoot's Personal Site

A personal portfolio site for Nabil Arnaoot: Principal Business Analyst, Project Leader, translator of complexity. Currently working at SFMTA.

## Emphasis

The site foregrounds **project leadership** — Nabil's ability to walk into ambiguous situations, define problems, build cross-functional processes, and deliver results. The "bringing clarity" theme is central, but framed around PM work rather than data storytelling. Data skills remain present as a supporting capability (third skill column on method.html).

## Site structure

### Root (live site)

| File | Purpose |
|------|---------|
| `index.html` | Homepage — hero, project cards, featured quote |
| `about.html` | Personal portrait, testimonials (PM-focused), education |
| `work.html` | Project case studies |
| `method.html` | How Nabil works |

### redesign/ (in-progress — do not overwrite root files)

| File | Purpose |
|------|---------|
| `redesign/index.html` | AC-themed homepage — portrait hero, stats, 3 project cards |
| `redesign/work.html` | Career River banner + CTA, career chain SVG, 4 case studies |
| `redesign/method.html` | 6 diagnostic questions, Duct Tape/Drano, animated skill bars |
| `redesign/about.html` | 8-section page with all 6 AC section banners |
| `redesign/career-river.html` | AC river illustration — 4 career stops |
| `redesign/career-excitement.html` | Bubble chart: excitement per role |
| `redesign/dual-timeline.html` | Horizontal dual-track timeline |
| `redesign/work-quadrant.html` | 2×2 quadrant: creative freedom vs social intensity |
| `redesign/personal-evolution.html` | Stacked bar: energy by career era |
| `redesign/favorite-tools.html` | Stacked bar: tools used per era |
| `redesign/books-bubble.html` | Scatter: books by genre vs engagement |
| `redesign/inspiration-donut.html` | Radial donut: inspiration segments |
| `redesign/game-of-life.html` | Board game path of career milestones |
| `redesign/gradient-circles.html` | Circles sized by years per role |
| `redesign/dark-arc-timeline.html` | Dark charcoal arc timeline |
| `redesign/portrait-infographic.html` | Tall single-column infographic |
| `redesign/impact-scale.html` | Concentric circles: reach per role |
| `redesign/skills-radar.html` | 8-axis radar: 2006 vs now |

## Design tokens (in every page's `:root`)

| Token | Value | Use |
|-------|-------|-----|
| `--coral` | `#E8614F` | Primary accent, nav logo |
| `--teal` | `#2DB5A8` | Secondary accent |
| `--mustard` | `#D4920A` | Tertiary |
| `--lavender` | `#8B7BC8` | Headings / kickers |
| `--sage` | `#6A9F7A` | Soft accent |
| `--bg` | `#FFFBF5` | Page background (warm cream) |
| `--text` | `#3D2B1F` | Body text (dark brown) |

Fonts: **Playfair Display** (headings, serif) + **Nunito** (body, sans)

## Visual theme

The redesign uses an **Animal Crossing** visual theme — illustrated character portrait, section banner images, and an AC-style career river. All AC imagery lives in `inspiration_samples/`.

### Key images

| File | Use |
|------|-----|
| `inspiration_samples/ProfilePicture.jpeg` | Hero portrait — full-body AC character illustration of Nabil |
| `inspiration_samples/CareerRiver.png` | Career River page + work.html banner |
| `inspiration_samples/AboutHero.png` | about.html — "The Human Behind the Projects" banner |
| `inspiration_samples/ThreePillars5.png` | about.html — "Three Things I Always Bring" banner (cherry blossom) |
| `inspiration_samples/TeachingScene2.png` | about.html — "One More Thing" banner |
| `inspiration_samples/ThingsILove3.png` | about.html — "Things I Love" banner (black cat) |
| `inspiration_samples/Testimonials2.png` | about.html — "What People Say" banner |
| `inspiration_samples/Education3.png` | about.html — "Education & Certifications" banner |

## Inspiration research

See `Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression (bell curves, book lists, career charts)
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, "Things I Love" icon grid
- **Jennifer Rash** — bold, confident, project-first

Inspiration files: `inspiration_samples/` folder (screenshots + PDFs)

## Branch

Active development: `claude/review-project-status-Ru30x`
