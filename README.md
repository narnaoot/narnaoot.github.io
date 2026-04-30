# narnaoot.github.io — Nabil Arnaoot's Personal Site

A personal portfolio site for Nabil Arnaoot: Principal Business Analyst, Project Leader, translator of complexity. Currently working at SFMTA.

## Emphasis

The site foregrounds **project leadership** — Nabil's ability to walk into ambiguous situations, define problems, build cross-functional processes, and deliver results. Data skills are a supporting capability, not the headline.

## Site structure

### Root (live site)

| File | Purpose |
|------|---------|
| `index.html` | Homepage |
| `about.html` | Personal portrait, three pillars, teaching vignette, off-the-clock (feminist SF), testimonials, education & certs |
| `work.html` | Career river, 6 projects (eBay + iCloud + Kernel as deep case studies, 3 lighter pieces linking to dedicated note pages) |
| `probability.html` | Conditional Probability for Normal Humans — full essay with tables |
| `gardens.html` | Secret Gardens of San Francisco — Tableau Public viz embed |
| `unicorns.html` | Chasing Unicorns for Pride — Tableau Public viz embed |
| `method.html` | "Some Patterns" — favorite questions (incl. "What are you reading?"), Duct Tape/Drano, bell-curve sweet spot, skill toolkit. (File still named `method.html`; visible label is "Patterns.") |

Nav on all 4 pages: Home · Work · Patterns · About

### Archive folders

| Folder | Contents |
|--------|---------|
| `original_version/` | Pre-redesign root files — ignore |
| `plan/` | Working notes — `NEXT_SESSION.md` (review log), `Inspiration.md` (research) |

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

- **April 28 review (S1–S6)** — see `plan/NEXT_SESSION.md` for the second whimsy pass. S1 (Off the Clock vignette) ✅ landed. S2 (hero kicker), S3 (chip strip), S4 (home echo) in progress this session. S5 (eBay miscategorized) deferred. S6 (Now strip) declined.
- **Browser QA** on all 4 pages, especially the career/education timelines on mobile
- **Testimonial word cloud** ✅ — `WordClouds Painted.png` live on about.html.
- **iCloud illustration** ✅ — `ConstellationPainted.png` wired up on work.html between project lead and tags.
- **Case study images shrunk** ✅ — `KernelCleanupPainted.png` and `ConstellationPainted.png` capped at 420px so they no longer overpower the text.
- **All case studies need a full rewrite** — copy has gotten distorted over multiple passes. Rewrite from source material, not by editing what's there. See plan/NEXT_SESSION.md for details.
- **Skill bars on method.html** ✅ — Replaced with color-coded chip pills. See plan/NEXT_SESSION.md for an AC illustration idea for this section.
- **Dedicated note pages** ✅ — `probability.html`, `gardens.html`, `unicorns.html` created in site style. Lighter reads on work.html trimmed to teasers (emoji + title link + 2-line lead + CTA), linking to local pages.
- **"Chasing Unicorns for Pride" added** ✅ — new lighter read with teal accent (work.html → unicorns.html).
- **SHAP lighter read removed** ✅ — dropped as outdated.
- **2018–2020 gap on career timeline** ✅ — "Sabbatical · Deliberate pause" node added between Apple and Independent Consulting.
- **"Now" strip on home** (optional) — what's on the workbench at SFMTA, what you're reading, current tea. Reinforces "not job-hunting, just available for conversation."
- **Cat cameo** ✅ — "Inspected by Cleo" with photo in footer of all 4 pages.

## Inspiration research

See `plan/Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, icon grids
- **Jennifer Rash** — bold, project-first
