# Next Session Handoff

## Current branch

`claude/review-website-docs-w9ZUh` — redundancy + structure pass, Praise merged into About, LinkedIn additions.

---

## What changed this session

### Round 1: Redundancy & structure (already committed)

- **index.html**: hero body + Superpower side-fact no longer echo the Brianna quote; ThingsILove thumbnail mismatch fixed; about-body no longer re-lists the stats strip; iTunes card text de-duped from work.html; 3rd card now points to About.
- **method.html**: 5 questions → 3 moves (Define / Diagnose / Translate); hero sub no longer a TOC; fabricated 85–98% skill percentages dropped.
- **about.html**: hero sub no longer previews the grid below; portrait 6→4 cells (work/method cells relocated); 4-col grid layout; SF cell reframed personal.
- **work.html**: Career Journey rebuilt as "A Through-Line" (caption + CareerRiver + chip timeline Elegrity→eBay→Apple→MS→SFMTA); iTunes step-outcome de-duped.

### Round 2: Praise merge + LinkedIn additions

**Praise → About merge (Option A chosen)**
- Testimonials section added to About as `#praise` (between Teaching vignette and Education).
- Bottom CTA-to-Praise block removed from About.
- Praise link removed from nav on all 4 pages.
- Home's 3rd card re-pointed to About with updated description.
- `redesign/testimonials.html` deleted (merged into About).
- **New: Testimonial "Recurring words" theme row** added above the quotes list — colored chips summarizing the 7 quotes' themes (asks the right questions, translates complexity, humanity, mentors generously, charm & kindness, gets results, incisive mind). Lets visitors scan before reading.

**LinkedIn-derived additions**
- **NEW case study on Work: "Kernel Updates for 500,000 Systems"** — previously only a chip in Method's Duct Tape/Drano panels. Now a full case study with 3 steps + outcome, placed between eBay and the personal projects. Notes 500K systems + 40+ engineering groups.
- **iCloud case study**: added a 3rd step "Harden the backbone" covering the disaster recovery / business continuity work from LinkedIn (strategy, testing, documentation, architecture improvements).
- **SFMTA start date surfaced**: index hero kicker now reads "Principal Business Analyst · SFMTA · Since April 2024" instead of "· San Francisco."
- **Elegrity dates** added to career chip timeline (2006–09) for data completeness.
- **Teaching vignette rewritten** to reflect Saint Mary's 4-year engagement (student → consultant) rather than a brief post-grad stint.

---

## Viz opportunities — image ideas for Nabil to create

Five ideas where Nabil's hand-drawn / illustrative style (per CareerRiver.png) could replace or strengthen text-heavy sections. Descriptions are specific enough to hand to an illustrator or generate externally.

### 1. Education Through-Line (**priority — matches existing visual language**)
Companion piece to `CareerRiver.png`. A meandering path or river representing the learning arc, with 4 milestones as stations along the way:
- **University of Chicago — BA, English Literature** (earliest, dimmer/smaller — "where it all began")
- **George Mason University — MS, Information Systems**
- **UC Berkeley — Data Analytics Certificate (2018–19)**
- **Saint Mary's College — MS, Business Analytics, Honors (2021–22)** — brightest, largest, with a small laurel or honors flourish
Tone: hand-drawn, warm, same palette as CareerRiver (coral / teal / mustard / sage on cream background). Could be horizontal or vertical. Would replace the current `Education.png` section thumbnail with something that *tells the story* rather than decorates it.

### 2. Three Pillars illustration
The About page's "Three Things I Always Bring" has three long text paragraphs from Mary Salome. Hard to scan. A single image would let the eye land first:
A central illustrated motif (could be Nabil's Animal Crossing avatar, or a simple abstract figure) with three radiating elements — a branching diagram, three interlocking shapes, or three "petals" around a center. Each labeled with one keyword:
- **Networked Intelligence** (icon: branching nodes or constellation)
- **Fierce Advocacy** (icon: shield or raised hand)
- **Incorruptible Practicality** (icon: scales balanced, or a sturdy tool)
Use lavender accent (already the section's color). Would go as the section thumbnail replacing `ThreePillars.png`.

### 3. Kernel Updates scale illustration (**biggest impact per pixel**)
For the new "Kernel Updates for 500,000 Systems" case study on Work. The numbers are huge and abstract; an image can make them visceral:
- Left half: **Before** — a scatter of disconnected dots (500K systems), some red/warning-colored, with scattered disconnected clusters (40+ teams), chaotic arrows.
- Right half: **After** — the same dots/clusters, now in tidy orderly flows, a single dashboard-like panel at the top showing status, arrows flowing cleanly.
- Style: grid of tiny dots like a pointillist grid. Could be quite small (300×200px inline) and still readable.
This case study has no step-chain image currently; this would anchor it.

### 4. Testimonial Themes word cloud
The "Recurring words" chip row I added on About is a tame version of this. A hand-drawn / illustrated word cloud could make it feel more personal:
- Largest/boldest: **asks the right questions**, **translates complexity**, **humanity**
- Medium: **mentors generously**, **charm**, **kindness**, **gets results**, **incisive mind**
- Smaller: **eloquent**, **genuine concern**, **relentless passion**, **cannot lie**, **fun to work with**
Could use the site's accent palette and Playfair italics for the big words. Could replace the `Testimonials.png` section thumbnail.

### 5. iTunes "Pagers Going Quiet" before/after mini chart
The iTunes case study has a strong narrative but no visual anchor beyond the emoji. A simple line/bar chart showing pager events dropping week-over-week as the crash-tracking system came online would make the outcome visceral. This one could be a coded SVG rather than an illustration.

---

## In-code viz changes I already made this session

- **Testimonial "Recurring words" chip row** — added above the quotes list on About. Colored chips summarize what the 7 quotes agree on.
- **Career chip timeline** (earlier chunk) — replaced a bare PNG-only Career Journey section.
- **Method diagnostic funnel** (earlier chunk) — simpler 3-move version.
- **Skill bars** (earlier chunk) — removed fake percentages, kept bars as relative indicators.

---

## Still open

- **Browser QA** on all 4 pages (especially About's new 4-col grid + testimonials themes row wrapping on narrow screens).
- **Orphan prototype files** in `redesign/` (15 of them): `books-bubble.html`, `career-excitement.html`, `career-river-3d.html`, `career-river.html`, `dark-arc-timeline.html`, `dual-timeline.html`, `favorite-tools.html`, `game-of-life.html`, `gradient-circles.html`, `impact-scale.html`, `inspiration-donut.html`, `personal-evolution.html`, `portrait-infographic.html`, `skills-radar.html`, `work-quadrant.html`. None linked from live pages. Candidates for deletion.
- **Images**: the 5 descriptions above — Nabil to create externally and drop in.
- **Promote `redesign/` to root**: when ready, replace the root site.

---

## Current page structure (after this session)

| Page | File | Sections |
|------|------|----------|
| Home | `redesign/index.html` | Hero · Stats strip · Brianna pull-quote · "The work, briefly" · Selected work (3 cards → Work, Method, About) |
| Work | `redesign/work.html` | "A Through-Line" (caption + CareerRiver + chip timeline) · 7 case studies (iTunes, iCloud, **Kernel Updates NEW**, eBay, SHAP, Secret Gardens, Conditional Probability) |
| Method | `redesign/method.html` | 3 Moves (Define / Diagnose / Translate) · Duct Tape/Drano · Bell Curve · Skill toolkit |
| About | `redesign/about.html` | Portrait grid (4 cells) · Three Pillars · Teaching vignette (4-year Saint Mary's) · **#praise: What People Say** (recurring-words chips + 7 testimonials) · Education & Certs |

Nav on all 4 pages: Home · Work · Method · About

---

## Technical notes

- All redesign work in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--coral` on Home/Work · `--teal` on Method · `--lavender` on About
- Nav is self-contained within `redesign/`
- Home hero portrait + Work CareerRiver reference `../inspiration_samples/` — not moved
- LinkedIn profile PDF in repo root (`linked_in_profile.pdf`)
