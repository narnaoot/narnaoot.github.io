# Next Session Handoff

## Current branch

`claude/update-website-markdown-LfNXM` — comprehensive copy, consistency, and tone pass across all 4 pages.

---

## What changed this session (full suggestions audit)

All changes implement the recommendations from the April 2026 suggestions review.

### index.html
- **Hero image path fixed**: was `inspiration_samples/ProfilePicture.jpeg`, now `ProfilePicture.jpeg` (root). Matches about.html.
- **Stats strip**: replaced "40+ Apple engineering teams" (4th stat) with "4 yrs · Teaching & consulting · Saint Mary's" — breaks up the Apple-heavy strip.
- **Pull quote trimmed**: Brianna Gamp quote shortened. Removed "quickly grasp the key milestones and action items" clause. Punchier.
- **"Six stories" fixed**: pcard description now reads "Seven projects, three told in depth." (was "Six stories, told in steps." — wrong count and overpromised).
- **Honors label removed**: side-fact now reads "MS Business Analytics · Saint Mary's · UChicago BA, English Lit" (no longer says "(Honors)").
- **Footer unified**: all 4 pages now share "Always up for a good conversation." (was "Let's talk about your next project." on home/about and "If you would like to chat" on work/method).

### about.html
- **Mary Salome attribution**: removed per-pillar `<div class="pillar-attr">As described by Mary Salome</div>` from all 3 pillar cards. Attribution remains only in the section tag. Was appearing 4× total (1 section tag + 3 card footers) — felt like a chant without context.
- **Teaching vignette**: separated teaching (Saint Mary's cohort) from consulting (community nonprofits) into distinct beats. The consulting period was not formally tied to Saint Mary's, so conflating them was misleading.
- **Microsoft Excel cert badge removed**: dropped from cert grid. For someone with 19 years' experience and an MS in Business Analytics, certifying Excel read as overcorrecting. Remaining badges: Google Cloud Essentials, Data/ML & AI Baseline, Scientific Data Processing.
- **Footer unified**: matches all other pages.

### work.html
- **Career chip strip removed**: the chip-arrow strip duplicating the horizontal timeline (Elegrity → eBay → Apple → MS Business Analytics · 2022 → SFMTA) is gone. It duplicated the timeline, dropped the consulting period, and inserted "MS Business Analytics · 2022" as a career stop (not accurate). Timeline carries the arc cleanly.
- **Projects split into two sections**:
  - **"Case Studies"** (three in depth) — iTunes, iCloud, Kernel Updates. Full step-by-step treatment.
  - **"Notes, Essays & Side Quests"** (four lighter reads) — eBay, SHAP, Secret Gardens, Conditional Probability. Framed honestly as lighter pieces.
- **Outcome lines added to all 4 lighter projects**: each now ends with a `step-outcome` block summarizing the result — eBay (security reviews became proactive), SHAP (default translation layer for model outputs), Secret Gardens (public Tableau dashboard of POPOS), Conditional Probability (first time Bayes makes sense).
- **Footer unified**: "Always up for a good conversation." (was "If you would like to chat").

### method.html
- **Skill bars normalized**: all `data-width` values set to 100. Was 85–98% — arbitrary precision on soft skills that can't be defended. Bars now function as visual rhythm, not false measurement.
- **"SQL / Python / R" renamed**: skill label is now "Working in code" — the original label bunched three distinct tools into one row with no explanation.
- **Bell curve peak callout updated**: replaced "Trust / Vision / Leadership" (abstract noun stack) with "Hand me the vision, get out of the way." (concrete, matches the register of the caption below). SVG rect widened to fit.
- **Footer unified**: "Always up for a good conversation." (was "If you would like to chat").

---

## Still open

### Images still needed (Nabil to create externally)
- Three Pillars illustration (replace `ThreePillars.png`)
- Kernel Updates before/after dot-grid (no image for this case study yet)
- Testimonial word cloud (replace `Testimonials.png`)
- Education Through-Line to replace `Education.png` (now orphaned — `EducationWalkPainted.png` in use)

### Optional additions (whimsy budget)
- **"Now" strip on home** — what's on the workbench at SFMTA (anonymized), what you're reading, current tea. Derek Sivers /now-page convention. Reinforces not-job-hunting stance.
- **Cat cameo** — a small line in the footer or hero ("Reviewed by Octavia") for the kind of whimsy that makes a site memorable.
- **iTunes "Pagers Going Quiet" line chart** — coded SVG showing pager events dropping as crash-tracking came online. Stronger than the current outcome text alone.

### QA
- Browser QA on all 4 pages, especially career and education timelines on mobile.
- Verify `ProfilePicture.jpeg` loads correctly from root in index.html (path fixed this session).
- Check cert badge 2×2 grid with 3 items (Excel removed) — last cell is empty, confirm layout looks fine or switch to 3-col.

---

## Page structure (current)

| Page | Sections |
|------|----------|
| **index.html** | Hero · Stats strip (4 yrs Saint Mary's replaces Apple teams) · Brianna pull-quote (trimmed) · "The work, briefly" · 3 project cards |
| **work.html** | "A Through-Line" (caption + CareerJourneyPainted + timeline, no chip strip) · "Case Studies" (iTunes, iCloud, Kernel — 3 deep) · "Notes, Essays & Side Quests" (eBay, SHAP, Secret Gardens, Conditional Probability — all with outcome lines) |
| **method.html** | 3 Moves · Duct Tape/Drano · Bell Curve (updated callout) · Skill toolkit (uniform bars, "Working in code" label) |
| **about.html** | Portrait grid · Three Pillars (no per-card attribution) · Teaching vignette (teaching + consulting separated) · What People Say · Education & Certs (3 badges, Excel dropped) |

---

## Technical notes
- All 4 pages share footer copy: "Always up for a good conversation." + "If there's an interesting problem in the room, I want to hear about it."
- Hero image path: `ProfilePicture.jpeg` (root) on both index.html and about.html — consistent now.
- `Education.png` is orphaned (not referenced in any live page). Safe to delete.
- Dead CSS in work.html: `.section-banner` and `.river-cta` classes remain in the style block but are not used in the page body. Safe to trim on a cleanup pass.
- Design tokens, fonts, and nav unchanged across all pages.
