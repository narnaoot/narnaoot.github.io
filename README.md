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
| `work.html` | Career river, 6 projects (iCloud + Kernel as deep case studies, 4 lighter pieces) |
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
| `ThreePillarsPainted.png` | about.html — "Three Things I Always Bring" ✅ |
| `KernelCleanupPainted.png` | work.html — Kernel Updates case study illustration ✅ |
| `ConstellationPainted.png` | work.html — iCloud case study illustration ✅ |
| `TeachingScene.png` | about.html — "One More Thing" |
| `ThingsILove.png` | index.html — "The work, briefly" section thumbnail |
| `WordClouds Painted.png` | about.html — "What People Say" ✅ |
| `Testimonials.png` | **nobody** — orphaned, safe to delete |
| `EducationWalkPainted.png` | about.html — "Education & Certifications" ✅ |
| `ProfilePicture.jpeg` | about.html + index.html — hero avatar (both now at root path) |
| `QuietedPagersPainted.png` | intentionally archived — not referenced in any live page |
| `CleoInspects.png` | footer on all 4 pages — "Inspected by Cleo" ✅ |
| `CareerJourneyPainted.png` | work.html — career journey illustration ✅ |

## Still to do

- **Browser QA** on all 4 pages, especially the career/education timelines on mobile
- **Testimonial word cloud** ✅ — `WordClouds Painted.png` live on about.html.
- **iCloud illustration** ✅ — `ConstellationPainted.png` wired up on work.html between project lead and tags.
- **Case study images shrunk** ✅ — `KernelCleanupPainted.png` and `ConstellationPainted.png` capped at 420px so they no longer overpower the text.
- **All case studies need a full rewrite** — copy has gotten distorted over multiple passes. Rewrite from source material, not by editing what's there. See NEXT_SESSION.md for details.
- **Skill bars on method.html** ✅ — Replaced with color-coded chip pills. See NEXT_SESSION.md for an AC illustration idea for this section.
- **Links for lighter reads on work.html** ✅ — Secret Gardens (`/work/gardens`), Conditional Probability (`/work/probability`), and Chasing Unicorns (`/work/unicorns`) all linked. SHAP dropped (felt outdated).
- **"Chasing Unicorns for Pride" added** ✅ — new lighter read with teal accent (work.html). Links to `https://n4bil.com/work/unicorns`.
- **SHAP lighter read removed** ✅ — dropped as outdated.
- **2018–2020 gap on career timeline** ✅ — "Sabbatical · Deliberate pause" node added between Apple and Independent Consulting.
- **"Now" strip on home** (optional) — what's on the workbench at SFMTA, what you're reading, current tea. Reinforces "not job-hunting, just available for conversation."
- **Cat cameo** ✅ — "Inspected by Cleo" with photo in footer of all 4 pages.

## Inspiration research

See `Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, icon grids
- **Jennifer Rash** — bold, project-first
