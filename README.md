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
| `work.html` | Career river, 6 projects (eBay + iTunes + Kernel as deep case studies, 3 lighter pieces linking to dedicated note pages) |
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
| `ConstellationPainted.png` | intentionally archived — was the iCloud case study illustration before iTunes replaced that slot |
| `TeachingScene.png` | about.html — "One More Thing" |
| `ThingsILove.png` | index.html — "The work, briefly" section thumbnail |
| `WordClouds Painted.png` | about.html — "What People Say" ✅ |
| `Testimonials.png` | **nobody** — orphaned, safe to delete |
| `EducationWalkPainted.png` | about.html — "Education & Certifications" ✅ |
| `ProfilePicture.jpeg` | about.html + index.html — hero avatar (both now at root path) |
| `QuietedPagersPainted.png` | work.html — iTunes case study illustration ✅ |
| `CleoInspects.png` | footer on all 4 pages — "Inspected by Cleo" ✅ |
| `CareerJourneyPainted.png` | work.html — career journey illustration ✅ |

## Still to do

- **April 30 review (T1–T9)** — see `plan/NEXT_SESSION.md` for the luxury-of-whimsy pass (second feminist-SF round). T1 (home-hero feminist-SF chip) ✅ pushed. T2 (Touchstones chip strip on About) ✅ pushed. T3–T9 are open recommendations — case study rewrite, recurring-words decision, toolkit column move, project-card variety, stats-strip phrasing, optional feminist-SF essay, browser QA. See review for suggested implementation order.
- **April 28 review (S1–S9)** — second whimsy pass. S1 (Off the Clock vignette) ✅, S5 (eBay promoted to case study) ✅, S7 (Duct Tape/Drano notes rewritten) ✅, S8 (favorite questions) ✅, S9 ("Patterns" rename) ✅. S2 (hero kicker), S3 (chip strip tightening), S4 (home echo) still open. S6 (Now strip) declined.
- **All case studies need a full rewrite** — copy has gotten distorted over multiple passes. Rewrite from source material, not by editing what's there. eBay was rewritten this way (S5); iCloud and Kernel still need it. See plan/NEXT_SESSION.md T3 for shape suggestions.
- **Browser QA** on all 4 pages, especially the career/education timelines on mobile, About's 4-col portrait grid, and the testimonials themes row on narrow screens.
- **Recurring-words chip strip on About** — needs a decision: real word cloud, or demote to a one-line caption above the testimonials. (T4)
- **"Translating Complexity" in wrong toolkit column on Patterns** — belongs under Translation & Communication, not Analysis & Insight. (T5)
- **Stats-strip phrasing on home** — "300M+ iCloud users whose outages I tracked" is grammatically tangled. (T7)
- **Selected-work cards on home** — three same-shape cards reads as redundant; consider differentiating. (T6)
- **Feminist-SF essay** as a fourth Notes/Side Quest (optional whimsy). (T8)
- **Touchstones chip strip on About** ✅ — six authors below the Off the Clock vignette: Butler, Le Guin, Delany, Russ, Tiptree, Jemisin. Easy to swap if any don't belong.
- **Feminist-SF chip on home hero** ✅ — `📚 Reads & writes feminist SF`.
- **Testimonial word cloud illustration** ✅ — `WordClouds Painted.png` live on about.html.
- **iCloud illustration** ✅ — `ConstellationPainted.png` wired up on work.html between project lead and tags.
- **Case study images shrunk** ✅ — `KernelCleanupPainted.png` and `ConstellationPainted.png` capped at 420px so they no longer overpower the text.
- **Skill bars on method.html** ✅ — Replaced with color-coded chip pills. See plan/NEXT_SESSION.md for an AC illustration idea for this section.
- **Dedicated note pages** ✅ — `probability.html`, `gardens.html`, `unicorns.html` created in site style. Lighter reads on work.html trimmed to teasers linking to local pages.
- **"Chasing Unicorns for Pride" added** ✅ — new lighter read with teal accent (work.html → unicorns.html).
- **SHAP lighter read removed** ✅ — dropped as outdated.
- **2018–2020 gap on career timeline** ✅ — "Sabbatical · Deliberate pause" node added between Apple and Independent Consulting.
- **"Now" strip on home** ✗ declined — see plan/NEXT_SESSION.md S6 for rationale (ages fast, requires maintenance, Cleo + tea chip already do the vibe-work).
- **Cat cameo** ✅ — "Inspected by Cleo" with photo in footer of all 4 pages.

## Inspiration research

See `plan/Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, icon grids
- **Jennifer Rash** — bold, project-first
