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

---

## Current page structure

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
- Review/QA each page in a browser (especially the new timelines on mobile)
- Decide if/when to promote `redesign/` to replace the root site
- Any copy or content edits

---

## Technical notes
- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--lavender` on About + Praise; `--coral` on Work + Method; `--teal` on Method funnel
- Nav is fully self-contained within `redesign/` (no `../` links)
- LinkedIn profile: `linked_in_profile.pdf` in repo root
