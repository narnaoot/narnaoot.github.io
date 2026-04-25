# Next Session Handoff

## Current branch

`claude/review-website-docs-P8MwH` — redundancy/reorganization + LinkedIn content + visualizations pass. Not yet merged to master.

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

| Page | File | Sections |
|------|------|----------|
| Home | `redesign/index.html` | Hero, stats strip, Brianna pull-quote, about blurb w/ ThingsILove thumbnail + tenure bar chart side-facts, 3 project cards |
| Work | `redesign/work.html` | CareerRiver image + career timeline viz, 6 case studies (3 professional, 3 personal/academic) |
| Method | `redesign/method.html` | 5-question diagnostic funnel, Duct Tape/Drano, Bell Curve SVG, animated skill toolkit |
| About | `redesign/about.html` | Portrait grid, Three Pillars, teaching vignette (+ nonprofit consulting), education timeline + cert badges, CTA to Praise |
| Praise | `redesign/testimonials.html` | 7 curated testimonials |

### Visualizations inventory
| Viz | Page | Type |
|-----|------|------|
| Stats strip | index | 4 big numbers |
| Tenure bar chart | index | horizontal mini-bars |
| Brianna pull-quote | index | styled blockquote |
| Bell curve (job satisfaction) | method | inline SVG |
| Diagnostic funnel | method | vertical CSS rail + colored dots |
| Animated skill bars | method | CSS bars + IntersectionObserver |
| Duct Tape / Drano panels | method | two-panel card |
| Career timeline | work | horizontal CSS rail + colored dots |
| Education timeline | about | vertical CSS rail + dots |
| Cert badges | about | 2×2 card grid |
| Portrait mini-bars (tea) | about | tiny CSS bars |
| CareerRiver image | work | PNG illustration |

### Images — all accounted for
| File | Use |
|------|-----|
| `AboutHero.png` | about.html — "The Human Behind the Projects" |
| `ThreePillars.png` | about.html — "Three Things I Always Bring" |
| `TeachingScene.png` | about.html — "One More Thing" |
| `ThingsILove.png` | index.html — "The work, briefly" section thumbnail |
| `Testimonials.png` | testimonials.html — "What People Say" |
| `Education.png` | about.html — "Education & Certifications" |
| `ProfilePicture.jpeg` | about.html hero avatar + index.html hero |
| `CareerRiver.png` | work.html — career journey |

---

## Still open

- **Browser QA** on all 4 pages (especially About's new 4-col grid + testimonials themes row wrapping on narrow screens).
- **Images still needed** (3 remaining — Nabil to create externally and drop in):
  - Three Pillars illustration (replace `ThreePillars.png`)
  - Kernel Updates before/after dot-grid (for work.html case study — no image yet)
  - Testimonial word cloud (replace `Testimonials.png`)
- Decide if/when to promote `redesign/` to replace the root site

### Images — done
| File | Use |
|------|-----|
| `CareerJourneyPainted.png` | work.html — career journey illustration ✅ |
| `EducationWalkPainted.png` | about.html — Education & Certifications ✅ |

---

## Copy & content suggestions (not yet implemented)

These are editorial changes identified in review — none require new illustrations, just copy edits or small structural decisions.

### High priority

**1. Footer copy — unify across all 4 pages**
Currently mismatched: index + about say "Let's talk about your next project." (job-seeker-y); work + method say "If you would like to chat." Pick one voice for all four. Suggested: "Always up for a good conversation." or "In my element when there's an interesting problem in the room." — keeps the door open without hustling.

**2. "Six stories, told in steps." on home — fix count and framing**
index.html Selected Work card currently says "Six stories, told in steps." Work page has 7 projects, and only iTunes/iCloud/Kernel have step-by-step treatment. Two fixes: (a) update the count, (b) reframe the description so it doesn't oversell the lighter pieces.

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

**9. Career chip strip on work.html — consider removing**
work.html has: painted illustration → 5-node career timeline → chip-arrow strip (Elegrity → eBay → Apple → MS Business Analytics · 2022 → SFMTA). That's three views of the same arc. The chip strip also drops the consulting period and substitutes "MS Business Analytics · 2022" as a career stop, which is odd. The timeline already carries this; the chip strip adds noise.

**10. Cert badges — trim**
about.html has 4 badges: Google Cloud Essentials, Data ML & AI Baseline, Scientific Data Processing, Microsoft Excel. For someone with 19 years and an MS in Business Analytics, certifying Excel reads as overcorrecting. At minimum drop the Excel badge. Could collapse all four to a single line: "Google Cloud + ML foundations, 2024."

**11. Bell curve peak label — let the caption work harder**
method.html bell curve peak is labeled "Trust / Vision / Leadership" — abstract noun stack. The caption already says "trusted with the vision, given room to lead" which is much better. Consider replacing the peak callout with something concrete like "Hand me the vision, get out of the way." and letting the caption explain it.

**12. Brianna pull quote — trim for punch**
index.html quote: "He has the unique ability to walk into an ambiguous situation, quickly grasp the key milestones and action items, identify technical needs that have not been addressed, and get results — all while getting a smile out of everyone in the room."
Middle clause ("quickly grasp the key milestones and action items") dilutes it. Suggested trim: "He walks into ambiguous situations, identifies what hasn't been addressed, and gets results — all while getting a smile out of everyone in the room."

### Lower priority / additive

**15a. "Now" strip on home**
A small strip (Derek Sivers /now-page convention) showing what's currently on the SFMTA workbench (anonymized), what Nabil is reading, current tea. Reinforces "not job-hunting, just available for conversation." Would sit naturally between the stats strip and the Brianna quote, or at the very bottom before the footer.

**15c. Cat cameo in footer or hero**
Cats currently appear in chips and the portrait grid. A single candid line somewhere — e.g. "Reviewed by Octavia" in the footer, or a one-liner in the hero — is the kind of whimsy that makes a site memorable without taking up space.

**16b. Dead CSS in work.html — clean up**
work.html contains unused `.section-banner` and `.river-cta` CSS rules. Worth removing once the redesign is promoted to root.

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
- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--coral` on Home/Work · `--teal` on Method · `--lavender` on About
- Nav is self-contained within `redesign/`
- Home hero portrait + Work CareerRiver reference `../inspiration_samples/` — not moved
- LinkedIn profile PDF in repo root (`linked_in_profile.pdf`)
