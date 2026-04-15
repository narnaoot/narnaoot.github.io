# Next Session Handoff

## Current branch

`claude/review-website-docs-P8MwH` — redundancy/reorganization pass. Not yet merged to master.

---

## What changed this session (redundancy & reorganization pass)

### 1. index.html — eliminated repeated messaging
- The hero, about-lead, and about-body all said "ambiguous situations → clarity" in different words. Collapsed to: hero keeps the core message, about-body now tells a *different* story (Apple specifics, iCloud).
- Superpower side-fact changed from "0 → 1 / making the invisible legible" (said elsewhere) to a fresh line.

### 2. about.html — removed redundant section, reorganized
- **Removed "Things I Love" grid** — it duplicated the portrait grid directly above it (cats, tea, books, SF, 0→1 all appeared in both).
- **Removed Ipsita quote** from teaching vignette (it lives as a full testimonial on the Praise page). Vignette now ends with its own conclusion.
- **Added Education & Certifications** (moved from testimonials.html — it's "about" content, not "praise" content). Education.png thumbnail included.
- **Removed Bell Curve** ("My Professional Sweet Spot") — moved to method.html where it belongs.
- Kept: portrait grid, three pillars, teaching vignette, CTA to Praise page.

### 3. method.html — merged questions, added visualizations
- **Merged Q2 + Q4** ("What is keeping you from getting your work done?" and "What's getting in your way?" were the same question). Now 5 questions instead of 6.
- **Converted questions from flat grid cards to a visual funnel/flowchart** with colored dots and a connecting rail — shows the diagnostic process as a narrowing sequence.
- **Added Bell Curve** ("My Professional Sweet Spot") between Duct Tape/Drano and Skill Toolkit.
- **Drano panel note** changed from "Love going from 0 to 1" (repeated on about.html) to concrete examples.

### 4. testimonials.html — simplified
- **Removed Education & Certifications section** (moved to about.html).
- Hero subtitle updated (no longer references education/credentials).
- Now purely a testimonials page — 15 quotes, no other content.

---

## Current page structure

| Page | File | Sections |
|------|------|----------|
| Home | `redesign/index.html` | Hero, stats strip, Brianna pull-quote, about blurb + side-facts, 3 project cards |
| Work | `redesign/work.html` | CareerRiver image, 4 case studies |
| Method | `redesign/method.html` | 5-question diagnostic funnel, Duct Tape/Drano, Bell Curve, skill toolkit |
| About | `redesign/about.html` | Portrait grid, Three Pillars, teaching vignette, Education & Certs, CTA to Praise |
| Praise | `redesign/testimonials.html` | 15 testimonials (pure) |

Nav on all 5 pages: Home · Work · Method · About · Praise

### Images

| File | Use | Status |
|------|-----|--------|
| `AboutHero.png` | about.html — "The Human Behind the Projects" | ✓ |
| `ThreePillars.png` | about.html — "Three Things I Always Bring" | ✓ |
| `TeachingScene.png` | about.html — "One More Thing" | ✓ |
| `ThingsILove.png` | *No longer used* (section removed) | orphan |
| `Testimonials.png` | testimonials.html — "What People Say" | ✓ |
| `Education.png` | about.html — "Education & Certifications" | ✓ (moved) |
| `ProfilePicture.jpeg` | about.html hero avatar | ✓ |
| `CareerRiver.png` | work.html — career journey | ✓ |

---

## Questions for Nabil (saved up during this pass)

1. **ThingsILove.png** is now an orphan — should we delete it, or repurpose it?
2. **Brianna Gamp quote** appears on both the homepage (featured pull-quote) and the Praise page (first testimonial). I kept both — the homepage feature feels intentional, not redundant. Agree?
3. **Three Pillars** (from Mary Salome) — is this a friend's description? It's beautiful but very personal. Do you want it on a professional portfolio, or should it be reframed?
4. **Method page now has 4 sections** (funnel, duct tape/drano, bell curve, skill toolkit). Is that too much for one page, or does the flow feel right?
5. **Praise page is now just testimonials** (15 quotes, nothing else). Should we add anything else, or is pure-testimonials the right call?

---

## Still open

- Review/QA each page in a browser
- Decide if/when to promote `redesign/` to replace the root site
- Consider whether ThingsILove.png should be deleted or repurposed
- Any copy or content edits

---

## Technical notes

- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--lavender` on About + Praise; `--coral` on Work + Method
- Nav is fully self-contained within `redesign/` (no `../` links)
- `inspiration_samples/old/` — all files are 2-byte corrupt stubs, not recoverable
