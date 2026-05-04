# Next Session Handoff

## Current state (May 4 2026)

Live root files: `index.html`, `about.html`, `work.html`, `patterns.html` (renamed this session from `method.html`). Note pages: `probability.html`, `gardens.html`, `unicorns.html`. Nav: Home · Work · Patterns · About.

**Rename:** `method.html` → `patterns.html` this session. All seven HTML files updated; the home project card pointing to the page was caught too. No redirect stub — the page hadn't been broadly published under the old URL. README updated; older entries in this file still say `method.html` because they describe past sessions accurately, not current state.

**Image re-encode:** all eleven painted assets the live site references were converted from PNG/JPEG to WebP (quality 82, capped at 900px wide; 1100 for the career illustration; 560 for the profile; 200 for the footer Cleo). Total live asset weight 31.5 MB → 0.9 MB (about 97% reduction). Originals removed from working tree but preserved in git history. `WordClouds Painted.png` lost its space in the rename → `WordCloudsPainted.webp`. Retained-as-PNG: `ConstellationPainted.png` (intentionally archived), and the orphans `Testimonials.png` / `ThingsILove.png` / `lighthouse.png` / `avatar.png` / `ac-river-scene.png` (still flagged safe-to-delete in README).

**Other improvements this session:** every below-the-fold image got `loading="lazy"`; meta descriptions added to all seven pages; the redundant inline italic labels on the bell-curve SVG (`Too stuck in status quo` / `Too unstructured`) were dropped — the captions below the SVG already say it.

**Open items I flagged but didn't change** (editorial calls left for Nabil): home stats-strip slot 2 ("300M+ iTunes users behind the dashboards") reads as a borrowed number; Brianna's pull-quote on home doesn't appear in the About testimonials; hero body and pull-quote on home overlap thematically; "Education" side-fact uses `·` as both within-entry and between-entry separator; Patterns toolkit columns are uneven (4/5/3 chips) and "Working in Code" is the most generic chip; tenure bar says "Consulting" while career timeline says "Independent Consulting." Browser QA was not possible from this session.

---

## Current state (older snapshots below — historical)

All prior branches have been merged to master. Redesign/ folder has been promoted to root — the four live files are now `index.html`, `about.html`, `work.html`, `method.html` at repo root. Several further fixes were applied after the initial promotion (Honors removal, UC Berkeley removal, George Mason arc label update, duplicate career illustration removed).

---

## What changed (three rounds of work)

### Round 1: Redundancy & reorganization (see git log for details)
- index.html: eliminated triple-repeated "ambiguity → clarity" message
- about.html: removed duplicate "Things I Love" grid; removed Ipsita quote from vignette; added nonprofit consulting to vignette; moved Education & Certs here; removed Bell Curve
- method.html: merged Q2+Q4; converted 6 questions to 5-step visual funnel; added Bell Curve
- testimonials.html: removed Education section; removed Brianna duplicate; curated from 15 → 7 testimonials

### Round 2: LinkedIn content additions
- work.html: added iCloud outage tracking case study; added eBay security program case study; added role titles + dates to all case study meta tags
- about.html: added nonprofit consulting to teaching vignette

### Round 3: Visualizations
- **work.html** — Added horizontal career timeline below CareerRiver.png. 5 employers with color-coded emoji dots (Elegrity=sage, eBay=mustard, Apple=coral, SMC=lavender, SFMTA=teal). SFMTA has glow ring + "Now" badge. Scrollable on mobile.
- **about.html** — Replaced plain education list with a vertical timeline (UChicago → George Mason → UC Berkeley → Saint Mary's), each with an arc label showing the learning progression ("arguing from evidence" → "adding technical layer" → "sharpening data skills" → "bringing it all together"). Replaced plain cert list with a 2×2 badge card grid.
- **index.html** — Replaced "Apple (7 yrs) · eBay · Elegrity" text with a mini horizontal bar chart showing tenure at each pre-SFMTA employer, proportional to Apple's 7-year max.
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

### 1. Education Through-Line — ✅ EducationWalkPainted.png is live
`EducationWalkPainted.png` is already in use on about.html. The live education timeline now has 3 stops (UC Berkeley was removed):
- **University of Chicago — BA, English Literature** — arc label: "Rigorous storytelling"
- **George Mason University — MS, Information Systems** — arc label: "From novels to databases"
- **Saint Mary's College — MS, Business Analytics** (no Honors marker) — arc label: "Bringing it all together"
If a new painted illustration is created, it should match these 3 stops. Note: `Education.png` is now orphaned and can be deleted.

### 2. Three Pillars illustration — ✅ ThreePillarsPainted.png is live
ACNH museum interior scene. Character (canonical chibi) stands left of frame gesturing toward three display pedestals. Each pedestal holds a symbolic artifact (framed constellation painting, golden shield, brass balance scale) with a large readable label card. Amber gallery lighting, parquet floor. Replaced `ThreePillars.png` on about.html.

### 3. Kernel Updates illustration — ✅ KernelCleanupPainted.png is live
ACNH outdoor garden scene. Character crouched center-frame pulling weeds, looking back at the transformed right side. Left half: overgrown weeds, crooked corkboard with illegible crumpled tickets. Right half: neat blooming garden, clean bulletin board with organized status. Small wooden "Before / After" signs with readable subtitles. Added to work.html between project-lead and project-tags on the Kernel Updates case study.

### 4. Testimonial word cloud — ✅ WordClouds Painted.png is live
ACNH Dream Suite aesthetic. Deep indigo-purple night sky, pink and lavender floating clouds, warm golden stars. Character sitting upright (not sleeping) on a large central cloud, reaching out to touch one of the floating word-bubbles. Ten word-bubbles in varying sizes and site accent colors: largest in coral/teal ("asks the right questions," "translates complexity," "humanity"), medium in mustard/lavender, smaller in sage. Replaced `Testimonials.png` on about.html.

### 5. iTunes "Pagers Going Quiet" before/after mini chart
The iTunes case study has a strong narrative but no visual anchor beyond the emoji. A simple line/bar chart showing pager events dropping week-over-week as the crash-tracking system came online would make the outcome visceral. This one could be a coded SVG rather than an illustration.

---

## Visualizations in the live site

| Viz | Page | Type |
|-----|------|------|
| Stats strip | index.html | 4 big numbers |
| Tenure bar chart | index.html | horizontal mini-bars (side facts) |
| Brianna pull-quote | index.html | styled blockquote |
| Bell curve (job satisfaction) | method.html | inline SVG |
| Favorite questions | method.html | colored vertical bars + Playfair italic — replaced 3-Move funnel ✅ |
| Skill chips | method.html | color-coded pill tags (teal/lavender/coral) — replaced bars ✅ |
| Duct Tape / Drano panels | method.html | two-panel card |
| Career timeline | work.html | horizontal CSS rail + 6 colored dots (incl. Sabbatical node ✅) |
| Education timeline | about.html | vertical CSS rail + 3 stops (UChicago, George Mason, Saint Mary's) |
| Cert badges | about.html | 3-column card grid (Excel removed ✅) |
| Portrait mini-bars (tea) | about.html | tiny CSS bars |
| Testimonials themes row | about.html | colored chip strip |

### Images — current state
| File | Used by | Notes |
|------|---------|-------|
| `AboutHero.png` | about.html | "The Human Behind the Projects" |
| `CareerJourneyPainted.png` | work.html | career journey illustration |
| `EducationWalkPainted.png` | about.html | "Education & Certifications" |
| `ThreePillarsPainted.png` | about.html | "Three Things I Always Bring" ✅ |
| `KernelCleanupPainted.png` | work.html | Kernel Updates case study illustration ✅ |
| `WordClouds Painted.png` | about.html | "What People Say" — in progress |
| `TeachingScene.png` | about.html | "One More Thing" |
| `ThingsILove.png` | index.html | "The work, briefly" section thumbnail |
| `ProfilePicture.jpeg` | about.html + index.html | hero avatar (both at root path — consistent) |
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
  - **"Notes, Essays & Side Quests"** (four lighter reads) — eBay, Secret Gardens, Conditional Probability, Chasing Unicorns for Pride. Framed honestly as lighter pieces. (SHAP removed as outdated.)
- **Outcome lines added to all 4 lighter projects**: each now ends with a `step-outcome` block summarizing the result — eBay (security reviews became proactive), Secret Gardens (public Tableau dashboard of POPOS), Conditional Probability (first time Bayes makes sense), Unicorns (data story that ends somewhere unexpected).
- **Footer unified**: "Always up for a good conversation." (was "If you would like to chat").

### method.html
- **Skill bars normalized**: all `data-width` values set to 100. Was 85–98% — arbitrary precision on soft skills that can't be defended. Bars now function as visual rhythm, not false measurement.
- **"SQL / Python / R" renamed**: skill label is now "Working in code" — the original label bunched three distinct tools into one row with no explanation.
- **Bell curve peak callout updated**: replaced "Trust / Vision / Leadership" (abstract noun stack) with "Hand me the vision, get out of the way." (concrete, matches the register of the caption below). SVG rect widened to fit.
- **Footer unified**: "Always up for a good conversation." (was "If you would like to chat").

---

## Still open

- **Browser QA** on all 4 pages (especially About's new 4-col grid + testimonials themes row wrapping on narrow screens).
- **Testimonial word cloud** ✅ — `WordClouds Painted.png` live on about.html. Dream Suite aesthetic (deep indigo/purple sky, floating cloud word-bubbles, character sitting upright on a cloud).
- **iTunes case study removed** ✅ — consolidated into iCloud. `QuietedPagersPainted.png` intentionally archived (not deleted, not referenced). index.html work card updated to 6 projects, 2 in depth.
- **Cat cameo** ✅ — `CleoInspects.png` in footer of all 4 pages as "Inspected by Cleo."
- **iCloud illustration** ✅ — `ConstellationPainted.png` live on work.html (between project lead and tags on the iCloud case study). Constellation metaphor: chaotic night sky → stars connected into root-cause constellations.
- **iCloud illustration** ✅ — `ConstellationPainted.png` live on work.html iCloud case study.
- **All case studies need a full rewrite** — copy has gotten distorted over multiple editing passes. Start fresh from source material (LinkedIn, memory) rather than editing what's there. Affects: iCloud, Kernel Updates, eBay on work.html. iCloud in particular needs to reflect the correct story: Apple's properties (iCloud, iTunes, Maps) had no shared way to track downtime and root causes over time; built a consistent measurement framework across all of them.

### Images — done
| File | Use |
|------|-----|
| `CareerJourneyPainted.png` | work.html — career journey illustration ✅ |
| `EducationWalkPainted.png` | about.html — Education & Certifications ✅ |
| `ThreePillarsPainted.png` | about.html — "Three Things I Always Bring" ✅ (replaced ThreePillars.png) |
| `KernelCleanupPainted.png` | work.html — Kernel Updates case study, between project-lead and tags ✅ |

---

## Copy & content suggestions (not yet implemented)

These are editorial changes identified in review — none require new illustrations, just copy edits or small structural decisions.

### High priority

**1. Footer copy — unify across all 4 pages**
Currently mismatched: index + about say "Let's talk about your next project." (job-seeker-y); work + method say "If you would like to chat." Pick one voice for all four. Suggested: "Always up for a good conversation." or "In my element when there's an interesting problem in the room." — keeps the door open without hustling.

**2. "Six stories, told in steps." on home — fix count and framing**
index.html Selected Work card currently says "Six stories, told in steps." Work page has 7 projects, and only iTunes/iCloud/Kernel have step-by-step treatment. Two fixes: (a) update the count, (b) reframe the description so it doesn't oversell the lighter pieces.

**5. Hero image path inconsistency**
index.html (line 269) references `inspiration_samples/ProfilePicture.jpeg`; about.html references `ProfilePicture.jpeg` at root. Both files probably exist but it's a maintenance smell. Pick one location and point both pages to it.

**6. Honors label drift — index.html line 368**
index.html still reads "MS Business Analytics (Honors) · UChicago BA, English Lit". The Honors flag was removed from the Saint Mary's entry on About. These should match.

### Medium priority

**3. Work page structure — split into two tiers**
Currently 7 case studies in one undifferentiated list. The first 3 (iTunes, iCloud, Kernel) are deep case studies with step-by-step treatment; the last 4 (eBay, SHAP, Secret Gardens, Bayes) are lighter pieces with only a lead paragraph + tags. Two options:
- Split into "Case studies" + "Notes, essays & side quests" sections (the second label fits the whimsy)
- Or add at least one concrete outcome line to each of the lighter 4

**4. Mary Salome attribution — reduce repetition on About**
"As described by Mary Salome" appears on each of the 3 pillar cards. We don't know who she is. Either: explain her once at the top of the section ("a friend who once described me as having three pillars…") and drop the per-card attribution, or keep it only as the section heading tag and remove from each card.

**7. Stats strip — too Apple-heavy**
Three of the four stats are Apple-flavored (300M+ iCloud users, 300+ engineers, 40+ teams). With 19 years of experience this makes the rest of the career invisible. Options: swap one for an SFMTA stat, a teaching/mentorship stat ("4 years teaching at Saint Mary's"), or something whimsical ("2 cats rehabilitated") to match the site's voice. The stats currently read like a resume, at odds with the relaxed tone everywhere else.

**8. Skill bars on method.html — still open**
The bars animate to specific percentage widths (88–98%) via `data-width` attributes — no text labels are shown, but the visual still implies false precision (Stakeholder Mgmt bar visibly wider than Agile bar). Three open options:
- Drop the varying widths; make all bars uniformly full so they're purely visual rhythm
- "SQL / Python / R" as a single bar row is confusing — either split into separate rows or rename to "Working in code"
- Consider replacing bars entirely with chips grouped by "what I love using" / "what I'm sharpening" — more honest and fits the playful tone better

**9. Career chip strip on work.html — consider removing**
work.html has: painted illustration → 5-node career timeline → chip-arrow strip (Elegrity → eBay → Apple → MS Business Analytics · 2022 → SFMTA). That's three views of the same arc. The chip strip also drops the consulting period and substitutes "MS Business Analytics · 2022" as a career stop, which is odd. The timeline already carries this; the chip strip adds noise.

**10. Cert badges — trim**
about.html has 4 badges: Google Cloud Essentials, Data ML & AI Baseline, Scientific Data Processing, Microsoft Excel. For someone with 19 years and an MS in Business Analytics, certifying Excel reads as overcorrecting. At minimum drop the Excel badge. Could collapse all four to a single line: "Google Cloud + ML foundations, 2024."

**11. Bell curve peak label — let the caption work harder**
method.html bell curve peak is labeled "Trust / Vision / Leadership" — abstract noun stack. The caption already says "trusted with the vision, given room to lead" which is much better. Consider replacing the peak callout with something concrete like "Hand me the vision, get out of the way." and letting the caption explain it.

**12. Brianna pull quote — trim for punch**
index.html quote: "He has the unique ability to walk into an ambiguous situation, quickly grasp the key milestones and action items, identify technical needs that have not been addressed, and get results — all while getting a smile out of everyone in the room."
Middle clause ("quickly grasp the key milestones and action items") dilutes it. Suggested trim: "He walks into ambiguous situations, identifies what hasn't been addressed, and gets results — all while getting a smile out of everyone in the room."

**13. Teaching vignette — separate teaching from consulting**
The `redesign/` version rewritten to reflect 4-year Saint Mary's arc (done ✅). One remaining editorial note: the vignette currently slides from "I taught my MS cohort" to "I consulted for community nonprofits" as if the consulting was formally tied to Saint Mary's — it wasn't. Worth splitting into two crisp sentences: one about the teaching instinct (cohort), one about where that instinct was applied (consulting for nonprofits independently).

### Lower priority / additive

**15a. "Now" strip on home**
A small strip (Derek Sivers /now-page convention) showing what's currently on the SFMTA workbench (anonymized), what Nabil is reading, current tea. Reinforces "not job-hunting, just available for conversation." Would sit naturally between the stats strip and the Brianna quote, or at the very bottom before the footer.

**15c. Cat cameo in footer or hero**
Cats currently appear in chips and the portrait grid. A single candid line somewhere — e.g. "Reviewed by Octavia" in the footer, or a one-liner in the hero — is the kind of whimsy that makes a site memorable without taking up space.

**16b. Dead CSS in work.html** ✅ — `.section-banner` and `.river-cta` rules removed.

---

## Current page structure

| Page | File | Sections |
|------|------|----------|
| Home | `index.html` | Hero · Stats strip · Brianna pull-quote · "The work, briefly" (English-major-in-disguise framing) · Selected work (3 cards → Work, Patterns, About) |
| Work | `work.html` | "A Through-Line" (CareerJourneyPainted.png + career timeline) · 6 projects: eBay + iTunes + Kernel (deep case studies, all rewritten from source) · Secret Gardens, Conditional Probability, Chasing Unicorns (lighter pieces, link to dedicated note pages) |
| Patterns | `method.html` | Some of My Favorite Questions (incl. "What are you reading?") · Two Kinds of Problems (Duct Tape / Drano) · Bell Curve sweet spot · Skill toolkit (Translating Complexity in Communication column) |
| About | `about.html` | Portrait grid (4 cells, section-intro alignment fixed) · Three Pillars · Teaching vignette · Off the Clock (feminist SF — Butler / Delany + Touchstones chip strip) · What People Say (testimonials lead — recurring-words chip strip removed) · Education & Certs (3 stops + 3 cert badges) |

### Images — all done ✅
All planned illustrations are live. No images currently needed.

| File | Use |
|------|-----|
| `QuietedPagersPainted.png` | work.html — iTunes case study illustration ✅ (restored from archive when iTunes replaced iCloud) |
| `ConstellationPainted.png` | intentionally archived — was the iCloud case study illustration before iTunes replaced that slot |

### Optional additions (whimsy budget)
- **"Now" strip on home** — what's on the workbench at SFMTA (anonymized), what you're reading, current tea. Derek Sivers /now-page convention. Reinforces not-job-hunting stance.
- **Cat cameo** — a small line in the footer or hero ("Reviewed by Octavia") for the kind of whimsy that makes a site memorable.

### QA
- Browser QA on all 4 pages, especially career and education timelines on mobile.
- Verify `ProfilePicture.jpeg` loads correctly from root in index.html (path fixed this session).
- Cert badge grid switched to 3-col ✅ — no blank cell.

---

## Page structure (current)

| Page | Sections |
|------|----------|
| **index.html** | Hero (kicker softened: "At SFMTA since April 2024 · Always up for a good problem") · Stats strip · Brianna pull-quote · "The work, briefly" (English-major-in-disguise) · 3 project cards (Work / Patterns / About) |
| **work.html** | "A Through-Line" (caption + CareerJourneyPainted + timeline) · "Case Studies" (eBay, iTunes, Kernel — 3 deep, all rewritten from source — chronological) · "Notes, Essays & Side Quests" (Secret Gardens, Conditional Probability, Chasing Unicorns — link to dedicated note pages) |
| **method.html** (Patterns) | "Some of My Favorite Questions" (4 incl. "What are you reading?") · Two Kinds of Problems (Duct Tape/Drano, project-name-free notes) · Bell Curve sweet spot · Skill toolkit (color-coded chips, no JS — Translating Complexity now in Communication column) |
| **about.html** | Portrait grid (section-intro thumbs center-aligned at 180px) · Three Pillars · Teaching vignette · Off the Clock (feminist SF + Touchstones) · What People Say (testimonials lead — chip strip removed) · Education & Certs (3 badges) |

---

## Technical notes
- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--coral` on Home/Work · `--teal` on Patterns · `--lavender` on About
- Nav is self-contained within `redesign/`
- LinkedIn profile PDF in repo root (`linked_in_profile.pdf`)
- All 4 pages share footer copy: "Always up for a good conversation." + "If there's an interesting problem in the room, I want to hear about it." Footer tagline "Made with curiosity & care" removed.
- Hero image path: `ProfilePicture.jpeg` (root) on both index.html and about.html — consistent.
- `Education.png` is orphaned (not referenced in any live page). Safe to delete.
- Dead CSS in work.html (`.section-banner`, `.river-cta`) ✅ — removed per suggestion #16b.
- Design tokens, fonts, and nav unchanged across all pages.

---

## What changed this session (April 26 2026 — review implementation pass)

All changes implement findings from the April 26 review below. One task per commit.

### Footer cleanup (committed separately before this pass)
- **"Made with curiosity & care" removed** from all 4 pages — line was redundant with the footer headline.
- **Cleo image enlarged** from `height:22px` to `height:36px` on all 4 pages.

### Review items completed
- **iCloud illustration wired up** — `ConstellationPainted.png` added to work.html between the iCloud project lead and tags, matching `KernelCleanupPainted.png` placement on the Kernel case study. ✅
- **Stats strip reframed** — "iCloud users at launch" changed to "iCloud users whose outages I tracked" so the 300M number reads as Nabil's contribution, not Apple's. ✅
- **Bell curve right-side label** — "In need of constraints" → "Too unstructured" (parallels "Too stuck in status quo" on the left). Caption updated to match. ✅
- **Funnel question 2 trimmed** — Two stacked questions merged with an em-dash into one fluid question. ✅
- **Drano panel duplicate removed** — Both Duct Tape and Drano referenced the kernel project. Replaced the Drano instance with the eBay security backlog example (surfacing a buried queue = Drano). ✅
- **Mary Salome attribution** — "as described by Mary Salome" → "as described by Mary Salome, a longtime friend." ✅
- **Cert badges grid** — 3 badges in a 2-column grid left a blank cell. Switched to 3-column grid with a 1-col mobile fallback. ✅
- **Unclosed div** — `career-timeline` div in work.html was opened but never explicitly closed. Fixed. ✅

### Still open / needs Nabil input
- **Skill bars → chips** ✅ — Replaced all 12 bars with color-coded chip pills. IntersectionObserver JS removed.
  - **AC illustration idea for this section:** character at the ACNH crafting table with three labeled "recipe cards" spread out (one per column), each with the skill names hand-lettered on them in the ACNH style. Could replace the three-column grid entirely or sit above it.
- **Dedicated note pages** ✅ — `probability.html` (full Conditional Probability essay, mustard accent, two reconstructed HTML tables), `gardens.html` (Secret Gardens Tableau embed, sage accent), `unicorns.html` (Unicorns Tableau embed, teal accent). All use site nav, footer, and design tokens. work.html lighter reads trimmed to teasers linking to local pages.
- **"Chasing Unicorns for Pride" added** ✅ — new lighter read (🦄, teal accent). Section tag reads "four lighter reads" because SHAP was dropped at the same time.
- **SHAP lighter read removed** ✅ — dropped per Nabil ("feels outdated now").
- **Case study images shrunk** ✅ — `KernelCleanupPainted.png` and `ConstellationPainted.png` capped at 420px (was full-width). Centered with `margin: 16px auto 24px`. Duplicate ConstellationPainted img tag on iCloud case study removed at the same time.
- **2018–2020 gap** ✅ — Added "Sabbatical · Deliberate pause · 2018–2020" node (sage color, 🌿) between Apple and Independent Consulting.
- **Mary Salome attribution** ✅ — Updated to "a longtime friend and collaborator."
- **Case studies full rewrite** — still needed. Copy has drifted. Start from LinkedIn + memory, not by editing what's there.
- **"Now" strip on home** — needs content from Nabil (SFMTA workbench item, current read, current tea).
- **Browser QA** — especially About's 4-col portrait grid and testimonials themes row on mobile.

---

## Review — April 26 2026 (whimsy-allowed pass)

Full re-read of all 4 pages with the brief: "I'm not job-hunting, I can afford to be whimsical." Findings ordered by impact. None implemented yet.

### High impact

**R1. method.html — skill bars are all 100%.**
All twelve `data-width` values were normalized to 100 in a prior pass (see "What changed this session" → method.html). Visually this means twelve full bars. The intent ("visual rhythm, not measurement") doesn't survive contact with a reader: twelve full bars reads as "I rated myself 10/10 on everything," which is the one moment on an otherwise self-aware site where credibility wobbles. Two clean exits:
- Calibrate honestly (e.g. PM 95, Process Design 95, Agile 80, Gap Analysis 85, Working in code 65). Honest variance is more persuasive than uniform mastery.
- Or drop the bars entirely and use the same chip/pill style the site already uses elsewhere — keeps the playfulness without making a quantitative claim.

**R2. work.html — "Notes, Essays & Side Quests" don't link anywhere.** ✅ Resolved.
Secret Gardens, Conditional Probability, and Chasing Unicorns for Pride each have a dedicated local page (`gardens.html`, `probability.html`, `unicorns.html`). work.html entries are teasers linking to those pages. SHAP removed as outdated. eBay has no dedicated page — linkless by design.

**R3. index.html — "300M+ iCloud users at launch" is an Apple stat, not a Nabil stat.**
Readers feel the difference. Replace with a personal-impact number (e.g. dashboards still in use, hours reclaimed) or rephrase to "300M users on systems I supported." Note: this dovetails with the still-open suggestion #7 ("Stats strip — too Apple-heavy") above.

**R4. Wire up the iCloud illustration.**
`ConstellationPainted.png` is sitting in the repo root, unreferenced. Per the "Still open" notes above, it was the in-progress iCloud illustration (chaotic night sky → constellation lines revealing root causes). Kernel Updates has an illustration; iCloud doesn't, which makes the Case Studies section visually asymmetric. Drop it into the iCloud project-item between project-lead and project-tags, mirroring the `KernelCleanupPainted.png` placement at work.html:255.

### Medium impact

**R5. eBay Site Security feels miscategorized as a "lighter read."**
It's framed as serious work (security architecture, decision support model) but lives under "four lighter reads" with only an outcome and no steps. Either promote it to a third case study with steps, or trim it to genuinely match the lighter tone of the others (SHAP, Secret Gardens, Bayes).

**R6. work.html — the 2018 → 2020 gap on the career timeline is unaddressed.**
Apple ends 2018, Independent Consulting starts 2020. Two-year gap reads as an unanswered question. The whimsical-because-not-job-hunting brief invites owning it directly — a small node ("between roles · reading, traveling, recovering from Apple," or whatever's true) would land better than the silence.

**R7. about.html — "as described by Mary Salome" needs context.**
Who is she? Friend, mentor, manager? Currently lives only as a section tag. A four-word descriptor in the section-h or a single intro sentence above the pillars ("a longtime friend who once told me…") would make this land. Earlier work removed the per-card attribution (good); this is the remaining residue.

**R8. method.html — Drano example duplicates Duct Tape example.**
Both panels reference the kernel update project. Pick a different Drano-flavored case so the contrast actually contrasts. The "spreadsheet nobody could read → automated crash-tracking" line in the same panel is good and could carry it alone.

### Small / polish

- **method.html bell curve label.** "In need of constraints" reads ambiguously (does it mean *you* need them?). "Needs structure" or "Too unstructured" parallels "Too stuck in status quo" cleanly.
- **method.html funnel question 2** is two questions stacked. Trim to: "What's actually in your way — the manual task you dread, the approval stuck somewhere, the data you don't have?"
- **index.html hero alt text** ("Animal Crossing character portrait standing in a village") is a great whimsical detail but only screen-reader users see it. A small visible caption or one-line "what is this?" hover would let everyone in on the joke. First-time visitors may genuinely wonder if it's a stylized photo or a game character.
- **Cat cameo expansion.** "Inspected by Cleo" in the footer is perfect. Per the open optional-additions list, a rotating second cat ("Inspected by Cleo · Audited by Octavia") would honor both rescues.
- **"Now" strip on home** (already in the optional/whimsy backlog above) is the single highest-leverage addition for reinforcing the not-job-hunting posture. No other change communicates that posture as directly.

### What's working well — leave alone

- Color palette + Playfair/Nunito pairing — confident and warm.
- Painted illustrations as section thumbnails — distinctive and personal.
- Catherine Madden bell curve, Duct Tape/Drano framing, Three Pillars — all memorable structures that beat the standard skills/projects/contact template.
- Testimonials with the "recurring words" chip strip on top — gives skim-readers a thesis before the quotes.
- "Six months from now, you are really happy. What has changed?" is the strongest single line on the site. Don't touch.
- Footer "Inspected by Cleo" with the photo — perfect tone.

### Suggested implementation order

If picking changes off one at a time: R1 (skill bars) → R4 (wire up constellation illustration) → R3 (de-Apple the stats strip) → R2 (link the lighter pieces). These four together address every "credibility wobble" without touching anything that's already working.

---

## Review — April 28 2026 (second whimsy pass · feminist-SF round)

Brief: "Not job-hunting, but want to keep my hand in. Could we work feminist SF in anywhere?" Status legend: ✅ done · → in progress this session · ⏸ deferred · ✗ declined.

### High impact

**S1. about.html — no reading/writing life shown anywhere.** ✅
The English-Lit-major / "translates complexity" through-line was never carried into the off-duty register. Added an "Off the Clock — the other writing life" vignette between the Teaching Vignette and Testimonials, naming feminist SF as the genre, Octavia E. Butler as the cat's namesake, and an anchor author "on the nightstand." Uses sage→teal gradient on the existing `.vignette` so it pairs with but doesn't duplicate the lavender→mustard teaching vignette directly above it. Confirmed by Nabil: Octavia *is* named for Butler. Anchor author corrected from Le Guin → **Samuel R. Delany** at Nabil's request.

**S2. index.html — hero kicker still wears a tie.** →
"Principal Business Analyst · SFMTA · Since April 2024" reads CV-formal in the one place on the site that should set the whimsy tone. With the "not job-hunting" brief, options like *"At SFMTA since April 2024 · Not job-hunting, just curious"* or *"Currently at SFMTA · Tea-fueled · Up for a good problem"* fit the rest of the page better.

**S3. about.html — testimonial "Recurring words" chip strip is over-decorated.** →
7 chips in 5 colors reads as ornament rather than thesis. Tightening to 4–5 chips in 2–3 colors would make the recurring themes scan harder.

**S4. index.html — hero body and "The work, briefly" echo each other.** →
Hero says "Nineteen years of building the process that didn't exist yet." About-lead says "The process didn't exist yet — so I built it." Same beat, twice in 200 vertical pixels. Either differentiate the two (hero = career stat, about-lead = orientation) or replace the about-lead with a different beat entirely (e.g. what's on the workbench now).

### Medium impact

**S5. work.html — eBay Site Security is miscategorized.** ✅
(Restates R5 from April 26.) Resolved via promotion (option a). eBay is now the first of three case studies in chronological order (eBay 2009–11 → iCloud 2011–18 → Kernel 2014–18), matching the career timeline directly above. Lead and steps rewritten from source material Nabil provided rather than by editing the prior copy: roadmap (transparency), kick-started intake questionnaire, engagement processes for internal-consultant operating mode, cross-company discussion group with PayPal security. Tags switched from lavender (lighter-reads palette) to teal (case-study palette). Section tags updated: "two in depth" → "three in depth"; "four lighter reads" → "three lighter reads."

### Declined / decided against

**S6. "Now" strip on home (currently reading / current tea / etc.).** ✗
Already on the optional backlog above. Recommended *against* implementing on this pass: ages fast, requires maintenance, and the Cleo cameo + "Tea, not coffee" chip already do the same vibe-work without dating. If a Now strip ever lands, it should be the *only* dated content on the page so it's easy to keep fresh.

**S7. method.html — Duct Tape/Drano panel notes named specific projects, redundantly with case studies.** ✅
At Nabil's flag: the metaphor itself (Duct Tape = pulling disconnected things together, Drano = unclogging stuck things) is what should land in this section. Naming iCloud / kernel updates / eBay backlog in the panel notes (a) duplicated the case studies one page over and (b) buried the metaphor under project trivia. Rewrote both notes as italicized vignettes of the kind of dysfunction each panel describes — no project names, no numbers, just the shape of the problem and what Nabil does about it. Tags untouched (already abstract problem-types). Resolves the residual issue from R8 (which only addressed kernel-duplication across panels, not project-naming itself).

**S9. Method page renamed: "How I Work" → "Patterns."** ✅
Follow-on from S8. With the funnel gone (S8) and the metaphor section softened (S7), the page is closer to "patterns I notice in myself" than "my method." Renamed to **Patterns** across all visible labels — the file is still `method.html` (cheaper, no broken external links). Updated:
- Nav label "Method" → "Patterns" on all 7 pages (4 main + 3 lighter-read pages)
- method.html `<title>`: "How I Work" → "Patterns"
- method.html hero kicker: "My Process" → "Practice"
- method.html hero title: "How I _Work_" → "Some _Patterns_" (matches the section heading "Some of My Favorite Questions" in tone)
- Home card: label "Process" → "Practice", title "How I Work" → "Patterns", desc tightened ("the questions I keep asking, the two kinds of problems that keep showing up..."), CTA "See my method →" → "See the patterns →"
- README.md updated (nav line, file table description)
The hero sub ("The same pattern, project after project: ask until the real problem surfaces, pick the right tool, know when I'm in the zone") was already pattern-flavored and now reads as the perfect setup line — left untouched.

**S8. method.html — "Three Moves, Every Time" reframed as "Some of My Favorite Questions."** ✅
At Nabil's flag: "I never loved the method piece." The Define/Diagnose/Translate funnel framed the questions as a method he runs. He'd rather they read as questions he likes — less prescriptive, more characterful, fits the not-job-hunting brief. Refactored:
- Section heading "Three Moves, Every Time." → "Some of My Favorite Questions"
- Section tag "diagnostic" → "asked early, often"
- Funnel CSS removed; replaced with `.fav-questions` / `.fav-q` styling that mirrors the side-fact pattern from index.html (colored vertical bar + Playfair italic question, no labels, no commentary notes)
- Added a fourth question: **"What are you reading?"** Placed last as the punchline — pivots from work-shaped to person-shaped, reinforces the new Off the Clock thread on About without restating it.
- Color bars: coral / mustard / lavender / teal across the four questions
The Patterns-page hero sub ("ask until the real problem surfaces, pick the right tool, know when I'm in the zone") still parses fine without the funnel underneath it; left untouched. (Note: page subsequently renamed Method → Patterns in S9.)

### Things to leave alone (working well)

- Brianna Gamp pull quote on home — the strongest single asset on the site. Don't move, don't trim.
- Three Pillars on About (Mary Salome's words). Specific, attributed, unimitable. Unchanged.
- Sabbatical node on the career timeline — the confidence move reads as confidence. Keep.
- Education arc labels ("Rigorous storytelling" → "From novels to databases" → "Bringing it all together") — beautiful. Untouched.
- Patterns-page bell-curve caption ("Hand me the vision, get out of the way") — quotable. Keep.
- Footer "Inspected by Cleo" with photo — perfect tone, perfect dose.

---

## Review — April 30 2026 (luxury-of-whimsy pass · second feminist-SF round)

Brief: *"I'm not job-hunting right now, so I have the luxury of whimsy. But I do want to keep my hand in. What works? What doesn't? Could we work feminist SF in anywhere?"* Status legend: ✅ done · → in progress · ⏸ deferred · ✗ declined.

### Pushed this session ✅

**T1. index.html — feminist-SF chip on home hero.** ✅ (commit `5b8a5c3`)
Added `📚 Reads & writes feminist SF` as a fourth chip alongside `📍 SF`, `🍵 Tea`, and `🐱 Octavia & Cleopatra`. Same register as the others — declarative, not cute. Surfaces the off-the-clock thread on the home page so a reader who never makes it to About still feels it.

**T2. about.html — Touchstones chip strip below Off the Clock vignette.** ✅ (commit `5b8a5c3`)
Added six author chips below the existing reading-and-writing paragraph: **Octavia E. Butler · Ursula K. Le Guin · Samuel R. Delany · Joanna Russ · James Tiptree Jr. · N. K. Jemisin**. Butler and Delany were already named in the prose; the four additions are canonical feminist-SF picks made under Nabil's "take your best guess" license. Easy to swap if any don't belong on Nabil's list — Tiptree and Jemisin are the most likely candidates for adjustment. Existing prose left untouched (the "same instinct" sentence is doing the real thesis work).

### What's working — leave alone

- *"An English major's career, in disguise"* — the strongest line on the site, full stop.
- Brianna Gamp pull quote on home.
- Patterns page (Duct Tape / Drano + Bell Curve sweet spot + favorite questions) — original, distinctive.
- *"What are you reading?"* as the fourth favorite question — already does the connective work between SF and the work without flagging itself. Don't over-explain.
- Mary Salome Three Pillars.
- Off the Clock vignette prose — deliberately not edited on this pass; the touchstones chips sit below it.
- Cleo footer.
- Career timeline including the Sabbatical node.

### Recommendations — high impact

**T3. work.html — case studies need a full rewrite from source material.** ✅
All three deep case studies are now rewritten from source per the suggested shape (the moment walked in → the question that surfaced the real problem → concrete moves → what got better that you can name). eBay was already rewritten in S5. **Kernel** rewritten next: three concurrent threads (surface-what-tickets-buried / automate-the-work / renegotiate-the-bar with infosec), outcome leans on Nabil's "reverse burnout" phrasing. **iTunes** then replaced the iCloud slot entirely (Nabil: "this story is more compelling") — power-shift narrative about making bugs countable: SREs knew the cause, post-mortems sat in Word docs nobody could aggregate, MySQL prototype on a discarded box, monthly downtime reviews, the friend's call from the iTunes offsite with a screenshot of one of Nabil's vizzes on the VP's slide. Illustration swap: `ConstellationPainted.png` archived, `QuietedPagersPainted.png` restored from archive (it was always the right pairing).

**T4. about.html — recurring-words chip strip is doing two jobs and committing to neither.** ✅
Decision: kill it. The four-chip `t-themes` block above the testimonials is gone. Testimonials now lead the section directly without a warm-up.

### Recommendations — medium impact

**T5. method.html — "Translating Complexity" is in the wrong toolkit column.** ✅
Moved to Translation & Communication (sc-lav, lavender), placed first in that column so it pairs with the subtitle "Making complexity legible." Communication now has 5 chips, Analysis 3 — feels right for someone whose headline is the translating, not the analyzing.

**T6. index.html — three project cards, three same-shape cards.**
Still open. The "Selected work" cards all link to other pages of the same site (Work / Patterns / About) and use the same layout, same CTA. Reads as redundant rather than as three different invitations. If two became full-bleed teaser strips and one stayed as a card, the eye would have something to do.

**T7. index.html — stats strip phrasing.**
Still open. "300M+ iCloud users whose outages I tracked" is grammatically tangled, *and* the iCloud reference is now slightly orphaned (the case-study slot is iTunes-shaped after T3). Two cleanup options worth considering together: (a) repoint to iTunes scale, (b) just rephrase ("300M+ user reach"). (Same observation as April 26 R3.)

### Recommendations — lower priority / additive

**T8. A feminist-SF essay as a fourth Notes/Side Quest.**
Still open. Whimsy budget — purely optional. Same shape as `probability.html`, `gardens.html`, `unicorns.html`: a short piece on what one Butler novel taught about systems, or what feminist SF taught about asking *"why do we do it this way."* Would give the off-the-clock thread a destination on the site rather than just a mention, and would test whether a regular essay practice fits the tone. Title candidates if useful: *"Defamiliarize: what feminist SF taught me about asking why we do it this way"* / *"Reading Octavia Butler at the office."*

**T9. Browser QA still pending.**
Carried over from prior reviews. Especially: career and education timelines on mobile, About's 4-col portrait grid, **and the new About `.section-intro` thumbnail alignment after the gap fix** (`align-items: flex-start` → `center`, thumb 220px → 180px) — eyeball the five sections that use this pattern.

### Bonus item that landed alongside the T-series

**About-page section thumbnail alignment.** The five `.section-intro` rows on About had a structural gap problem: `align-items: flex-start` with a 220px-tall thumbnail beside a one-line heading meant the flex row's height was driven by the image, so content underneath only began after the image ended — leaving an L-shaped void below each heading. Fixed via `align-items: center` (heading vertically pairs with thumbnail) + thumb 220px → 180px (proportionally shorter row). Two-line CSS change. Mobile breakpoint untouched.

### Suggested implementation order

T3 / T4 / T5 / About-thumb-alignment all landed. **T6 + T7 resolved in the May 1 pass below** alongside R-series recommendations. **Still open: T8 (optional feminist-SF essay), T9 (browser QA).**

---

## Review — May 1 2026 (luxury-of-whimsy pass · third feminist-SF round)

Brief: *"Not job-hunting, luxury of whimsy. What works? What doesn't? Could we work feminist SF in anywhere?"* Same brief as the April 30 pass, fresh eye. Status legend: ✅ done · → in progress · ⏸ deferred · ✗ declined.

### Bug-tier fixes pushed first (commit `3b68baa`)

- **Duplicate hero chip on home** ✅ — `📚 Reading feminist SF` (older) and `📚 Reads & writes feminist SF` (T1) both lived on the hero. T1 should have replaced the older chip; instead it appended. Removed the duplicate.
- **Stats-strip orphaned iCloud reference** ✅ — `300M+ iCloud users behind the dashboards` repointed to `iTunes users` (the case-study slot is iTunes-shaped after T3). Smaller delta than R2 below, applied first as a bug fix.
- **Selected Work card on home — orphaned iCloud reference** ✅ — `iCloud outage systems, kernel updates...` updated to lead with the actual iTunes case study: `Making iTunes' crashes countable, kernel updates...`.
- **Bell-curve aria-label on Patterns** ✅ — still said `peaks at trust, vision, and leadership` (old peak copy from before that text was rewritten). Updated to match the visible `Hand me the vision, get out of the way.` peak label.

### R-series — recommendations pushed this session ✅

**R1. index.html — three same-shape Selected Work cards.** ✅
T6 from the April 30 pass, finally addressed. Restructured: one full-bleed teaser strip (image left, text right, coral→mustard gradient) leading the section, with `QuietedPagersPainted.png` as the visual anchor and a project-flavored title (*"Making iTunes' crashes countable, and other stories."*). Below it, a 2-col secondary grid with the Patterns + About cards (kept in their existing pcard style). The asymmetry gives the eye a hierarchy — *here is the work; here is the rest of the site* — instead of three flat invitations. Mobile collapses the teaser to single-column, image above text.

**R2. Stats strip — too Apple-heavy, no whimsy.** ✅
Replaced the 4th stat (`300+ Engineers using systems I built` — most generic of the four) with `1 Tiptree Award nominee · feminist SF`. Both fulfills the standing recommendation that the strip needed *one* whimsy stat among three serious ones, *and* lands the user-requested Tiptree mention in the highest-visibility location on the site. (Tiptree Award was renamed Otherwise Award in 2019; preserved user's original phrasing — easy swap if user prefers Otherwise.)

**R3. about.html — hero sub still hooks to colleague-testimony.** ✅
*"How an English-literature degree, two feral cats, and a stubbornly curious mind add up to **the kind of professional my colleagues describe below**."* — the closing clause was a 2024-job-hunt artifact. Rewritten: *"…add up to **a person who reads Octavia Butler at lunch and asks 'why do we do it this way?' before standup**."* Tells visitors what kind of room they're walking into; carries the feminist-SF thread + the favorite-question motif into the About hero.

**R4. about.html — Saint Mary's edu-dot still styled as honors.** ✅
The `edu-dot honors` class added a mustard ring + emoji 🏅 originally signalling MS Honors. The Honors *label* was removed in earlier work, but the dot kept its visual privilege — making Saint Mary's read as "the special one" of three. Dropped the `honors` class; emoji 🏅 → 🎓 to match the academic register of the other dots. All three stops now visually equivalent.

**R5. method.html — toolkit column titles read like LinkedIn headers.** ✅
*Project & Program Leadership / Translation & Communication / Analysis & Insight* with subtitles *Building what doesn't exist yet / Making complexity legible / Turning numbers into decisions*. Promoted the subtitles to titles; dropped the LinkedIn-flavored top line entirely. The new titles can stand alone — and match the voice of the rest of the page.

### User-requested addition

**Tiptree Award nomination mentioned in two places:**
1. **Stats strip on home** — as `1 Tiptree Award nominee · feminist SF` (R2 above). Highest-visibility surface.
2. **About > Off the Clock vignette** — added a sentence to the existing prose: *"…The drafts live in a different folder than the dashboards — one of them was nominated for the **Tiptree Award**."* Gives the stats-strip number narrative context for visitors who scroll into About.

### What's working — leave alone

Same list as April 30, with one addition:
- **The new home teaser strip** — the QuietedPagers painting was always the right visual to lead with on Selected Work. Don't fall back to three same-shape cards.

### Image audit (per user question)

**Kernel Updates already has its illustration** — `KernelCleanupPainted.png` is live on work.html line 285 (between project lead and tags). It's the painted before/after garden scene. No action needed; the user may have forgotten it's there.

**eBay Site Security Program — illustration done.** ✅ `LighthousePainted.png` live on work.html eBay case study, between project-lead and project-tags, capped at 420px to match iTunes/Kernel placement. Closes the visual asymmetry with the other two deep case studies.

Path that got us here:
1. First concept ("Map for the Maze" — noticeboard before/after with intake desk, bridge, second island, PayPal character) was rendered and didn't land. Diagnosed problem: too many competing metaphors (noticeboard, intake, bridge, second island, second character) — the working illustrations (`KernelCleanup`, `QuietedPagers`) each carry one strong central object through a before/after.
2. Brainstormed five single-object alternatives: lighthouse, bridge, constellation, open door, switchboard.
3. **Lighthouse** chosen — folds the cross-company beat into the central metaphor cleanly via a *second* lighthouse on a distant headland, with the two beams crossing in mid-air ("two organizations signaling to each other"). No second human character needed.
4. Two drafts generated by user. Picked `lighthouse2.png` over `lighthouse.png` on character canonicality (the latter had the character turned three-quarters away with face obscured; the former showed the canonical Nabil — glasses, goatee, hair, calm-and-quietly-proud expression — matching the rest of the site).
5. Renamed `lighthouse2.png` → `LighthousePainted.png` to match the existing `[Metaphor]Painted.png` naming convention. `lighthouse.png` runner-up left in the repo root for the user to delete.

The lighthouse beam is the shared map (transparency, visible work). The second lighthouse with crossing beams is the cross-company conversation with PayPal. The character is the calm keeper who turned the light on. Sign subtitles read **"Ships in fog"** / **"Beams crossing"**.

Surfaces that could plausibly use an illustration but currently don't:
- **About > Off the Clock vignette.** No section thumbnail (the section uses the inline-vignette pattern, not the section-intro pattern). Could add one — a painted scene of the character reading on a couch with a stack of SF paperbacks, or at a writing desk — but the prose + Touchstones chips are already carrying the section. **Verdict: not necessary.**
- **About > Education & Certifications.** Has `EducationWalkPainted.png`. Already done.
- **Method/Patterns > "What I Bring" toolkit.** The 3-column chip grid has no illustration. There's a dormant idea in this file (Round 4 image suggestion) about a crafting-table scene with three recipe cards. **Verdict: optional, no urgency. The chips are doing their job.**
- **Patterns > Two Kinds of Problems (Duct Tape/Drano).** No illustration. The 🩹/🪣 emoji + colored panels carry the metaphor. **Verdict: leave alone.**

**Recommendation: no new images needed.** All three deep case studies now have painted before/after illustrations. Everywhere else, what's there is sufficient.

### Still open

- **eBay illustration** ✅ — `LighthousePainted.png` live on work.html. See Image audit above for the full path-that-got-us-here.
- **`lighthouse.png` runner-up cleanup** — sitting in the repo root, unused; safe to `git rm` whenever convenient.
- **T8 — feminist-SF essay** as a fourth Notes/Side Quest. Carried forward.
- **T9 — browser QA.** Carried forward, with one new surface to eyeball: the **R1 home teaser strip** at the 720px breakpoint (collapses image-above-text, image capped at 240px) and on narrow mobile. Also worth eyeballing the new `LighthousePainted.png` rendering at the 420px cap on mobile.
