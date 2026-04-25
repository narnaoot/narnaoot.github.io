# narnaoot.github.io — Nabil Arnaoot's Personal Site

A personal portfolio site for Nabil Arnaoot: Principal Business Analyst, Project Leader, translator of complexity. Currently working at SFMTA.

## Emphasis

The site foregrounds **project leadership** — Nabil's ability to walk into ambiguous situations, define problems, build cross-functional processes, and deliver results. Data skills are a supporting capability, not the headline.

## Site structure

### Root (live site)

| File | Purpose |
|------|---------|
| `index.html` | Homepage |
| `about.html` | Personal portrait, three pillars, teaching vignette, testimonials, education & certs |
| `work.html` | Career river, chip timeline, 7 case studies |
| `method.html` | 3 Moves (Define / Diagnose / Translate), Duct Tape/Drano, Bell Curve, skill toolkit |

Nav on all 4 pages: Home · Work · Method · About

### Archive folders

| Folder | Contents |
|--------|---------|
| `old/` | Earlier prototype explorations — ignore |
| `original_version/` | Pre-redesign root files — ignore |

## Design tokens (in every page's `:root`)

| Token | Value | Use |
|-------|-------|-----|
| `--coral` | `#E8614F` | Primary accent, nav logo |
| `--teal` | `#2DB5A8` | Secondary accent |
| `--mustard` | `#D4920A` | Tertiary |
| `--lavender` | `#8B7BC8` | About hero kicker + accents |
| `--sage` | `#6A9F7A` | Soft accent |
| `--bg` | `#FFFBF5` | Page background (warm cream) |
| `--text` | `#3D2B1F` | Body text (dark brown) |

Fonts: **Playfair Display** (headings) + **Nunito** (body)

## Images

Section thumbnails live in the root alongside the HTML files.

| File | Use |
|------|-----|
| `AboutHero.png` | about.html — "The Human Behind the Projects" |
| `ThreePillars.png` | about.html — "Three Things I Always Bring" |
| `TeachingScene.png` | about.html — "One More Thing" |
| `ThingsILove.png` | index.html — "The work, briefly" section thumbnail |
| `Testimonials.png` | about.html — "What People Say" |
| `EducationWalkPainted.png` | about.html — "Education & Certifications" |
| `ProfilePicture.jpeg` | about.html hero avatar (root path); index.html references `inspiration_samples/ProfilePicture.jpeg` — ⚠️ path inconsistency, see NEXT_SESSION.md #5 |
| `CareerJourneyPainted.png` | work.html — career journey illustration |

## Still to do

- **Browser QA** on all 4 pages, especially the career/education timelines on mobile
- **Illustrations still needed** (Nabil to create — see NEXT_SESSION.md for descriptions):
  - Three Pillars illustration (replace `ThreePillars.png`)
  - Kernel Updates before/after dot-grid (for work.html case study)
  - Testimonial word cloud (replace `Testimonials.png`)
  - iTunes "Pagers Going Quiet" line chart (could be coded SVG)
- **Education Through-Line** — `EducationWalkPainted.png` is live ✅; `Education.png` is now orphaned and can be deleted
- **Copy & content edits** — see "Copy & content suggestions" section in NEXT_SESSION.md for full list

## Inspiration research

See `Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, icon grids
- **Jennifer Rash** — bold, project-first
