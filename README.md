# narnaoot.github.io — Nabil Arnaoot's personal site

Personal portfolio for Nabil Arnaoot — Principal Business Analyst and project leader at SFMTA. Plain static HTML, deployed via GitHub Pages at **n4bil.com** (see `CNAME`).

## Emphasis

Foregrounds **project leadership** — walking into ambiguous situations, finding the real problem, building the process that's missing, and delivering. Data/analytics is a supporting capability, not the headline.

## Site structure (all live, at repo root)

| Page | Contents |
|------|----------|
| `index.html` | Home — hero, stats strip, pull quote, "The work, briefly", selected-work teaser + cards |
| `work.html` | Career through-line · 3 deep case studies (eBay, iTunes, Kernel) · 3 lighter reads linking to the note pages |
| `patterns.html` | Favorite questions · Duct Tape / Drano · Everything Starts on a Whiteboard · Microchipping Sheep · What I Bring |
| `about.html` | Personal portrait · three pillars · teaching · off-the-clock (feminist SF) · testimonials · education & certs |
| `gardens.html` | Secret Gardens of San Francisco — Tableau embed |
| `probability.html` | Conditional Probability for Normal Humans — essay + tables |
| `unicorns.html` | Chasing Unicorns for Pride — Tableau embed |

Masthead nav (4 main pages): Home · Work · Patterns · About. The three note pages link back from Work.

## Design system

Each page carries its own `:root` token block and inline `<style>`, plus a signature accent used for the wordmark, nav underline, and footer/button chrome:

| Page | Accent |
|------|--------|
| Home | orchid |
| Work | coral |
| Patterns · Unicorns | teal |
| About | lavender |
| Gardens | sage |
| Probability | mustard |

Shared palette: warm cream `--bg #FFFBF5`, ink `--text #3D2B1F`, `--muted #7C6151`; accents `--coral #F5563F`, `--teal #12C2B0`, `--mustard #F0A500`, `--sage #4FB870`, `--lavender #9B6DE8`, `--orchid #A75FA0` (plus `--denim`, `--blush`, `--citron`). Each accent has a deep `-dk` cut for legible colored text on tinted backgrounds (e.g. `--teal-dk #14655D`), so text-on-tint pairings clear WCAG AA.

Fonts: **Libre Caslon Text** (serif headings) + **Nunito** (body).

## Assets

All illustrations are WebP (converted from source PNG/JPEG; the originals remain in git history). Root images:

| File | Where used |
|------|------------|
| `Monogram.svg` | masthead logo (all pages) |
| `ProfilePicture.webp` | Home + About hero avatar |
| `CleoInspects.webp` | "Inspected by Cleo" footer (all pages) |
| `CareerJourneyPainted.webp` | Work — career through-line |
| `LighthousePainted.webp` | Work — eBay case study |
| `QuietedPagersPainted.webp` | Work — iTunes case study; also the Home teaser thumbnail |
| `KernelCleanupPainted.webp` | Work — Kernel case study |
| `AboutHero.webp`, `ThreePillarsPainted.webp`, `TeachingScene.webp`, `WordCloudsPainted.webp`, `EducationWalkPainted.webp` | About section thumbnails |
| `duct_tape.webp`, `drano.webp` | Patterns — Two Kinds of Problems panels |
| `microchip.webp` | Patterns — Microchipping Sheep (whiteboard photo) |
| `icons/*.png` | Home chips + About portrait icons (book, cats, house, tea) |

The repo now holds only what the live site uses. Prior source PNG/JPEG originals, reference imagery (`inspiration_samples/`), and old site versions were removed from the working tree and remain in git history.

## Working notes

- `plan/NEXT_SESSION.md` — running handoff / review log and current open items.
- `plan/Inspiration.md` — design research and reference designers (its image links point at the removed `inspiration_samples/`; the notes still read fine, images are in git history).
