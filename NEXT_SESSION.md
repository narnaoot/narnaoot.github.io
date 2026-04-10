# Next Session Handoff

## Current branch

`master` — all work is committed and pushed directly to master.

---

## What's done

### redesign/ — fully built, fully linked site

| Page | File | Status |
|------|------|--------|
| Home | `redesign/index.html` | Done |
| Work | `redesign/work.html` | Done — CareerRiver image, 4 case studies |
| Method | `redesign/method.html` | Done |
| About | `redesign/about.html` | Done — 4 sections with thumbnail insets |
| Praise | `redesign/testimonials.html` | Done — 15 testimonials + education/certs |

Nav on all 5 pages: Home · Work · Method · About · Praise

### Images — all resolved

All section thumbnails live in `redesign/` and are referenced with simple relative paths (no `../`).

| File | Use | Status |
|------|-----|--------|
| `AboutHero.png` | about.html — "The Human Behind the Projects" | ✓ |
| `ThreePillars.png` | about.html — "Three Things I Always Bring" | ✓ |
| `TeachingScene.png` | about.html — "One More Thing" | ✓ |
| `ThingsILove.png` | about.html — "Things I Love" | ✓ |
| `Testimonials.png` | testimonials.html — "What People Say" | ✓ |
| `Education.png` | testimonials.html — "Education & Certifications" | ✓ |
| `ProfilePicture.jpeg` | about.html hero avatar | ✓ |

`inspiration_samples/CareerRiver.png` is still referenced by `work.html` (unchanged, working).

---

## Still open

None known. The redesign is feature-complete with all images wired up.

Possible next steps:
- Review/QA each page in a browser
- Decide if/when to promote `redesign/` to replace the root site
- Any copy or content edits

---

## Technical notes

- All redesign work lives in `redesign/` — root files untouched
- Design tokens: `--coral`, `--teal`, `--mustard`, `--lavender`, `--sage`
- Fonts: Playfair Display (headings) + Nunito (body)
- Hero kicker color: `--lavender` on About + Praise; `--coral` on Work + Method
- Nav is fully self-contained within `redesign/` (no `../` links)
- `inspiration_samples/old/` — all files are 2-byte corrupt stubs, not recoverable
