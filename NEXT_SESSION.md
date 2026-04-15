# Next Session Handoff

## Current branch

`claude/review-website-docs-P8MwH` — redundancy/reorganization pass + LinkedIn content additions. Not yet merged to master.

---

## What changed (two rounds of work)

### Round 1: Redundancy & reorganization

#### index.html
- Eliminated 3x repetition of "ambiguous situations → clarity" (hero, about-lead, about-body). Hero keeps the message; about-body now tells a *different* story (Apple specifics, iCloud).
- Superpower side-fact changed from "0 → 1" (said elsewhere) to a fresh line.
- **Added ThingsILove.png** as section thumbnail for "The work, briefly" (repurposed from removed section).

#### about.html
- **Removed "Things I Love" grid** — duplicated the portrait grid above it.
- **Removed Ipsita quote** from teaching vignette (kept on Praise page only).
- **Added Education & Certifications** (moved from testimonials.html).
- **Removed Bell Curve** — moved to method.html.
- **Added nonprofit data consulting** to teaching vignette (from LinkedIn — student → teacher → consultant arc).

#### method.html
- **Merged Q2 + Q4** (both "what's in your way?"). Now 5 questions instead of 6.
- **Converted questions to visual funnel** with colored dots and connecting rail.
- **Added Bell Curve** ("My Professional Sweet Spot") between Duct Tape/Drano and Skills.
- Drano panel note changed from "0 to 1" to concrete examples.

#### testimonials.html
- **Removed Education section** (moved to about.html).
- **Removed Brianna Gamp quote** (lives on homepage only).
- **Curated from 15 → 7 testimonials**. Kept: Robert Mooney, Chris Winter, Sneha Phadke, Faron Lyons, Kim Anderson, Frankie Hill, Ipsita.

### Round 2: LinkedIn content additions

#### work.html
- **Added iCloud case study** — outage tracking system built from scratch for 300M users. Step-by-step narrative.
- **Added eBay case study** — Site Security Program, risk prioritization, decision support.
- **Added role titles + dates** to all professional case studies (EPM 2011-14, BA/BPE 2014-18, PM 2009-11).
- Now 6 case studies: 3 professional (iTunes, iCloud, eBay), 3 personal/academic (SHAP, Secret Gardens, Conditional Probability).

---

## Current page structure

| Page | File | Sections |
|------|------|----------|
| Home | `redesign/index.html` | Hero, stats strip, Brianna pull-quote, about blurb w/ ThingsILove thumbnail + side-facts, 3 project cards |
| Work | `redesign/work.html` | CareerRiver image, 6 case studies (3 professional, 3 personal) |
| Method | `redesign/method.html` | 5-question diagnostic funnel, Duct Tape/Drano, Bell Curve, skill toolkit |
| About | `redesign/about.html` | Portrait grid, Three Pillars, teaching vignette (+ nonprofit consulting), Education & Certs, CTA to Praise |
| Praise | `redesign/testimonials.html` | 7 curated testimonials |

Nav on all 5 pages: Home · Work · Method · About · Praise

### Images — all accounted for

| File | Use | Status |
|------|-----|--------|
| `AboutHero.png` | about.html — "The Human Behind the Projects" | ✓ |
| `ThreePillars.png` | about.html — "Three Things I Always Bring" | ✓ |
| `TeachingScene.png` | about.html — "One More Thing" | ✓ |
| `ThingsILove.png` | index.html — "The work, briefly" section thumbnail | ✓ (repurposed) |
| `Testimonials.png` | testimonials.html — "What People Say" | ✓ |
| `Education.png` | about.html — "Education & Certifications" | ✓ (moved) |
| `ProfilePicture.jpeg` | about.html hero avatar + index.html hero | ✓ |
| `CareerRiver.png` | work.html — career journey | ✓ |

---

## Nabil's answers to questions from Round 1

1. ThingsILove.png → repurposed as index.html section thumbnail ✓
2. Brianna Gamp → removed from Praise page, kept on homepage only ✓
3. Three Pillars (Mary Salome) → keep as is ✓
4. Method page 4 sections → use judgement (kept all 4, flow is good) ✓
5. Testimonials → curated from 15 to 7 ✓

---

## Still open

- Review/QA each page in a browser
- Decide if/when to promote `redesign/` to replace the root site
- Any copy or content edits
- Consider: the 3 project cards on index.html still link to Work, Method, About — should the third card link to Praise instead now that About has more content?

---

## Technical notes

- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--lavender` on About + Praise; `--coral` on Work + Method
- Nav is fully self-contained within `redesign/` (no `../` links)
- `inspiration_samples/old/` — all files are 2-byte corrupt stubs, not recoverable
- LinkedIn profile saved as `linked_in_profile.pdf` in repo root
