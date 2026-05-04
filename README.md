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
| `patterns.html` | "Some Patterns" — favorite questions (incl. "What are you reading?"), Duct Tape/Drano, bell-curve sweet spot, skill toolkit. (Renamed from `method.html` on 2026-05-04.) |

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

Section thumbnails live in the root alongside the HTML files. As of 2026-05-04 the live painted assets are WebP at ~900px wide (1100px for the career illustration), down from 31.5 MB of source PNG/JPEG to ~0.9 MB total. The original PNG/JPEG sources were removed from the working tree but remain in git history.

| File | Use |
|------|-----|
| `AboutHero.webp` | about.html — "The Human Behind the Projects" |
| `ThreePillarsPainted.webp` | about.html — "Three Things I Always Bring" |
| `KernelCleanupPainted.webp` | work.html — Kernel Updates case study illustration |
| `TeachingScene.webp` | about.html — "One More Thing" |
| `WordCloudsPainted.webp` | about.html — "What People Say" (was `WordClouds Painted.png`; space removed in the rename) |
| `EducationWalkPainted.webp` | about.html — "Education & Certifications" |
| `ProfilePicture.webp` | about.html + index.html — hero avatar |
| `QuietedPagersPainted.webp` | work.html — iTunes case study illustration; also the work-teaser thumbnail on index.html |
| `CleoInspects.webp` | footer on all pages — "Inspected by Cleo" |
| `CareerJourneyPainted.webp` | work.html — career journey illustration |
| `LighthousePainted.webp` | work.html — eBay Site Security case study illustration (lighthouse before/after with peer-lighthouse beams crossing) |
| `ConstellationPainted.png` | intentionally archived (still PNG, not in HTML) — was the iCloud case study illustration before iTunes replaced that slot |
| `Testimonials.png` | orphaned PNG, safe to delete |
| `ThingsILove.png` | orphaned PNG (former index thumbnail, superseded by the QuietedPagers teaser strip), safe to delete |
| `lighthouse.png` | runner-up draft from the eBay illustration round, safe to delete |
| `avatar.png`, `ac-river-scene.png` | unreferenced legacy assets (already small) |

## Still to do

- **eBay illustration** ✅ — `LighthousePainted.png` live on work.html eBay case study, between project-lead and project-tags, capped at 420px to match iTunes/Kernel pattern. Lighthouse before/after metaphor: dark lighthouse + boats in fog → lit lighthouse with beam, second peer-lighthouse on distant headland with beams crossing in the middle (= cross-company conversation with PayPal). Replaced the earlier "Map for the Maze" noticeboard concept after a single-object metaphor was found to read more cleanly. Two drafts were generated; `lighthouse2.png` won on character canonicality (chosen + renamed `LighthousePainted.png`); `lighthouse.png` runner-up is safe to delete from the repo root.
- **May 1 review (R1–R5)** — see `plan/NEXT_SESSION.md`. R1 (home Selected Work → teaser strip + 2 cards) ✅, R2 (Tiptree nomination replaces Apple-engineers stat) ✅, R3 (About hero sub ends on personal beat) ✅, R4 (Saint Mary's honors-dot styling dropped) ✅, R5 (Patterns toolkit subtitles promoted to titles) ✅. Tiptree mention also added to About > Off the Clock vignette. Still open: eBay illustration, T8 (optional feminist-SF essay), T9 (browser QA).
- **April 30 review (T1–T9)** — see `plan/NEXT_SESSION.md`. T1 (home-hero feminist-SF chip) ✅, T2 (Touchstones chip strip on About) ✅, T3 (case-study rewrites — Kernel ✅, iTunes ✅ replacing iCloud, eBay was already done in S5) ✅, T4 (recurring-words chip strip killed) ✅, T5 (Translating Complexity moved to Communication column) ✅, T6 (project-card variety) ✅ resolved by R1, T7 (stats-strip phrasing) ✅ resolved by R2 + the iCloud→iTunes fix.
- **April 28 review (S1–S9)** — second whimsy pass. S1 (Off the Clock vignette) ✅, S5 (eBay promoted to case study) ✅, S7 (Duct Tape/Drano notes rewritten) ✅, S8 (favorite questions) ✅, S9 ("Patterns" rename) ✅. S2 (hero kicker), S3 (chip strip tightening — superseded by T4), S4 (home echo) still open. S6 (Now strip) declined.
- **iTunes case study replaces iCloud** ✅ — work.html slot rewritten from source as "Making iTunes' Crashes Countable." Illustration swapped: `ConstellationPainted.png` archived, `QuietedPagersPainted.png` restored to live use. Emoji ☁️ → 🎵.
- **Kernel case study rewritten** ✅ — work.html "Kernel Updates for 500,000 Systems" rewritten from source per T3 shape (moment → real problem → moves → outcome). Three concurrent threads: surface what tickets buried, automate the work, renegotiate the bar with infosec.
- **eBay case study** ✅ — already rewritten from source in S5.
- **Recurring-words chip strip on About** ✅ — removed (T4). Testimonials lead the section directly.
- **"Translating Complexity" toolkit column** ✅ — moved from Analysis & Insight to Translation & Communication on Patterns (T5). Now leads the Communication column.
- **About-page section thumbnail alignment** ✅ — fixed the orphaned-heading gap in the five `.section-intro` rows. `align-items: flex-start` → `center`, thumbnail width 220px → 180px.
- **Stats-strip on home** ✅ — orphaned iCloud reference repaired (now `iTunes users behind the dashboards`); 4th stat reframed as `1 Tiptree Award nominee · feminist SF` (R2 + Tiptree request).
- **Selected-work cards on home** ✅ — restructured as one full-bleed teaser strip (with `QuietedPagersPainted.png`) leading into two smaller cards for Patterns + About. The asymmetry gives the eye somewhere to land. (R1, resolves T6.)
- **Feminist-SF essay** as a fourth Notes/Side Quest (optional whimsy). (T8)
- **Browser QA** on all 4 pages, especially the career/education timelines on mobile, About's 4-col portrait grid, and the new About thumbnail alignment after the section-intro change. (T9)
- **Touchstones chip strip on About** ✅ — six authors below the Off the Clock vignette: Butler, Le Guin, Delany, Russ, Tiptree, Jemisin. Easy to swap if any don't belong.
- **Feminist-SF chip on home hero** ✅ — `📚 Reads & writes feminist SF`.
- **Testimonial word cloud illustration** ✅ — `WordClouds Painted.png` live on about.html.
- **Case study images shrunk** ✅ — `KernelCleanupPainted.png` and case-study illustrations capped at 420px so they no longer overpower the text.
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
